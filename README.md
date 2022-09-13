# djangoplicity-mailmain

## Publishing a new version to PyPI

Increment the version number in setup.py (`version` and `download_url`)

Then run the following commands:
```
python3 -m pip install --upgrade build
python3 -m build
```

Tag it with the version, than push it to GitHub
```
git tag 0.4.x
git push origin main
```

Create a Release in https://github.com/djangoplicity/djangoplicity-mailman/releases

Then include the following files in the release:

```
dist/djangoplicity_mailman-0.4.2-py3-none-any.whl
dist/djangoplicity_mailman-0.4.2.tar.gz
```
