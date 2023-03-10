# Dumbo Scopus

Simple CLI to search on Scopus and obtain the results in a XLSX file.


# Prerequisites

- Python 3.10
- An API key from [Elsevier](http://dev.elsevier.com)
- [ChromeDriver](https://sites.google.com/chromium.org/driver/downloads?authuser=0) (download and install the most appropriate version for your OS)



# Install

Install using `pip`:
```bash
$ pip install dumbo-scopus
```


# Usage

Get help directly from the command:
```bash
$ python -m dumbo_scopus --help
$ python -m dumbo_scopus search --help
$ python -m dumbo_scopus citations --help
```

Use the following command line to perform a Scopus Search and obtain the result as a CSV file:
```bash
$ python -m dumbo_scopus search "TITLE(magic sets)" --api-key=YOUR-API-KEY
```
Check [this web page](https://dev.elsevier.com/sc_search_tips.html) for the format of the query.

To download the citations of an article, given its Scopus ID as for example `2-s2.0-84949895809`, use the following command line:
```bash
$ python -m dumbo_scopus citations 2-s2.0-84949895809
```
