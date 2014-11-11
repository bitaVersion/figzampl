Django + PostgreSQL + Fig = Example
============================

This project is a simple example of a [Fig](http://orchardup.github.io/fig/)
project setup. It uses Django and PostgreSQL.

Running Requirements
====================

* [Fig](http://orchardup.github.io/fig/)
* [Docker](http://docs.docker.io/en/latest/installation/ubuntulinux/)

These two requirements must be setup and are outside the scope of this readme. The links above are a good starting place.

Start Fig
=========

```bash
$ fig up -d
$ fig run web python manage.py syncdb --noinput
```

Now browse to [http://localhost:8000](http://localhost:8000)

The Django server was started in auto-reload mode and fig shares the
current folder with the docker instance, so you can edit the python code
to see changes!
