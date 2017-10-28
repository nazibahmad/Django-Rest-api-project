# Django-Rest-api-project

#Setting up a new environment

virtualenv env
source env/bin/activate
----------------------------------------------
#install package requirements.

pip install django
pip install djangorestframework
pip install pygments  # i'll be using this for the code highlighting

------------------------------------------------------------------------------
#i'll need to add our new snippets app and the rest_framework app to INSTALLED_APPS. Let's edit the tutorial/settings.py file:

INSTALLED_APPS = (
    ...
    'rest_framework',
    'snippets.apps.SnippetsConfig',
)

---------------------------------------------------

#start up Django's development server.
python manage.py runserver

--------------------------------------------------

#In another terminal window, we can test the server.

#We can test our API using curl or httpie. Httpie is a user friendly http client that's written in Python. Let's install that.

#You can install httpie using pip:


pip install httpie

