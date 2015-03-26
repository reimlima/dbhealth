dbhealth
--------------------------------------------------------------------------------

Check table consistence for MySQL and try to fix existing errors

Notice
--------------------------------------------------------------------------------

This script was tested and work well in:

* Linux
        - OS Distribution: CentOS release 6.6 (Final)
        - Kernel: 2.6.32-504.3.3.el6.x86_64
        - GNU bash: version 4.1.2(1)-release (x86_64-redhat-linux-gnu)

Changelog
--------------------------------------------------------------------------------

2015-03-16      - v1    - First Stable Release

How to use it
--------------------------------------------------------------------------------

CONF FILE:

Just  fill  the  configuration  file  with  the  values  for DBUSER, DBPASSWORD,
DBARRAY, TMPFILEPATH, DBHEALTHLOG, then run the script.

Legend:

	DBUSER:		MySQL Access Login
        
	DBPASSWORD:     MySQL Access Password
        
	DBARRAY:	Databases to Check
			fill it in format like => "db1 db2 dbN"
                                        
	TMPFILEPATH:	Internal temporary file used by script
        
	DBDUMPLOG:	Log File

Example:

	DBUSER="root"
	DBPASSWORD="pass1234"
	DBARRAY="zabbix nagios cacti"
	TMPFILEPATH="/tmp"
	DBHEALTHLOG="dbhealth.log"
