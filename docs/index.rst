Welcome to ``PyJWT``
===========================

``PyJWT`` is a Python library which allows you to encode and decode JSON Web
Tokens (JWT). JWT is an open, industry-standard (`RFC 7519`_) for representing
claims securely between two parties.

Installation
------------
You can install ``pyjwt`` with ``pip``:

.. code-block:: console

    $ pip install pyjwt

See :doc:`Installation <installation>` for more information.

Example Usage
------------

.. code-block:: python

    >>> import jwt

    >>> jwt.encode({'some': 'payload'}, 'secret', algorithm='HS256')
    'eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJzb21lIjoicGF5bG9hZCJ9.4twFt5NiznN84AWoo1d7KO1T_yoc0Z6XOpOVswacPZg'

    >>> jwt.decode('eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJzb21lIjoicGF5bG9hZCJ9.4twFt5NiznN84AWoo1d7KO1T_yoc0Z6XOpOVswacPZg', 'secret')
    {'some': 'payload'}


See :doc:`Usage Examples <usage>` for more examples.

.. toctree::
    :maxdepth: 2

    installation
    usage
    faq
    algorithms
    api

.. _`RFC 7519`: https://tools.ietf.org/html/rfc7519
