Begin The Symfony
========================

Symfony app with login and user management features.

Requirements
------------

  * PHP 7.1.3 or higher;
  * and the [usual Symfony application requirements][2].

Installation
------------

Configure DB connention in `.env` file

```bash
$ DATABASE_URL=mysql://user_name:password@127.0.0.1:3306/db_name?serverVersion=10.1.37-MariaDB
```

Install dependencies

```bash
$ composer update
```

Run migrations

```bash
$ php bin/console doctrine:migrations:migrate
```

Usage
-----

There's no need to configure anything to run the application. If you have
[installed Symfony][4], run this command and access the application in your
browser at the given URL (<https://localhost:8000> by default):

```bash
$ cd my_project/
$ symfony serve
```

If you don't have the Symfony binary installed, run `php -S localhost:8000 -t public/`
to use the built-in PHP web server or [configure a web server][3] like Nginx or
Apache to run the application.
