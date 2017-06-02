openwisp-network-topology
=========================

.. image:: https://travis-ci.org/openwisp/openwisp-network-topology.svg?branch=master
    :target: https://travis-ci.org/openwisp/openwisp-network-topology

.. image:: https://coveralls.io/repos/github/openwisp/openwisp-network-topology/badge.svg
    :target: https://coveralls.io/github/openwisp/openwisp-network-topology

.. image:: https://requires.io/github/openwisp/openwisp-network-topology/requirements.svg?branch=master
    :target: https://requires.io/github/openwisp/openwisp-network-topology/requirements/?branch=master
    :alt: Requirements Status

.. image:: https://badge.fury.io/py/openwisp-network-topology.svg
    :target: http://badge.fury.io/py/openwisp-network-topology

------------

TODO:

------------

.. contents:: **Table of Contents**:
   :backlinks: none
   :depth: 3

------------

Current features
----------------

* TODO

Project goals
-------------

* TODO

Install stable version from pypi
--------------------------------

Install from pypi:

.. code-block:: shell

    pip install openwisp-network-topology

Install development version
---------------------------

Install tarball:

.. code-block:: shell

    pip install https://github.com/openwisp/openwisp-network-topology/tarball/master

Alternatively you can install via pip using git:

.. code-block:: shell

    pip install -e git+git://github.com/openwisp/openwisp-network-topology#egg=openwisp-network-topology

If you want to contribute, install your cloned fork:

.. code-block:: shell

    git clone git@github.com:<your_fork>/openwisp-network-topology.git
    cd openwisp-network-topology
    python setup.py develop

Setup (integrate in an existing django project)
-----------------------------------------------

Add ``openwisp_network_topology`` to ``INSTALLED_APPS``:

.. code-block:: python

    INSTALLED_APPS = [
        # other apps
        'openwisp_network_topology',
    ]

Add the URLs to your main ``urls.py``:

.. code-block:: python

    urlpatterns = [
        # ... other urls in your project ...

        # openwisp-network-topology urls
        # keep the namespace argument unchanged
        url(r'^', include('openwisp_network_topology.urls', namespace='network_topology')),
    ]

Then run:

.. code-block:: shell

    ./manage.py migrate

Installing for development
--------------------------

Install sqlite:

.. code-block:: shell

    sudo apt-get install sqlite3 libsqlite3-dev

Install your forked repo:

.. code-block:: shell

    git clone git://github.com/<your_fork>/openwisp-network-topology
    cd openwisp-network-topology/
    python setup.py develop

Install test requirements:

.. code-block:: shell

    pip install -r requirements-test.txt

Create database:

.. code-block:: shell

    cd tests/
    ./manage.py migrate
    ./manage.py createsuperuser

Launch development server:

.. code-block:: shell

    ./manage.py runserver

You can access the admin interface at http://127.0.0.1:8000/admin/.

Run tests with:

.. code-block:: shell

    ./runtests.py

Settings
--------

TODO

Contributing
------------

1. Announce your intentions in the `OpenWISP Mailing List <https://groups.google.com/d/forum/openwisp>`_
2. Fork this repo and install it
3. Follow `PEP8, Style Guide for Python Code`_
4. Write code
5. Write tests for your code
6. Ensure all tests pass
7. Ensure test coverage does not decrease
8. Document your changes
9. Send pull request

.. _PEP8, Style Guide for Python Code: http://www.python.org/dev/peps/pep-0008/

Changelog
---------

See `CHANGES <https://github.com/openwisp/openwisp-network-topology/blob/master/CHANGES.rst>`_.

License
-------

See `LICENSE <https://github.com/openwisp/openwisp-network-topology/blob/master/LICENSE>`_.

Support
-------

See `OpenWISP Support Channels <http://openwisp.org/support.html>`_.