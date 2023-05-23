<!-- Links used on this page (Declaration) -->
[ABAP_GIT]:       https://docs.abapgit.org/


# How to pull our repositories
## Needed tools
You will need [abapGit][ABAP_GIT] to install our software on your system.

## Package structure
Since we are developing in our own namespace, all object names start with ```/USI/```. 
The latest version of abapGit handles namespaces automatically, so that no manual steps are required anymore.

However the package name used when creating an online repository must start with ```/USI/```.
Otherwise, abapGit will show an error message right after creating the repository.

Since all of our developments are encapsulated, it is recommended to use package type ```Main Package``` and to activate encapsulation.
This ensures that package checks will work properly if they are active in your system.

![Package_Builder_Create_Package](https://user-images.githubusercontent.com/86975244/234884419-10195267-123d-499d-9cda-5da492913f82.png)
