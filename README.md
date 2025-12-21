# templates

Python project templates for quick and reliable setups.

## Installation

```console
pip install copier
git clone https://github.com/goessl/templates.git
```

## Usage

```console
cd templates
```

- For a **module** (single Python file package):
  ```console
  python -m copier copy module YOUR_PROJECT_NAME
  ```

- For a **C extension**:
  ```console
  python -m copier copy extension YOUR_PROJECT_NAME
  ```

- For a **package**:
  ```console
  python -m copier copy package YOUR_PROJECT_NAME
  ```

And then follow the appearing quastionnaire. Done!

## Design references

### `pyproject.toml`

[Python Packaging User Guide - Writing your pyproject.toml](https://packaging.python.org/en/latest/guides/writing-pyproject-toml/#a-full-example)
filtered and more ordered like [Python Packaging User Guide - pyproject.toml specification](https://packaging.python.org/en/latest/specifications/pyproject-toml/).
For extensions/setuptools [setuptools documentation - Configuring setuptools using pyproject.toml files](https://setuptools.pypa.io/en/latest/userguide/pyproject_config.html).

### `mkdocs.yml`

Derived from [squidfunk/mkdocs-material - mkdocs.yml](https://github.com/squidfunk/mkdocs-material/blob/master/mkdocs.yml).

### `LICENSE.txt`

[Choose a License - MIT License](https://choosealicense.com/licenses/mit/)

### `.gitignore`

[github/gitignore - Python.gitignore](https://github.com/github/gitignore/blob/main/Python.gitignore)

### `extension`

[python/cpython - Modules/xxlimited.c](https://github.com/python/cpython/blob/main/Modules/xxlimited.c) linked from [Python 3 documentation - Extending Python with C or C++](https://docs.python.org/3/extending/extending.html#the-module-s-method-table-and-initialization-function).

## Roadmap

- [x] Deploy
- [x] References
- [ ] Update extension C source
- [ ] Web interface
- [x] Ballin

## License (MIT)

Copyright (c) 2025 Sebastian Gössl

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
