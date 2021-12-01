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

If you are missing a feature or have a cool idea, you can always open an issue.

You can also contribute code.

Since our developments must undergo a rigorous review process, we will never merge code from a pull request directly in GitHub. Instead, we will transfer the code to our backend system and perform quality assurance there. After the code has passed all checks, it is transferred to the repository via abapGit.

If you want your contribution to be linked to your user account, we need your email address because gitHub identifies user accounts by their respective email addresses. If you submit your email address with the pull request, we will use it to identify you as the author of the commit. If you don't, there is no way we know of to mark you as the author.

# Software catalog

We are currently offering the following components:

Component       | Description  
--------------- | -------------
[Authority check](https://github.com/SchwarzIT/sap-usi-authority-check) | Authority check for transactions (S_TCODE). Technical dependecy of many USI developments.
[Exception API](https://github.com/SchwarzIT/sap-usi-exception) | Contains the USI root exception class and a text getter API, that can convert exceptions texts into various formats, such as BAPIRET2 or SYMSG.
[Logging API](https://github.com/SchwarzIT/sap-usi-logging-api) | Creates complete, comprehensive logs with almost no effort and extends SAP's standard logging API by powerful features.
