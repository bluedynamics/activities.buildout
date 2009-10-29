activities.buildout
===================

Meta Package for installation of all necessary packages for the
Activity Model Runtime Engine for Python (AMREP).


Python 2.6
==========
AMREP was developed for Python 2.6. Currently, on many computers Python 2.5 is
installed. There is a buildout in dev/py2.6 which can be used to install Python
2.6 side by side with other Python versions.

How to install
==============
It's assumed that py26 links to the Python 2.6 interpreter. Bootstrap buildout
like so:
$ py26 bootstrap.py

Run buildout with the standard buildout configuration file:
$ ./bin/buildout

After a while AMREP and it's dependencies should be installed.

How to run tests
================
Test for activities.runtime:
$ ./bin/test -s activities.runtime -t runtime.txt

Test for activities.metamodel:
$ ./bin/test -s activities.metamodel -t elements.txt

Test for activities.transform.xmi:
$ ./bin/test -s activities.transform.xmi -t transform.txt

Test for activities.test.hospital:
$ ./bin/test -s activities.test.hospital -t tests.txt

Test for activities.test.article:
$ ./bin/test -s activities.test.article -t tests.txt


Author and Copyright
====================
Johannes Raggam <johannes@raggam.co.at>,
BlueDynamics Alliance - http://bluedynamics.com

License
=======
See License.txt
