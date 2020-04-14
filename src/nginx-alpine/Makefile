help:
	@echo '-----TOC------'
	@echo 'docker-build: build nginx-alpine'
	@echo 'docker-run: run the nginx-alpine image'
	@echo 'check: check the container with curl'
	@echo 'inspect: an example of inspecting container content' 

docker-build:
	docker build -t nginx-alpine -f Dockerfile_nginx_alpine .

docker-run:
	docker run --rm -d -p 8080:80 --name nginx-alpine-example nginx-alpine

check:
	curl localhost:8080

inspect:
	docker exec nginx-alpine-example find -name nginx
