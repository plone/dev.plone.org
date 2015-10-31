======================================
Sphinx Themes for Plone Documentation
======================================

sphinx.themes.plone is a collection of `Sphinx`_ themes for the `Plone`_ documentation project.

The different themes are used on `docs.plone.org`_, but are not limited for this purpose.
It might be used for all Plone Package Documentations, or even private usecase but than without the Plone Logo and Footer (respect the License).


Features
--------

- sphinx.themes.plone comes with own themes for 

  * Plone Classic (Plone 2.0-3.3 Design)
  * Plone Sunburst (Plone 4 Design)
  * Plone Barceloneta (Plone 5 Design)
  * Plone Org 4 (Generation of Plone 4)
  * Plone Org 5 (Generation of Plone 5)

Installation
------------

Install sphinx.themes.plone with buildout::

    [buildout]
    parts=
        sphinx

    [sphinx]
    recipe=zc.recipe.egg
    eggs=
        Sphinx
        sphinx.themes.plone

.. CAUTION::
    *You should never use a checkout of the theme package for just appling a theme to your documentations.*
    Never touch this package to adjust configuration or customize parts, there is no need for that. Read the documentation please: http://docs.plone.org/...

Configuration
-------------

Edit the "conf.py" configuration file to point to the plone themes::

    # At the top.
    import sphinx.themes.plone

    # ...

    # Activate the theme path:
    html_theme_path = sphinx.themes.plone.get_html_theme_path()

    # Activate the theme like this:
    html_theme = 'plone_org_4'

Additional switches for the theme, see detailed documentation.

Available Themes
----------------

- plone_classic
- plone_sunburst
- plone_barceloneta (TODO: to be implemented)
- plone_org_4
- plone_org_5 (TODO: to be finalized)

Contribute
----------

- Issue Tracker: https://github.com/plone/sphinx.themes.plone/issues
- Source Code: https://github.com/plone/sphinx.themes.plone

.. _licence:

License
-------

* The technical parts of this project is licensed under the GPLv2 license.
* The text and illustrations in this package / generated pages are licensed by the Plone Foundation under a Creative Commons Attribution 4.0 International license.
* Plone and the Plone :sup:`®` logo are registered trademarks of the Plone Foundation, registered in the United States and other countries.
* For guidelines on the permitted uses of the Plone trademarks, see https://plone.org/foundation/logo
* All other trademarks are owned by their respective owners.

.. _Sphinx: http://sphinx-doc.org/
.. _Plone: http://plone.org
.. _docs.plone.org: http://docs.plone.org
