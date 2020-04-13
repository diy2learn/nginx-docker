
docker-build:
	docker build -t nginx-alpine -f Dockerfile_nginx_alpine .

check:
	curl localhost:8080

inspect:
	docker exec 619459e50fdd find --name nginx
