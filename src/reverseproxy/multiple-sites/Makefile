help:
	@echo "site1-up: build (if needed) and compose-up" 
	@echo "site1-down: docker-compose down site1"
	@echo "site2-up: build (if needed) and compose-up site2"
	@echo "site2-down: docker-compose down site2"
	@echo "reverse-proxy-down: run docker-compose down for reverse-proxy"
	@echo "reverse-proxy-up: run docker-compose up for reverse-proxy"
	@echo "check-site1: check index in site1"
	@echo "check-site2: check index in site2"


site1-up:
	docker-compose -f site1/docker-compose.yml up -d

site1-down:
	docker-compose -f site1/docker-compose.yml down

site2-up:
	docker-compose -f site2/docker-compose.yml up -d

site2-down:
	docker-compose -f site2/docker-compose.yml down

reverse-proxy-down:
	docker-compose -f reverse-proxy/docker-compose.yml down

reverse-proxy-up:
	docker-compose -f reverse-proxy/docker-compose.yml up -d

check-site1:
	curl site1.example.com

check-site2:
	curl site2.example.com
