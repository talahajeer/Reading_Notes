# Guide to Docker
 This is a beginner’s guide to Docker which is a way to isolate and run entire applications. With Docker it doesn’t matter if you are using a Mac, Windows, or Linux computer anymore. The entire development environment is isolated: programming language, software packages, databases, and more.

 With Docker we now longer have to mess around with virtual environments. We can faithfully reproduce a production environment locally. And Docker can be shared among team members so everyone is working on the same setup. Wins all around.

## Containers vs Virtual Environments
 If you are a Python programmer (like me) a common question at this point is, what about virtual environments? How do they differ from containers?

 Virtual environments are used to isolate Python software packages locally. We can create an isolated box for individual projects so one can use Python 2.7 and Django 1.5 while another can use Python 3.5 and Django 2.1 on the same computer. Virtual environments are great.

 But…virtual environments can only isolate Python packages. They still rely on a global, system-level installation of Python albeit they can refer to the proper version. So when we use Python 2.7 in a project, we’re pointing to an installation of Python 2.7 on the computer itself, not actually within the virtual environment.

 Also we can’t run a production database or other services within virtual environments so compared to Docker containers they are far more limited.

## Library Website and API
 Django REST Framework works alongside the Django web framework to create web APIs. We cannot build a web API with only Django Rest Framework; it always must be added to a project after Django itself has been installed and configured.

### Django REST Framework
 Django REST Framework is added just like any other third-party app. Make sure to quit the local server Control + c if it is still running. Then on the command line type the below.

 ```
 (library) $ pipenv install djangorestframework~=3.11.0
```
 Add it to the INSTALLED_APPS config in our settings.py file. I like to make a distinction between third-party apps and local apps as follows since the number of apps grows quickly in most projects. 