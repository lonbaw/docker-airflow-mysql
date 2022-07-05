PACKAGES := "mysql8.0"

.PHONY: up
up:
	docker-compose-for-etl -f docker-compose.yml  up -d 

.PHONY: down
down: 
	docker-compose-for-etl -f docker-compose.yml  down

.PHONY: ps 
ps:
	docker-compose-for-etl -f docker-compose.yml  ps 