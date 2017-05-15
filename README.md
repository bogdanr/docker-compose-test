The purpose of this example is to demonstrate docker-compose for running an application that uses two containers:

#### web container:

* build on top of ubuntu:16.04
* separate volume for web files
* expose port 80

#### database container:

* mysql on the ubuntu:16.04 image
* separate volume for database files
* expose port 3306 (discuss about this one)
