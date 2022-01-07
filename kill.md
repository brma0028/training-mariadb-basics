# Kill Session/User 

```
MariaDB [(none)]> show processlist;
+----+-------------+-----------+------+---------+------+--------------------------+--------------------+----------+
| Id | User        | Host      | db   | Command | Time | State                    | Info               | Progress |
+----+-------------+-----------+------+---------+------+--------------------------+--------------------+----------
| 37 | root        | localhost | NULL | Query   |    0 | Init                     | show processlist   |    0.000 |
| 38 | root        | localhost | NULL | Query   |   10 | User sleep               | select sleep(1000) |    0.000 |
 
 # kill thread 38. Connection will be interrupted. User session will be cancelled 
 kill 38


```
