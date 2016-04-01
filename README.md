# lib_mysqludf_sys
The fix for the historical bug #2 (http://bugs.mysql.com/bug.php?id=2) is here.
Based on the UDF library with functions to interact with the operating system. These functions allow you to interact with the execution environment in which MySQL runs.
I've added make_toast function and make_toast python script
See here for more details: https://www.percona.com/blog/2016/04/01/fixing-mysql-bug2-now-mysql-makes-toast/

* Install PiFace software and Python bindings
* Test the make_toast python script
* Add user “mysql” to the spi and gpio groups so it can manipulate pins:

gpasswd -a mysql gpio; gpasswd -a mysql spi

* Download the make toast UDF code and run install.sh.
