# aiozyre
asyncio-friendly Python bindings for [Zyre](https://github.com/zeromq/zyre), an open-source framework for proximity-based peer-to-peer applications.

![build_status](https://travis-ci.org/elijahr/aiozyre.svg?branch=master)

## Installation

```shell
pip install aiozyre
```

Tests run on both Linux and macOS for the following Python versions:
* CPython: 3.6.4, 3.7.0, 3.8.0
* PyPy: 7.2.0 (3.6.9)

CPython 3.6.3 and lower are not supported due to [this bug](https://bugs.python.org/issue20891).

## Usage

See the [example peer-to-peer chat client](https://github.com/elijahr/aiozyre/blob/master/examples/chatter.py).

## Contributing

Pull requests are welcome, please file any issues you encounter.

## Changelog

### v1.1.6 (2024-09-23)

* Support for Python 3.12

### v1.1.5 (2020-07-22)

* Fix memory leak where zlist items were not being freed
* Fix egg installation issue by passing zip_safe=False

### v1.1.4 (2020-05-23)

* Handle `SILENT` message