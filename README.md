[![SIT](https://img.shields.io/badge/SIT-About%20us-%236e1e6e)](https://it.schwarz)

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

## How to participate

If you are missing a feature or have a great idea, you can open an issue.

You can also contribute code, but please ensure, that new features are matching the overall purpose of the component.
If you are not sure about that, just open an issue and discuss it with us beforehand.

Please do not get confused if it takes us days or - depending on the size of your contribution - even weeks to merge your changes into the main branch.
This is NOT because we do not appreciate your work or simply do not care. In fact the opposite is the case.

Every new version has to undergo a rigorous internal review process before merging.
The code has to pass:
* ATC Checks
* Unit Tests
* A manual review by a developer (Yes, we will actually read every single line of that code!)
* Manual explorative tests

The list is not necessarily complete. If applicable, we might end up writing test code to test parts of the development in isolation.
And for the sake of compliance the review has to be documented internally and at least three different colleagues will be involved.
This process simply takes some time.

Please do not get intimidated by that review process.
We will not make that your problem and we will try to keep things friendly.

As long as the new version does not introduce harmful things like e.g. bugs or security issues, we will accept the pull request.
If your code does not comply to our internal guidelines, we will refactor it internally, so that it passes the review process.
After that we will merge your version into the main branch right before pushing our refactored version into the main branch.

## Software catalog

We are currently offering the following components:

Component       | Description  
--------------- | -------------
[Authority check](https://github.com/SchwarzIT/sap-usi-authority-check) | Authority check for transactions (S_TCODE). Technical dependecy of many USI developments.
[Exception API](https://github.com/SchwarzIT/sap-usi-exception) | Contains the USI root exception class and a text getter API, that can convert exceptions texts into various formats, such as BAPIRET2 or SYMSG.
[Logging API](https://github.com/SchwarzIT/sap-usi-logging-api) | Creates complete, comprehensive logs with almost no effort and extends SAP's standard logging API by powerful features.
