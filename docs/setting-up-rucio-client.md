---
id: setting-up-rucio-client
title: Setting Up the Rucio Client
sidebar_label: Setting Up the Rucio Client
---

## Prerequisites

Rucio clients run on Python 2.7, 3.6, 3.7 and 3.8 on any Unix-like
platform.

## Install via pip

When `pip` is available, the distribution can be downloaded from the
Rucio PyPI server and installed in one step:

```bash
pip install rucio-clients
```

This command will download the latest version of Rucio and install it to
your system. The dependencies are listed in the file
[`etc/pip-requires-client`](https://github.com/rucio/rucio/blob/master/etc/pip-requires-client)
and will be pulled in as necessary.

## Upgrade via pip

To upgrade via pip:

```bash
pip install --upgrade rucio-clients
```

## Install via pip and virtualenv

To install the Rucio clients in an isolated `virtualenv` environment:

```bash
wget --no-check-certificate https://raw.github.com/pypa/virtualenv/master/virtualenv.py
python virtualenv.py rucio
source rucio/bin/activate.csh
pip install rucio-clients
export RUCIO_HOME=`pwd`/rucio/
```


## Installing using setup.py

Otherwise, you can install from the distribution using the `setup.py`
script:

```bash
python setup.py install
```
