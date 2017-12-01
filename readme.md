# Alpine cpp docker image

Alpine based images for c++ development.


## How to build and push image

```
docker build -t alpinecpp .
docker tag alpinecpp kracejic/alpinecpp:latest
docker push kracejic/alpinecpp:latest

docker build -t alplinecppheavy .
docker tag alplinecppheavy kracejic/alplinecppheavy:latest
docker push kracejic/alplinecppheavy:latest
```

Build behind proxy:
```
docker build -t alplinecppheavy . --build-arg http_proxy="$http_proxy" --build-arg https_proxy="$https_proxy"
```

Run image: `docker run -it alpinecppheavy`
Run with proxy: `docker run -e "https_proxy=$https_proxy" -e "http_proxy=$http_proxy" -it alpinecppheavy`


