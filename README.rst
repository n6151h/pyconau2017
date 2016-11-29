pyconau2017/website
===============

This is a fork of the lca2017 site website.
Original here:  https://github.com/lca2017/website

At the present time, /home/nicks/anaconda/lib/python2.7/site-packages/appconf/utils.py
must be modified to look like this.  (Version hell problem.)

    from django.utils.module_loading import import_module

before you can launch.


Launchifying
------------

- create a virtualenv with python 2.7
- activate the virtualenv
- cd into the ``website`` directory
- ``pip install -r requirements.txt``
- ``python manage.py migrate``
- ``python manage.py loaddata ./fixtures/*``
- ``python manage.py runserver [YOUR PORT]``
