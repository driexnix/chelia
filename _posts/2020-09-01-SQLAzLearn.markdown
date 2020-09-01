---
layout: post
title:  SQL Az Learning
date:   2020-09-01 10:10:00 +0300
image:  02.jpg
---
### SQL

# SQL Query all usernames in DB


<pre><code>
select name as username,
       create_date,
       modify_date,
       type_desc as type,
       authentication_type_desc as authentication_type
from sys.database_principals
where type not in ('A', 'G', 'R', 'X')
      and sid is not null
      and name != 'guest'
order by username;
</code></pre>


# Login
Als je inlogt met SQL Admin, heb je geen mogelijkheid tot het toevoegen van Azure AD members.

# Toevoegen van AZ Users

<pre><code>
CREATE USER [username@company.com] FROM EXTERNAL PROVIDER;
CREATE USER [username@company.com] FROM EXTERNAL PROVIDER;
CREATE USER [username@company.com] FROM EXTERNAL PROVIDER;
</code></pre>


# Toevoegen van Groups

> Create USER [SQLAzDev] FROM EXTERNAL PROVIDER;
If you get an issue, check token - reconnect and check you are in the correct db.

# Toevoegen van rechten

> ALTER ROLE db_datawriter ADD MEMBER [username.comp]
