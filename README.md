Rails docker example using debugger
This example was based on [this article](https://medium.com/gogox-technology/debugging-rails-app-with-docker-compose-39a3767962f4)

## Setup

Running containers
```
docker-compose up
```

Stop containers
```
docker-compose stop
```

## Debugging

Use byebug in the code to create a breakpoint and then attach the container_id

Listing containers

```
docker ps
```

Attach container

```
docker attach <container_id>
```

Exit from attach

```
Ctrl + p + q
```

Now it's possible running byebug commands like `continue`, `next`, `exit` and so on

