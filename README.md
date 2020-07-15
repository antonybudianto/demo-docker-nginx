# demo-docker-nginx

## Using docker

docker build . -t demo-nginx

docker build . -t demo-nginx -f Dockerfile

docker run -d -p 8000:80 demo-nginx

docker stop <container-id>

```
$ curl http://localhost:8000
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Document</title>
  </head>
  <body>
    Hello
  </body>
</html>
```

```
$ curl http://localhost:8000/hello
Hello from /hello
```

## Using docker-compose

docker-compose up
docker-compose exec demo_nginx sh
docker-compose stop
docker-compose down
