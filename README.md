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
