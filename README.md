# Oracle Pluggable Database Assignment II

## Student Information

Name: Mohamed  
Student ID: 28224  
Course: INSY 8311 – Database Development with PL/SQL  


## Overview

This assignment focuses on practical implementation of Oracle Multitenant Architecture using Oracle Database 19c. The tasks involved creating and managing Pluggable Databases (PDBs), creating users inside a PDB, deleting a temporary PDB, and verifying the configuration using Oracle Enterprise Manager (OEM).


## Task 1 – Creation of Main Pluggable Database

In this task, I connected to the Oracle Container Database (CDB) as SYSDBA and created a new Pluggable Database using the required naming convention:

PDB Name: `mo_pdb_28224`

After successfully creating the PDB, I opened it and verified that its status was OPEN. I then switched the session to the newly created PDB and created a user inside it:

Username: `mohamed_plsqlauca_28224`

This user was granted the necessary privileges (CONNECT and RESOURCE) to be used for future PL/SQL laboratory work. The successful creation and configuration of the PDB were verified using SQL commands.



## Task 2 – Creation and Deletion of Temporary PDB

In this task, I created a temporary Pluggable Database named:

`mo_to_delete_pdb_28224`

After confirming that the PDB was created successfully and opened properly, I proceeded to close it using the CLOSE IMMEDIATE command. Then, I deleted the PDB completely using the DROP PLUGGABLE DATABASE command including datafiles.

Finally, I verified that the temporary PDB no longer existed by checking the list of available PDBs. This ensured that the deletion process was completed successfully.



## Task 3 – Oracle Enterprise Manager (OEM)

In this task, I accessed Oracle Enterprise Manager (OEM) through the browser interface. After logging in as SYSDBA, I navigated to the Pluggable Databases section to verify that my created PDB (`mo_pdb_28224`) was visible and in OPEN state.

The OEM dashboard confirmed that the Oracle environment was functioning correctly and reflected the completed PDB tasks. Screenshots of the dashboard and PDB details are included in the repository as evidence.


## Challenges Faced

During the configuration of Oracle Enterprise Manager, a port conflict error was encountered. The issue was resolved by resetting and reconfiguring the HTTPS port using the DBMS_XDB_CONFIG package. After restarting the database, OEM became accessible successfully.



## Integrity Statement

I confirm that this assignment was completed individually. All commands were executed by me, and all screenshots represent my own practical work.
