# Reqboost

![banner](ext/banner.png)

[![PyPI version](https://img.shields.io/pypi/v/reqboost?style=flat-square&logo=pypi)](https://pypi.org/project/reqboost/) [![License](https://img.shields.io/github/license/Khushiyant/reqboost?style=flat-square&logo=open-source-initiative)]([./LICENSE](https://github.com/Khushiyant/reqboost/blob/main/LICENSE)) [![Issues](https://img.shields.io/github/issues/Khushiyant/reqboost?style=flat-square&logo=github)](https://github.com/Khushiyant/reqboost/issues)

Reqboost is a high-performance Python library developed primarily in C++ and built on libcurl. It is designed for developers who need a fast, efficient HTTP client with minimal overhead and extensive control.

# Prerequisites

Make sure you have `libcurl`, `poco` ( and `pkg-config` in case of UNIX-systems) install on your system

## Linux

### Ubuntu/Debian-based Systems

```bash
sudo apt-get update
sudo apt-get install libcurl4-openssl-dev
sudo apt-get install libpoco-dev
sudo apt-get install pkg-config
sudo apt-get install nlohmann-json3-dev
```

### Fedora-based Systems

```bash
sudo dnf update
sudo dnf install libcurl-devel
sudo dnf install poco-devel
sudo dnf install pkg-config
sudo dnf install nlohmann-json3-dev
```

## MacOS

```bash
brew install curl
brew install poco
brew install pkgconfig
brew install nlohmann-json
```

## Windows

Download the latest Windows binary from the [libcurl website](https://curl.se/download.html) and following environment variables.

```bash
setx CURL_INCLUDE_DIR "C:\path\to\curl\include"
setx CURL_LIB_DIR "C:\path\to\curl\lib"
setx POCO_INCLUDE_DIR "C:\path\to\poco\include"
setx POCO_LIB_DIR "C:\path\to\poco\lib"

```

> Binaries can be downloaded for UNIX-based systems also

# Installation

* Clone the repo and install:

```bash
git clone https://github.com/Khushiyant/reqboost.git
cd reqboost
pip install .
```

> Above example will install in root, so try to use virtual environment for installation

* Use direct github installation

```bash
pip install git+https://github.com/Khushiyant/reqboost.git
```

# Contribution

Contributions are welcome! If you find a bug or have a feature request, please open an issue on the [Reqboost GitHub repository](https://github.com/Khushiyant/reqboost/issues).

## Troubleshooting Builds

In case, modified code builds are not reflected in final build due to caching of previous builds. Use the following commands:

```bash
python setup.py clean --all
python setup.py build_ext --inplace
```

# License

Reqboost is licensed under the Apache License, Version 2.0. See the [LICENSE](https://github.com/Khushiyant/reqboost/blob/main/LICENSE) file for more information.
