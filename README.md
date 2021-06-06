# Domain Checker

## Project description

The challenge originated in an audit project to identify whether a number of website domains owned by an organisation were still required. A list of these domains existed although in some cases it was unclear which area of the business they "belonged" to. 

The solution was twofold:

1. To develop a application using Python to read in a list of domains contained in a csv file, iterate for each domain to acquire WHOIS data and perform a DNS lookup to obtain IP address, and output to a spreadsheet all the information about the domain (IP address, Registrar, Expiration date and whether the WHOIS query found the domain or failed due to timeouts).
2. To use regular expressions to identify patterns in domain names relating to different areas of the business, bin the data into categories, and output as columns in a spreadsheet. This would help determine which ones to keep because they were currently in use, may be used in the future, or were required for purposes of intellectual property and brand protection.

## Source

Test dataset created for the purpose of testing the algorithm. 

## Requirements

* Python 3.8.x
* whois: a Python wrapper of a client for WHOIS directory service
* click: a Python package for creating command line interfaces