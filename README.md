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
  python -m copier copy module MODULE_NAME
  ```

- For a **package**:
  ```console
  python -m copier copy package PACKAGE_NAME
  ```

- For a **C extension**:
  ```console
  python -m copier copy extension EXTENSION_NAME
  ```

And then follow the appearing quastionnaire. Done!

## Design references

```bash
MODULE_NAME
│   .gitignore                  Every repository needs this
│   LICENSE                     and this
│   README.md                   and that.
│   
│   pyproject.toml              Pythons necessary packaging metainformation.
│   py.typed                    Enable typing.
│   
│   MODULE_NAME.py              Your actual code comes here.
│   test_MODULE_NAME.py         Tests come here.
│   
│   mkdocs.yml                  Optional: MkDocs configuration.
│   index.md                    Webpage.
│   mathjax.js                  MathJax for math.

PACKAGE_NAME
│   .gitignore                  Every repository needs this
│   LICENSE                     and this
│   README.md                   and that.
│   
│   pyproject.toml              Pythons necessary packaging metainformation.
│   
├───PACKAGE_NAME
│       __init__.py             Necessary package entry point.
│       MODULE_NAME.py          Your actual code comes here.
│       py.typed                Enable typing.
│   
├───tests
│       test_MODULE_NAME.py     Tests come here.
│   
│   mkdocs.yml                  Optional: MkDocs configuration.
├───docs
│       index.md                Landing page.
│       MODULE_NAME.md          Module documentation.
│       mathjax.js              MathJax for math.

[EXTENSION_NAME]
│   .gitignore                  Every repository needs this
│   LICENSE                     and this
│   README.md                   and that.
│   
│   pyproject.toml              Pythons necessary packaging metainformation.
│   
├───EXTENSION_NAME
│       __init__.py             Necessary package entry point.
│       _pyEXTENSION_NAME.py    Python implementation comes here.
│       _EXTENSION_NAMEmodule.c C implementation comes here.
│       _EXTENSION_NAME.pyi     Typing stub.
│       py.typed                Enable typing.
│   
│   test_EXTENSION_NAME.py      Tests come here.
│   
│   mkdocs.yml                  Optional: MkDocs configuration.
│   index.md                    Webpage.
│   mathjax.js                  MathJax for math.
```

### `pyproject.toml`

Filtered version of

[Python Packaging User Guide - Writing your pyproject.toml](https://packaging.python.org/en/latest/guides/writing-pyproject-toml/#a-full-example)

and more ordered like

[Python Packaging User Guide - pyproject.toml specification](https://packaging.python.org/en/latest/specifications/pyproject-toml/).

For extensions/setuptools used

[setuptools documentation - Configuring setuptools using pyproject.toml files](https://setuptools.pypa.io/en/latest/userguide/pyproject_config.html).

License specification acc. to [PEP 639](https://packaging.python.org/en/latest/guides/writing-pyproject-toml/#license-and-license-files).

### `mkdocs.yml`

Filtered version of

[squidfunk/mkdocs-material - mkdocs.yml](https://github.com/squidfunk/mkdocs-material/blob/master/mkdocs.yml).

Automatically enabled features:

- auto/bright/dark mode
- mkdocstrings preconfigured
- math, code highlighting, tasklists

### `LICENSE`

[Choose a License - MIT License](https://choosealicense.com/licenses/mit/)

### `.gitignore`

[github/gitignore - Python.gitignore](https://github.com/github/gitignore/blob/main/Python.gitignore)

## Roadmap

- [x] Deploy
- [x] References
- [x] Update extension C source
- [ ] Switch from [MkDocs](https://www.mkdocs.org/) to [Zensical](https://zensical.org/) because of [The Slow Collapse of MkDocs](https://fpgmaas.com/blog/collapse-of-mkdocs/).
- [ ] Web interface
- [x] Ballin

## License (MIT)

Copyright (c) 2025-2026 Sebastian Gössl

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
