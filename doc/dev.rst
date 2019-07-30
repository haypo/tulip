Run tests
=========

Run tests with tox
------------------

The `tox project <https://testrun.org/tox/latest/>`_ can be used to build a
virtual environment with all runtime and test dependencies and run tests
against different Python versions (2.6, 2.7, 3.2, 3.3).

For example, to run tests with Python 2.7, just type::

    tox -e py27

To run tests against other Python versions:

* ``py26``: Python 2.6
* ``py27``: Python 2.7
* ``py32``: Python 3.2
* ``py33``: Python 3.3


Test Dependencies
-----------------

On Python older than 3.3, unit tests require the `mock
<https://pypi.python.org/pypi/mock>`_ module. Python 2.6 requires also
`unittest2 <https://pypi.python.org/pypi/unittest2>`_.

To run ``run_aiotest.py``, you need the `aiotest
<https://pypi.python.org/pypi/aiotest>`_ test suite: ``pip install aiotest``.


Run tests on UNIX
-----------------

Run the following commands from the directory of the Trollius project.

To run tests::

    make test

To run coverage (``coverage`` package is required)::

    make coverage


Run tests on Windows
--------------------

Run the following commands from the directory of the Trollius project.

You can run the tests as follows::

    C:\Python27\python.exe runtests.py

And coverage as follows::

    C:\Python27\python.exe runtests.py --coverage

