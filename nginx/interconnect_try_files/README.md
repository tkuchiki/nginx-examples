# Interconnect try_files

```console
$ docker-compose up -d

$ docker-compose exec web1 ls /usr/share/nginx/html
50x.html    index.html  web1

$ docker-compose exec web2 ls /usr/share/nginx/html
50x.html    index.html  web2

$ docker-compose exec web3 ls /usr/share/nginx/html
50x.html    index.html  web3

$ curl -s 127.0.0.1:8080/web1/test.txt
web1
$ curl -s 127.0.0.1:8080/web2/test.txt
web2
$ curl -s 127.0.0.1:8080/web3/test.txt
web3

$ curl -s 127.0.0.1:8081/web1/test.txt
web1
$ curl -s 127.0.0.1:8081/web2/test.txt
web2
$ curl -s 127.0.0.1:8081/web3/test.txt
web3

$ curl -s 127.0.0.1:8082/web1/test.txt
web1
$ curl -s 127.0.0.1:8082/web2/test.txt
web2
$ curl -s 127.0.0.1:8082/web3/test.txt
web3
```
