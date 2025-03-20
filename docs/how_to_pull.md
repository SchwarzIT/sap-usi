<!-- Links used on this page (Declaration) -->
[ABAP_GIT]:       https://docs.abapgit.org/
[COMP_AC]:        https://github.com/SchwarzIT/sap-usi-authority-check
[COMP_CX]:        https://github.com/SchwarzIT/sap-usi-exception
[COMP_LG]:        https://github.com/SchwarzIT/sap-usi-logging-api

# Needed tools
You will need [abapGit][ABAP_GIT] to install our software on your system.

# Parent packages
It seems like ABAPGit also exports the parent packages of a repositories main package. If you are getting random error messages for /USI/-packages you never heard of, you might need to create the following package structure manually.

| Package name        | Description                      | Superpackage | Package type | Package encapsulated | Parent package of          |
| ------------------- | -------------------------------- | ------------ | ------------ | -------------------- | -------------------------- |
| /USI/GLOBAL         | Main package /USI/               | N/A          | Structure    | No                   | N/A                        |
| /USI/INFRASTRUCTURE | Basis, security, access          | /USI/GLOBAL  | Structure    | No                   | [USI Exception][COMP_CX]   |
| /USI/DEVELOPMENT    | USI Development                  | /USI/GLOBAL  | Structure    | No                   | [USI Logging API][COMP_LG] |
| /USI/SECURITY       | USI Development for SAP Security | /USI/GLOBAL  | Structure    | No                   | [USI Auth][COMP_AC]        |

# Target Package
Since we are developing in our own namespace, all object names start with ```/USI/```. 
The latest version of abapGit handles namespaces automatically, so that no manual steps are required anymore.

However the package name used when creating an online repository must start with ```/USI/```.
Otherwise, abapGit will show an error message right after creating the repository.

It is recommended to use package type ```Main Package``` and to keep encapsulation deactivated.

![Package_Builder_Create_Package](https://github.com/user-attachments/assets/84eb778a-be8f-45ef-82fb-bd89950ba58e)
