Welcome to Flask-Shell2HTTP!
================================

.. image:: https://www.codefactor.io/repository/github/eshaan7/flask-shell2http/badge
.. image:: https://img.shields.io/lgtm/grade/python/g/Eshaan7/Flask-Shell2HTTP.svg?logo=lgtm&logoWidth=18
.. image:: https://img.shields.io/pypi/v/flask-shell2http

A minimalist Flask_ extension that serves as a RESTful/HTTP wrapper for python's subprocess API.

- **Convert any command-line tool into a REST API service.**
- Execute shell commands asynchronously and safely via flask's endpoints.
- Designed for binary to binary/HTTP communication, development, prototyping, remote control and more.

.. _Flask: https://github.com/pallets/flask

**Use Cases:**

- Set a script that runs on a succesful POST request to an endpoint of your choice.
- Map a base command to an endpoint and pass dynamic arguments to it.
- Can also process multiple uploaded files in one command.
- This is useful for internal docker-to-docker communications if you have different binaries distributed in micro-containers.
- You can define a callback function/ use signals to listen for process completion.
- Currently, all commands run asynchronously (default timeout is 3600 seconds), so result is not available directly. An option _may_ be provided for this in future release.

   `Note: This extension is primarily meant for executing long-running 
   shell commands/scripts (like nmap, code-analysis' tools) in background from an HTTP request and getting the result at a later time.`

Quickstart
-------------------------------
Get started at :doc:`Quickstart`. There are also
more detailed :doc:`Examples` that shows different use-cases for this package. 

.. toctree::
   :maxdepth: 2
   
   Quickstart
   Examples
   Logging

API Reference
-------------------------------
If you are looking for information on a specific function, class or
method, this part of the documentation is for you.

.. toctree::
   :maxdepth: 2
   
   api

Indices and tables
================================

* :ref:`genindex`
* :ref:`modindex`
* :ref:`search`
