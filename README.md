# djangoplicity-mailmain

## Publishing a new version to PyPI

Increment the version number in setup.py (`version`)

Build the package:
```
python3 -m pip install --upgrade build
python3 -m build
```

Install twine
```
python3 -m pip install --upgrade twine
```

Then publish the package to PyPI
```
python3 -m twine upload dist/*
```
> **IMPORTANT**: You will be prompted for a username and password. For the username, use __token__. For the password, use the token value, including the pypi- prefix.
> **IMPORTANT2**: In case you didn't read, the username is "__token__"

For more information see:
- https://packaging.python.org/en/latest/tutorials/packaging-projects/
