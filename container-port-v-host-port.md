## Container Port vs Host Port

A few topics to keep in mind:

1. Multiple containers can run on your host machine
2. Your host machine has limited number of ports
3. Conflict may arise if two containers try to bind to the same port on your host machine

Example:

host port 2000 -->  container port 2000
host port 7001 -->  container port 6379
host port 7000 -->  container port 6379

All of these works ✅

None are binding to the same port