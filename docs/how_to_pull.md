<!-- Links used on this page (Declaration) -->
[ABAP_GIT]:       https://docs.abapgit.org/

# Needed tools
You will need [abapGit][ABAP_GIT] to install our software on your system.

# Package structure
Since we are developing in our own namespace, all object names start with ```/USI/```. 
The latest version of abapGit handles namespaces automatically, so that no manual steps are required anymore.

However the package name used when creating an online repository must start with ```/USI/```.
Otherwise, abapGit will show an error message right after creating the repository.

It is recommended to use package type ```Main Package``` and to keep encapsulation deactivated.

![Package_Builder_Create_Package](https://github.com/user-attachments/assets/84eb778a-be8f-45ef-82fb-bd89950ba58e)
