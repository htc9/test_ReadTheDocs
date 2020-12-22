# test_ReadTheDocs
This repo is being used to test connecting a Read the Docs to a github repo.

The Read the Docs test can be found here: https://testing-clewscan.readthedocs.io/en/latest/


## Important Files and Directories
* **docs/index.rst**
	* Documentation master file
	* Table of contents
* **docs/pages/**
	* In this directory are all the additional .rst files to make the html pages
* **docs/conf.py**
	* Configuration file for the Sphinx documentation builder

[Not in Repository, but possibly applicable]
* **docs/\_build/html/**
	* In this directory are all the .html files 
* **docs/\_build/html/pages/**
	* In this directory are all the .html files for the pages


## Building New Pages
(Basic instructions, look online for more detailed explanations)
1. In the directory **pages/**, create a new .rst file
2. Write into .rst file whatever is desired
3. In index.rst, add it under the toctree section. Example:
```
.. toctree::
   :maxdepth: 2
   :caption: Contents:

   pages/testing
   pages/intro
   pages/references
   pages/contacts
```
4. Commit .rst files into the repository
5. Read the Docs (if already connected) will update automatically

[Optional] - Only if an additional html page without Read the Docs is desired

6. In the command line, write
```bash
cd docs
make html
```
7. Now the HTML pages will be in the directory '\_build/html/pages'

## Read The Docs
This repository is linked to a Read the Docs, which will automatically
be updated as changes are made as long as the respository stays public.





