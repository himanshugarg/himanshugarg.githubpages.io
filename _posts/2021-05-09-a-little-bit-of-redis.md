Unlike RDBMS's, Redis is an in memory key-data-structure store, supporting strings, lists, hash-tables, sets, and sorted sets as values.

Commonly used operations include:-

STRING | LIST          | SET       | HASH    | ZSET
-------|---------------|-----------|---------|--------------
 GET   |               |           |         |
 SET   |               |           |         |
 DEL   |               |           |         |
       | LPUSH/RPUSH   | SADD      | HSET    | ZADD
       | LPOP/RPOP     | SMEMBERS  | HGET    | ZRANGE
       | LRANGE/RRANGE | SISMEMBER | HGETALL | ZRANGEBYSCORE
       | LINDEX/RINDEX | SREM      | HDEL    | ZREM
