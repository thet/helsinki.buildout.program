howto install
=============

debian dependencies
-------------------
$ apt-get install libmysqlclient-dev mysql-server


* checkout the repository

  readwrite: $ git@github.com:thet/helsinki.buildout.program.git

  readonly: $ git://github.com/thet/helsinki.buildout.program.git


* checkout the submodules
    $ git submodule init

    $ git submodule update


* install the application
    $ python-2.6 bootrap.py -d -c base.cfg

    $ ./bin/buildout -c base.cfg

* create the db
    $ ./bin/django syncdb


* import the data fixtures
    $ ./bin/django loaddata musicfocus
    $ ./bin/django loaddata broadcastformats
    $ ./bin/django loaddata rrules
    $ ./bin/django loaddata showinformation
    $ ./bin/django loaddata showtopics


* run the server
    $ ./bin/django runserver 
