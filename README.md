<!-- Links used on this page (Declaration) -->
[ABAP_GIT]:       https://docs.abapgit.org/
[CONTRIBUTING]:   ./docs/CONTRIBUTING.md


[![SIT](https://img.shields.io/badge/SIT-About%20us-%236e1e6e)](https://it.schwarz/en)

# USI Development Chapter
## Who we are and what we do

The Schwarz Group operates over 800 SAP systems with about 200 of them being productive. 
Some subtasks - like sending an email or writing the application log - came up again and again over time.

The USI development chapter was created to avoid the redundant implementation of such subtasks. 
Our goal is to provide reusable solutions for such repetitive tasks, that can easily be consumed by other developers.

You can think of our developments as a developer toolbox or a technical foundation, that can be used to:
* avoid redundancies
* boost developer productivity
* enhance your products with powerful features

## Getting started
The following activities must be performed once for each relevant development system:
* install [abapGit][ABAP_GIT]

**HINT**: Since our developments take place in a dedicated namespace, the package name used in abapGit must start with ```/USI/```. It is recommended to use the package type ```Main Package``` and to activate encapsulation.

![Package_Builder_Create_Package](https://user-images.githubusercontent.com/86975244/234884419-10195267-123d-499d-9cda-5da492913f82.png)

## How to contribute
Please check our [contribution guidelines][CONTRIBUTING] to learn more about this topic.

## Software catalog

We are currently offering the following components:

Component       | Description  
--------------- | -------------
[Authority check](https://github.com/SchwarzIT/sap-usi-authority-check) | Authority check for transactions (S_TCODE). Technical dependecy of many USI developments.
[Exception API](https://github.com/SchwarzIT/sap-usi-exception) | Contains the USI root exception class and a text getter API, that can convert exceptions texts into various formats, such as BAPIRET2 or SYMSG.
[Logging API](https://github.com/SchwarzIT/sap-usi-logging-api) | Creates complete, comprehensive logs with almost no effort and extends SAP's standard logging API by powerful features.
