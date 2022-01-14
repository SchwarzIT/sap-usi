<!-- Links used on this page (Declaration) -->
[ABAP_GIT_NAMESPACES]: https://docs.abapgit.org/ref-namespaces.html


# Maintain repair license key
USI developments take place in their own namespace. The objects can only be edited if at least the repair license key has been maintained in the development system. 
The current version of [abapGit][ABAP_GIT_NAMESPACES] exports the key, but cannot (yet) automatically transfer it to new systems.

For this reason, the repair license key must be manually maintained once in transaction SE03 before the first repository is cloned to a system. 
The relevant data of our namespace can also be found in the src-directories (#usi#.nspc.xml) of our repositories, but for the sake of simplicity I copied them into this document.

| Field          | Value                           |
| -------------- | ------------------------------- |
| Namespace      | /USI/                           |
| Namespace role | C                               |
| Repair License | 07181429931319159598            |
| Short Text     | Unternehmensgruppe Schwarz - IT |
| Owner          | SITIOS                          |
