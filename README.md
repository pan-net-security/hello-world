# hello-world

A web app container which listens on tcp/8080 and prints "Hello World". 

Static compiled, no dynamic dependencies, no OS (distroless).

## Build 

```sh
docker build -t hello-world .
```

## Run

```sh
docker run --rm -p 8080:8080 hello-world
```

The container will run and bind to port `8080` on `localhost`.
In another terminal screen, do:

```sh
curl localhost:8080
Hello world!
```

## Image Size

```sh
docker image ls hello-world --format '{{ .Size }}'
4.19MB
```
