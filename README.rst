Email Client
============

A simple python interface for the email service.

Installation
------------

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
