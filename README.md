
# Azure Data Explorer Library
Azure Data Explorer pubic library of queries, functions & notebooks

This repository contains user functions, sample queries & notebookes for Azure Data Exlorer (Kusto). In order to test these queries you need to connect to a cluster & database. To store functions you need write permission for the specific database, or you can use the inline (lambda) version.

The Samples database on the Help cluster contains the tables required to test the sample queries, you can quickly connect to it using:

#connect cluster('help').database('Samples')

The structure of the repository:
* top level contains thematic folders (e.g. ML, Time Series etc.)
* in each thematic folder there are 3 sub-folders:
    * funtions - containing definition of stored and/or lambda functions
    * queries - demo queries
    * notebooks - demo Jupyter/Databricks notebooks

# Contributing

This project welcomes contributions and suggestions.  Most contributions require you to agree to a
Contributor License Agreement (CLA) declaring that you have the right to, and actually do, grant us
the rights to use your contribution. For details, visit https://cla.microsoft.com.

When you submit a pull request, a CLA-bot will automatically determine whether you need to provide
a CLA and decorate the PR appropriately (e.g., label, comment). Simply follow the instructions
provided by the bot. You will only need to do this once across all repos using our CLA.

This project has adopted the [Microsoft Open Source Code of Conduct](https://opensource.microsoft.com/codeofconduct/).
For more information see the [Code of Conduct FAQ](https://opensource.microsoft.com/codeofconduct/faq/) or
contact [opencode@microsoft.com](mailto:opencode@microsoft.com) with any additional questions or comments.
