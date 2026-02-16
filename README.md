# Oracle_pdb_Ass_II_27885_kevin

**Course**: Database Development with PL/SQL (INSY 8311)  
**Instructor**: MANIRAGUHA Eric
**My names**: Kevin Ntwari
**ID**: 27885
**Grpoup**: c
**Submission date**:16/2/2026
**Assignment**:Pluggable Database (PDB) Management – Assignment II

-----------Overview Of Task-------------

This assignment focused on practical skills in managing Oracle Multitenant Architecture.
The main objective was to understand how to create, manage, and monitor Pluggable Databases (PDBs) using Oracle tools.

The tasks completed include:

. Creating a new pluggable database following strict naming conventions
. Creating a dedicated user inside the PDB
. Creating and deleting a temporary PDB
. Accessing and configuring Oracle Enterprise Manager (OEM)
. Documenting the entire process professionally

-----------Oracle Environment Used------------

The practical work was completed using the following Oracle environment:

. Oracle Database Version: Oracle 21c
. Architecture: Multitenant (CDB & PDB)
. Tool Used: SQL*Plus 
. OEM: Oracle Enterprise Manager Database Express
. Operating System: Window

  ___Task 1- Create a New Pluggable Database___

.PDB Name: ke_pdb_27885

  __Steps Perfomed__
 1. Start with installing oracle version 21c
 2. Connected to the Container Database (CDB) as SYSDBA.
 3. Executed the CREATE PLUGGABLE DATABASE command using the required naming format.
 4. Opened the PDB using:
  .ALTER PLUGGABLE DATABASE OPEN;
 5. Saved the open state:
  . ALTER PLUGGABLE DATABASE SAVE STATE;
    
__User creation Inside PDB__
.Username: kevin_plsqlauca_27885

  __Steps__

1.Switched session to the created PDB.
2.Created the user with a password.
3.Granted necessary privileges (CONNECT, RESOURCE).

___Task 2 — Create and Delete a Temporary PDB___

.Temporary PDB Name: ke_to_delete_pdb_27885

__Creation Process__

.Executed the PDB creation command successfully.
.Verified existence using:
    SHOW PDBS;

__Deletion Process__

1.Closed the PDB:
ALTER PLUGGABLE DATABASE CLOSE IMMEDIATE;

2.Dropped the PDB completely:
DROP PLUGGABLE DATABASE ... INCLUDING DATAFILES;

3.Verified deletion using SHOW PDBS;
The temporary PDB no longer appeared in the list.

___Task 3 — Oracle Enterprise Manager (OEM)___

Oracle Enterprise Manager Database Express was configured and accessed via browser.

__Activities Performed__

.Logged in as SYSDBA
.Accessed the dashboard
.Verified Oracle environment status
.Confirmed visibility of created PDBs
.Monitored database health and storage

__The dashboard clearly displayed__:

.Container Database
.Created PDB
.Database services
.Active sessions

__Screenshots Evidence__
All required screenshots are stored in the repository under:  
__Contents include__:

PDB creation command
.Open PDB state
.User created inside PDB
.Temporary PDB creation
.Temporary PDB deletion
.OEM dashboard view

___Challenges Faced & Solutions___

__During the assignment, a few challenges were encountered:__

Challenge 1: Error while creating PDB due to file path issues.
Solution: Corrected the datafile directory path.

Challenge 2: User creation failed initially due to container mismatch.
Solution: Switched session to the correct PDB before creating the user.

These challenges helped improve my understanding of Oracle Multitenant architecture.

___Integrity Statement___

I hereby declare that this assignment work is my own practical effort.
All commands were executed and tested in my Oracle environment.
Screenshots provided are original and taken during my lab practice.

I understand that academic integrity and professional ethics are essential in database administration.
 
