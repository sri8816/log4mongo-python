log4mongo-python
================
log4mongo-python is mongo database handler for python logging, part of log4mongo.org project.
log4mongo-python is using pymongo driver - http://github.com/mongodb/mongo-python-driver


Requirements
------------

- python 2.7+
- pymongo
- MongoDB

For more information see *debian_requirements.txt* and *requirements.txt* files.

Configuration
-------------

Example handler python configuration: ::

 import logging
 from log4mongo.handlers import MongoHandler

 logger = logging.getLogger('test')
 logger.addHandler(MongoHandler(host='localhost'))
 logger.warning('test')


Tests
-----

**Tested on evnironment**

- Xubuntu Linux 11.10 oneiric 64-bit
- python 2.7.1+
- python unittest

**Running tests**

To run the test run command: ::

 $ python test.py
 $ python setup.py test


Author
------

| char0n (Vladimír Gorej, CodeScale s.r.o.) 
| email: gorej@codescale.net
| web: http://www.codescale.net

References
----------
- http://www.mongodb.org/
- http://docs.python.org/library/logging.html
- http://github.com/mongodb/mongo-python-driver
- http://log4mongo.org