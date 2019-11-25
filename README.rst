[![FOSSA Status](https://app.fossa.io/api/projects/git%2Bgithub.com%2Faffoio%2Faffo-email-client.svg?type=shield)](https://app.fossa.io/projects/git%2Bgithub.com%2Faffoio%2Faffo-email-client?ref=badge_shield)

|Build Status| |Code Style|

AFFO Email Client
=================

A simple python interface for the email service.

Installation
------------

============ =============================================
**Version**  1.0.0
**Web**      https://affo.io/
**Download** https://pypi.org/affoio/affo-email-client/
**Source**   https://github.com/affoio/affo-email-client/
**Keywords** python, email, service, client
============ =============================================

::

   pip install python-email-client

Usage
-----

The example below shows how you get an inform

.. code:: python

   import affo_email_client

   client = affo_email_client.Client(api_root_url="https://localhost/api/v1.0/")
   client.message.create(body={
       "from_": "from@example.com",
       "to": ["to@example.com"],
       "subject": "Hello",
       "html": "",
       "text": "",
       "tag": "test"
   })

.. |Build Status| image:: https://travis-ci.org/affoio/affo-email-client.svg?branch=master
   :target: https://travis-ci.org/affoio/affo-email-client
.. |Code Style| image:: https://img.shields.io/badge/code%20style-black-000000.svg
   :target: https://github.com/psf/black


## License
[![FOSSA Status](https://app.fossa.io/api/projects/git%2Bgithub.com%2Faffoio%2Faffo-email-client.svg?type=large)](https://app.fossa.io/projects/git%2Bgithub.com%2Faffoio%2Faffo-email-client?ref=badge_large)