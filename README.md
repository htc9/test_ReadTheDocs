# test_ReadTheDocs
This repo is being used to test connecting a Read the Docs to a github repo.

The Read the Docs test can be found here: https://testing-clewscan.readthedocs.io/en/latest/


## Important Files and Directories
* **docs/index.rst**
	* Documentation master file
	* Table of contents
* **docs/pages/**
	* In this directory are all the .rst files to make the html pages
* **docs/\_build/html/**
	* In this directory are all the .html files 
* **docs/\_build/html/pages/**
	* In this directory are all the .html files for the pages


## Building New Pages
(Undetailed instructions)
1. In the directory **pages/**, create a new .rst file
2. Write into .rst file whatever is desired
3. In index.rst, add it under the toctree section
4. In command line, write
```bash
cd docs
make html
```
5. Now the HTML pages will be in the directory '\_build/html/pages'


## Read The Docs
This repository is linked to a Read the Docs, which will automatically
be updated as changes are made



