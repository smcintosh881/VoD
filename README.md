# VoD
Vulnerability of the Day CWE-250

Execution with Unnecessary Privileges

# Run Example
To run this example execute the command 

    `Python vulnerability.py`
 
We can see that the privilege is never returned 
to the lowest minimum required to excecute the code. 
Therefore the privilege stays raised and the user could
gain access to additional functionality that is granted with this
higher level of privilege. 

Mitigations:

- Do not give unecessary privalages to users. A temoprary link to a page that a user is usually not given access to may be safer than temporarily elivating privalages, or simply making a custom permission so that users have access to specifically only what they need to have access to.
- If displaying information to only certain users on a page then make sure to check that the user has the right to see the options before rendering say a button to give a user the permission to do something that only some users can do on that page. Also make sure to check the permission in the controller incase users somehow call the controller action without being able to see the view option that triggers it. The controller action would be a sanity check ot a check to make sure malicious users will not attempt to hack into the system.
