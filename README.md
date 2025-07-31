# genericPiPyPackage

This is a simple example Python package. [Here](https://packaging.python.org/en/latest/tutorials/packaging-projects/) you can find instructions on how to create a package. The [TestPyPi](https://test.pypi.org/)-index allows you to upload packages for testing.

## Instructions

### Build Backend

Upgrade *build*:
```
py -m pip install --upgrade build
```

Build Package:
```
py -m build
```

### Upload

Install *twine*:
```
py -m pip install --upgrade twine
```

Upload to TestPyPi:
```
py -m twine upload --repository testpypi dist/*
```
You will be prompted to enter your API token.

### Installation

```
py -m pip install --index-url https://test.pypi.org/simple/ --no-deps example-package-YOUR-USERNAME-HERE
```

### Edit Markdown files

Shortcut to render Markdown in VS Code

```
ctrl + k and v
```
