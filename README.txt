This is the development buildout for the dexterity project.

Dexterity development on Plone 3:
---------------------------------

To build a Plone 3 environment, use the plone3.cfg configuration like so:

   bin/buildout -c plone3.cfg


Dexterity development on Plone 4:
---------------------------------

To build a Plone 4 environment, use the plone4.cfg configuration like so:

   bin/buildout -c plone4.cfg

Building PIL within your environment:
-------------------------------------

If you need PIL, you can use the pil.cfg file and include it like so:

   1. Create a new configuration file, such as local.cfg

   2. Add the following lines (to use Plone 4, change the plone3.cfg to plone4.cfg):

      [buildout]
      extends = plone3.cfg pil.cfg

   3. Run buildout like so:

      bin/buildout -c local.cfg


Building lxml within your environment:
-------------------------------------

If you need lxml, you can use the lxml.cfg file and include it like so:

   1. Create a new configuration file (or edit an existing one), such as local.cfg

   2. Add the following lines (to use Plone 4, change the plone3.cfg to plone4.cfg):

      [buildout]
      extends = plone3.cfg lxml.cfg

   3. Run buildout like so:

      bin/buildout -c local.cfg



