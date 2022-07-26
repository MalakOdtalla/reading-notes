## Reading Class 20

## Django Models

A Django model is the built-in feature that Django uses to create tables, their fields, and various constraints. In short, Django Models is the SQL of Database one uses with Django

- Each model is a Python class implemented as subclasses of django.db.models.Model, and can include fields, methods and metadata.

- Each attribute of the model represents a database field

## Using Django Models
To use Django Models, one needs to have a project and an app working in it. After you start an app you can create models in app/models.py

for more details about models and how to create it, see this [website](https://developer.mozilla.org/en-US/docs/Learn/Server-side/Django/Models)


## Django admin site
The Django admin application can use  models to automatically build a site area that  can be used to create, view, update, and delete records.

All the configuration required to include the admin application in the website was done automatically when  created the skeleton project. As a result, all we must do to add models to the admin application is to register them.