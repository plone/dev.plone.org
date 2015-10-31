About
=====

This is a static landing page, based on `Sphinx <http://sphinx-doc.org/>`_, running on https://dev.plone.org.

Updating
--------

For updating the content, please change into the *source* directory and edit the file you wish to change

Example of updating the index.html

.. code-block:: bash

    $ cd source
    $ vim index.rst

When you are finished, please change back to the root  directory and create the html

.. code-block:: bash

    $ cd ..
    $ make html
