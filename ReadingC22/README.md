## Django Custum User Model

create a custom User model in Django so that an email address or phone  can be used as the primary user identifier instead of a username for authentication.

### AbstractUser vs AbstractBaseUser
The default User model in Django uses a username to uniquely identify a user during authentication. If you'd rather use an email address, you'll need to create a custom User model by either subclassing AbstractUser or AbstractBaseUser.

Options:

- AbstractUser: Use this option if you are happy with the existing fields on the User model and just want to remove the username field.

- AbstractBaseUser: Use this option if you want to start from scratch by creating your own, completely new User model.

The steps are the same for each:

Step 1: Set up a Django project.

Step 2: Create a custom User model and Manager


Manager is a class that provides an interface through which database query operations are provided to Django models. You can have more than one manager for your model.

Step 3: The Settings

We now have to tell Django our new model that should be used to represent a User

Step 4: Customize the UserCreationForm and UserChangeForm forms

Django’s built-in UserCreationForm and UserChangeForm forms must be extended to let them know the new user model that we are working with.

Step 5: Update the admin

Tell the admin panel to use these forms by extending from UserAdmin

**Note**:

This [site](https://learndjango.com/tutorials/django-custom-user-model) explains step-by-step how to create a custom User model in Django.



