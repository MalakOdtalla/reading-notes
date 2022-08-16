## Django settings

A Django settings file contains all the configuration of your Django installation. 

### Managing Django Settings: Issues
Different environments. Usually, you have several environments: local, dev, ci, qa, staging, production, etc. Each environment can have its own specific settings (for example: DEBUG = True, more verbose logging, additional apps, some mocked data, etc). You need an approach that allows you to keep all these Django setting configurations.

Sensitive data: You have SECRET_KEY in each Django project. On top of this there can be DB passwords and tokens for third-party APIs like Amazon or Twitter. This data cannot be stored in VCS.
Sharing settings between team members. You need a general approach to eliminate human error when working with the settings. For example, a developer may add a third-party app or some API integration and fail to add specific settings. On large (or even mid-size) projects, this can cause real issues.


Django settings are a Python code: It gives you a lot of flexibility, but can also be a problem – instead of key-value pairs, settings.py can have a very tricky logic.


### Setting Configuration: Different Approaches
There is no built-in universal way to configure Django settings without hardcoding them. But books, open-source and work projects provide a lot of recommendations and approaches on how to do it best.


More details about django settings [site](https://djangostars.com/blog/configuring-django-settings-best-practices/#header11)



## SSH

SSH, also known as Secure Shell or Secure Socket Shell, is a network protocol that gives users, particularly system administrators, a secure way to access a computer over an unsecured network.

SSH also refers to the suite of utilities that implement the SSH protocol. Secure Shell provides strong password authentication and public key authentication, as well as encrypted data communications between two computers connecting over an open network, such as the internet.

In addition to providing strong encryption, SSH is widely used by network administrators to manage systems and applications remotely, enabling them to log in to another computer over a network, execute commands and move files from one computer to another.

More details about SSH in this [site](https://www.hostinger.com/tutorials/ssh-tutorial-how-does-ssh-work#What_Is_SSH)
