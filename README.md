# Jenkins Pipeline to Build Docker Image


``` shell
docker images
docker image build -t ubuntu:flask .
docker run -d --hostname webserv1 --name webserv1 -p 80:5000 ubuntu:flask
docker exec webserv1 ps
curl localhost
```

docker image build -t ubuntu:dbot .