# Learn-Redis-Step-By-Step

https://www.udemy.com/learn-redis-step-by-step/

- **Start redis server** - .[REDIS_HOME]/srs/redis-server

- **Open redis command line** - .[REDIS_HOME]/srs/redis-cli

- Redis commands (executed through redis cli):
  - insert data: `SET name "kaustubh"`
  - get data: `GET name`
  - delete data: `DEL name`
  - increment value by 1: `INCR key_name`
  - decrement value by 1: `DECR key_name`
  - create list: 
    - `RPUSH key_name "value"` - inserts value to the end of the list
    - `LPUSH key_name "value"` - inserts value to the beginning of the list
  - delete value from the list:
    - `LPOP key_name` - deletes value at the beginning
    - `RPOP key_name` - deletes value the the end
  - get value from list: `LRANGE key_name 0 -1`
  - create set: `RSADD key_name "value"`
  - get values from set: `SMEMBERS key_name`
  - check (true/false) if set value exists: `SISMEMBERS key_name "value"`
  - remove value from set: `SREM key_name "value"`
  - create sorted set: `ZADD key_name 1 "value"` (here 1 is score which is number)
  - get list of set: `ZRANGE key_name 0 -1`
  - remove value form set: `ZREM key_name "value"`
  - create hash set: `HMSET key_name_obj obj_prop1 "obj_prop1 value" obj_prop2 "obj_prop2 value"`
  - add new property to existing hash set: `HSET key_name_obj obj_prop3 "obj_prop3 value"`
  - get all properties of hash set object: `HGETALL key_name_obj`
  - get specific property of hash set object: `HGET key_name_obj obj_prop`
  - delete specific property hash set object: `HDEL key_name_obj obj_prop`
  - delete whole hash set object: `DEL key_name_obj`  
  - redis all commands: http://redis.io/commands

- Data types in redis
  1. `String`
  2. `List` - order is random. collection of strings. Kind of linked list data type
  3. `Sets` - no order. no duplicates
  4. `Sorted Sets` - order provided by us. no duplicates
  5. `HashSet`

## Redis tutorial
- http://www.tutorialspoint.com/redis/index.htm

## Jedis
- **Example** - http://www.tutorialspoint.com/redis/redis_java.htm

## Redisson
- home - https://github.com/mrniko/redisson
- wiki - https://github.com/mrniko/redisson/wiki
- slack channel - https://gitter.im/mrniko/redisson