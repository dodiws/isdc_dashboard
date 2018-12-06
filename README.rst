=========
dashboard
=========

Display base mapping data.
Mandatory Module for ISDC

Quick start
-----------

1. Add "dashboard" to your ISDC_BASE_APPS setting like this::

   ISDC_BASE_APPS = [
       ...
       'dashboard',
   ]

   For development in virtualenv add GEODB_PROJECT_DIR path to VENV_NAME/bin/activate:
       export PYTHONPATH=${PYTHONPATH}:\
       ${HOME}/GEODB_PROJECT_DIR

2. To create the flood tables:

   python manage.py makemigrations
   python manage.py migrate dashboard --database geodb
