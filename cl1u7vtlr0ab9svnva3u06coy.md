## Django PostgreSQL Migration from SQLite

Full Article on [Sweetcode](https://sweetcode.io/django-postgresql-migration-from-sqlite/)

PostgreSQL is a powerful, open-source object-relational database system that uses and extends the SQL language combined with many other features that safely store complicated data workloads.

The database comes with many features that not only help developers build applications but also help administrators protect data no matter how big or small the dataset is.

As developers, we often work on different projects depending on our level of expertise. As a beginner, you worked on an app like a ‘to-do app’ which didn’t require a heavy database mechanism to store records of tasks. But as you advance, the kind of projects you handle change with time. A point will reach where you will need to build a production-ready project which will need a database structure.

Usually, a basic Django project will ship with an SQLite database as the default. Even though this is the default database, Django also supports other databases like:

* PostgreSQL
* MySQL
* Oracle 

In this article, we will focus on PostgreSQL and how we can implement it on Django projects.

## Why use PostgreSQL 
PostgreSQL comes with many features that not only help developers build applications but also help administrators protect data no matter how big or small the dataset is.

So, why should you consider PostgreSQL over the others:

* It is free to use and it’s also an open-source program which makes it easy to upgrade or extend.
* PostgreSQL is highly extensible – for example, you can define your own data types, build your own functions and even write code from different programming languages without having to recompile your database.
* It supports many SQL features.
* It also supports multiple programming languages like Python, Java, C/C++, Ruby, etc…
* Works on most popular Operating Systems.
* It is not controlled by any cooperation meaning it is free.

Let’s get started and see how to implement PostgreSQL.

## Setting up Django project 

Now, for us to be able to make a database migration it means we need a project to work with. Let’s go ahead and create a new Django project.

As always the first step is to create a virtual environment, which is accomplished in two steps:

`pip install virtualenvwrapper-win`

This installs virtual an environment, so the next step is to name the virtualenv:

`mkvirtualenv [name]`

Naming it automatically activates the virtual environment.

Now, since we are working on a Django project, installing it is essential. It will be installed in the virtual environment

`pip install django`

Next, we have to create our Django project, in this case, it can be named testproject.

`django-admin startproject testproject`

Then, we create an app within our project folder.

`python manage.py startapp projectApp`

Finally, we can run the project so as to initialize the SQLite database with this command.

`python manage.py runserver`

We will be using this simple Django application to perform the migration in the following steps.

### Step 1: Backup existing Database

In the first step, we will need to create a backup of our current data which we are going to export into PostgreSQL later on.

To perform a data backup, we use the following command:

`python manage.py dumpdata > data.json`

This command will generate a data.json file in the root of your project, meaning you generated the dumpdata from SQLite and stored it in JSON format.

### Step 2: Installing PostgreSQL

<------------->

Read the rest of the article on [Sweetcode](https://sweetcode.io/django-postgresql-migration-from-sqlite/)

I appreciate your time reading.

Your support will be really appreciated

<a href="https://www.buymeacoffee.com/lary" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/default-orange.png" alt="Buy Me A Coffee" height="41" width="174"></a>

Connect With me at [Twitter](https://twitter.com/larymak1) | [GitHub](https://github.com/larymak) | [YouTube](https://www.youtube.com/channel/UCrT1ARRZfLOuf6nc_97eXEg) | [LinkedIn](https://www.linkedin.com/in/hillary-nyakundi)  | 