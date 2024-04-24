# Sphinx

## Check the current version of Sphinx
```
sphinx-build --version
```


## Change directory
```
cd docs
```

## Install Sphinx
```
pip install -U sphinx (poetry add)
```


## Generate documentation
```
sphinx-quickstart
```

## Change directory
```
cd ..
```

## Generate the .rst files: Use the sphinx-apidoc -o docs command. to automatically generate .rst (reStructuredText) files for the Python modules in your project. This command will generate .rst files for all Python modules in the current directory and place these files in the docs directory.
```
sphinx-apidoc -o docs .
```

## Add your modules to the Python path: Sphinx needs to be able to import your modules to generate documentation. You can add your project's root directory to the Python path at the beginning of your conf.py file:
```
import os
import sys
sys.path.insert(0, os.path.abspath('..'))

extensions = ['sphinx.ext.todo', 'sphinx.ext.viewcode', 'sphinx.ext.autodoc']
```

## Change directory
```
cd docs
```

## Make HTML
```
.\make.bat html
```
