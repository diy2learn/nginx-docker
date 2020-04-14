help:
	@echo '-----TOC----'
	@echo 'dcp-up: docker-compose up'
	@echo 'dcp-down: docker-compose down'
	@echo 'test-proxy: check reverse proxy with whoami http service'
	@echo 'refs: references for more details'

dcp-up:
	docker-compose up -d

dcp-down:
	docker-compose down

test-proxy:
	curl -H "Host: whoami.example.com" localhost
refs:
	@echo 'understand a simple http server- "whoami": https://devopswithdocker.com/part2/'
	@echo 'seems a recent tutor on nginx-proxy: https://blw.sh/blog/create-fast-local-docker-web-dev-environment/'
