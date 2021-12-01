[![SIT](https://img.shields.io/badge/SIT-awesome-blueviolet.svg)](https://it.schwarz)
# Who we are and what we do

The Schwarz Group operates over 800 SAP systems with about 200 of them being productive. 
Some subtasks - like sending an email or writing the application log - came up again and again over time.

The USI development chapter was created to avoid the redundant implementation of such subtasks. 
Our goal is to provide reusable solutions for such repetitive tasks, that can easily be consumed by other developers.

You can think of our developments as a developer toolbox or a technical foundation, that can be used to:
* avoid redundancies
* boost developer productivity
* enhance your products with powerful features

# How to participate

If you are missing a feature or have a great idea, you can either open an issue or contribute code directly.

Please do not get confused if it takes us days or - depending on the size of your contribution - even weeks to merge your changes into the main branch.
This is NOT because we do not appreciate your work or simply do not care. In fact the opposite is the case.

Every contribution has to undego a rigorous internal review process before merging.
The code has to pass:
* ATC Checks
* Unit Tests
* A manual review by a developer (Yes, we will actually read every single line of that code!)
* Manual explorative tests

The list is not necessarily complete. If applicable, we might end up writing test code to test parts of the development in isolation.
And for the sake of compliance the review has to be documented internally and at least three different colleagues will be involved.

This process simply takes some time.

# Software catalog

We are currently offering the following components:

Component       | Description  
--------------- | -------------
[Authority check](https://github.com/SchwarzIT/sap-usi-authority-check) | Authority check for transactions (S_TCODE). Technical dependecy of many USI developments.
[Exception API](https://github.com/SchwarzIT/sap-usi-exception) | Contains the USI root exception class and a text getter API, that can convert exceptions texts into various formats, such as BAPIRET2 or SYMSG.
[Logging API](https://github.com/SchwarzIT/sap-usi-logging-api) | Creates complete, comprehensive logs with almost no effort and extends SAP's standard logging API by powerful features.
