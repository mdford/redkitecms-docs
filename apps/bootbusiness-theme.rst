Add the Bootbusiness Theme-Block to RedKite CMS
===============================================

A great theme design for a professional website. This is the default theme that comes with a Standard RedKite CMS installation.

Installation
------------

You can add the **Bootbusiness Theme-Block** to the application managed by RedKite 
CMS, adding it to the **composer.json** of your Symfony2 application:

.. code-block:: text

    {
        [...]
		
        "require": {
            [...]        
            "redkite-labs/bootbusiness-theme-bundle": "dev-master",        
        }
    }

Be sure that there is declared the reference to **http://apps.redkite-labs.com** repository,
under the **repositories** option:

.. code-block:: text

    "repositories": [

        [...]

        {
            "type": "composer",
            "url": "http://apps.redkite-labs.com"
        }
    ],

then run the composer's update command:

.. code-block:: text

    php composer.phar update redkite-labs/sunshine-theme-bundle

To have the new block available, don't forget to clear the cache for the **rkcms environment**
as follows:

.. code-block:: text

    app/console cache:clear --env=rkcms

Theme preview
-------------

To preview the theme, click the **Themes** button on the toolbar, then the **Preview**
button.

.. class:: fork-and-edit

Found a typo ? Something is wrong in this documentation ? `Just fork and edit it !`_

.. _`Just fork and edit it !`: https://github.com/redkite-labs/redkite-docs