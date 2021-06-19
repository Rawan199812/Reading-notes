## A Beginner's Guide to Docker

- With Docker We can faithfully reproduce a production environment locally. 
- Docker can be shared among team members so everyone is working on the same setup. 
-  We can run a production database with Docker

***How is `Docker is Linux containers ` ?***

**Linux containers which are a type of virtualization. And Virtualization has its roots at the beginning of computer science when large, expensive mainframe computers were the norm.**


***Install Docker***
1. download the desktop app on our computer and create a free account.
2. `docker --version`
Docker version 19.03.5, build 633a0ea
3. `docker-compose --version`
docker-compose version 1.24.1, build 4667896b
4. `docker run hello-world` (To confirm Docker installed correctly)

**To create custom images :**

- A Dockerfile is the recipe for a cake
- An image is a snapshot of the recipe at a given time
- A docker-compose.yml says how to make the cake
- And the container is the actual, baked cake


- Dockerfile is a list of instructions for creating an image
- Images are made up of one or more layers
- Containers are a running instance of an image
- docker-compose.yml controls how to run the container
- Containers are stateless and ephemeral in nature. We can link the local filesystem via volumes but things become - more complex with databases (which we didn’t cover here).


## Django for APIs

**First we need a dedicated directory on our computer to store the code. (The location really does not matter; it just needs to be easily accessible.)**
`cd ~/Desktop`
`mkdir code && cd code`

**To create a dedicated directory for our library site, install Django via Pipenv, and then enter the virtual environment using the shell command.** 
`mkdir library && cd library`
`pipenv install django~=3.1.0`
`pipenv shell`

**To create a new project**
`(library) $ django-admin startproject config .`


### Django REST Framework

**Make sure to quit the local server Control + c if it is still running.**
`(library) $ pipenv install djangorestframework~=3.11.0`

**Add it to the INSTALLED_APPS config in our settings.py file. AS A Thisd party**
# config/settings.py
INSTALLED_APPS = [
    'django.contrib.admin',
    'django.contrib.auth',
    'django.contrib.contenttypes',
    'django.contrib.sessions',
    'django.contrib.messages',
    'django.contrib.staticfiles',

    # 3rd party
    'rest_framework', # new

    # Local
    'books',
]

**To create a new api app.**
`(library) $ python manage.py startapp api`

**Inside the config/settings.py**
INSTALLED_APPS = [
    'django.contrib.admin',
    'django.contrib.auth',
    'django.contrib.contenttypes',
    'django.contrib.sessions',
    'django.contrib.messages',
    'django.contrib.staticfiles',

    # 3rd party
    'rest_framework',

    # Local
    'books',
    'api', # new
]

**Make a serializers.py file within our api app.**
`(library) $ touch api/serializers.py`