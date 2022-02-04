<!-- Links used on this page (Declaration) -->
[ABAP_GIT_NAMESPACES]: https://docs.abapgit.org/ref-namespaces.html


# What are Namespaces
USI developments take place in their own namespace. Namespaces are SAP's standard solution to avoid naming conflicts if software has to be distributed from one source system to a large number of target systems.

Using the "normal" customer namespace (Z*) would not solve this problem, since this namespace is open to anyone who has a developer key. If a developer has created an object that happens to have the same name as an object we are shipping, problems would occur during rollout.

Reserved namespaces solve this problem because a license key is required to develop in them. The owner of a namespace receives these license keys from SAP when registering the namespace. As long as he keeps these license keys to himself, it is technically ensured that nobody but him can develop in this namespace.

# Why you need our license key
When cloning a repository to a target system, abapGit technically creates the development object in that system. If the development objects belong to a reserved namespace, SAPs development tools will only allow this, if the namespace was previously registered on the development system.

The current version of [abapGit][ABAP_GIT_NAMESPACES] exports the key, but cannot (yet) automatically transfer it to new systems.

This is why you need to manually maintain the namespace once per system.

# Maintain repair license key
Namespaces can be maintained in transaction **SE03**.

You could find the details of our namespace in all repositories, that contain source code. 
The file is named "#usi#.nspc.xml" and can be found in the /src-folder.

For the sake of simplicity, I copied that information to the table below.


| Field          | Value                           |
| -------------- | ------------------------------- |
| Namespace      | /USI/                           |
| Namespace role | C                               |
| Repair License | 07181429931319159598            |
| Short Text     | Unternehmensgruppe Schwarz - IT |
| Owner          | Schwarz IT                      |
