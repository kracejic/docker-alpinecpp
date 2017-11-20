# Alpine cpp docker image

Alpine based images for c++ development.


## How to build and push image

```
sudo docker build -t alpinecpp .
sudo docker tag alpinecpp kracejic/alpinecpp:latest
sudo docker push kracejic/alpinecpp:latest
```

Run image: `sudo docker run -it ubuntugitlabci`


