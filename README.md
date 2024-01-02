In order to follow proper standards in maintaining the code, we require the following packages in order to verify the code

1. Black (to modify the code based on pep8 standards)
2. Flake8 (To check whether the code follows the pep8 standards or not)
3. "Isort" (is to sort modules in a alphabetical manner)
4. interrogate (it is used to check whether the code is properly documented or not)
5. "".pre-commit-config.yaml" is used to create hooks for the above packages in github
6. pdoc3 is a document string library uses to generate a api document for the given code based on the doc strings

Steps:

1. black -> flake8 -> isort -> interrogate -> pre-commit install -> git add . -> git commit -m "code standards" --no-verify
2. TO create a doc file using pdoc3 from given code and save it in local docs folder
pdoc --html calculator.py --output-dir docs
3. If you want to see live updates to the documentation as you change your code, you can start a live-reloading server with:
  pdoc --http :8000 calculator.py 




