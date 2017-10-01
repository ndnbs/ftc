Home of any H2 DBs used

#####
# Can use the H2 "Shell" like this.
#####
C:\data\git-work\ftc>java -cp build\libs\ftc-all.jar org.h2.tools.Shell  

            OR like this

C:\data\git-work\ftc>java -cp build\libs\ftc-all.jar org.h2.tools.Shell \
-url "jdbc:h2:tcp://192.168.14.184:9092/C:/data/git-work/ftdb/support/db/ftdb" \
-user sa -password ""

NOTE: A remote connection may look something like this:

   jdbc:h2:tcp://192.168.14.184:9092/C:/data/git-work/ftdb/support/db/ftdb
	
Welcome to H2 Shell 1.4.196 (2017-06-10)
Exit with Ctrl+C
[Enter]   jdbc:h2:./support/db/ftdb
URL
[Enter]   org.h2.Driver
Driver
[Enter]   sa
User
[Enter]   Hide
Password
Password
Connected
Commands are case insensitive; SQL statements end with ';'
help or ?      Display this help
list           Toggle result list / stack trace mode
maxwidth       Set maximum column width (default is 100)
autocommit     Enable or disable autocommit
history        Show the last 20 statements
quit or exit   Close the connection and exit

sql> show columns from os;
FIELD      | TYPE          | NULL | KEY | DEFAULT
ID         | INTEGER(10)   | NO   | PRI | NULL
........
(20 rows, 88 ms)
sql>


