howto install
=============

run
$ python-2.6 bootrap.py -d -c base.cfg
$ ./bin/django syncdb
$ ./bin/django loaddata musicfocus
$ ./bin/django loaddata broadcastformats
$ ./bin/django loaddata rrules
$ ./bin/django loaddata showinformation
$ ./bin/django loaddata showtopics

$ ./bin/django runserver 
