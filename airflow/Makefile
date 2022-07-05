PACKAGES := "airflow"

.PHONY: build
build:
	docker build . -f Dockerfile --tag apache/airflow:lonbaw

.PHONY: up
up:
	docker-compose-for-etl -f docker-compose.yml up -d 

.PHONY: down
down: 
	docker-compose-for-etl -f docker-compose.yml  down

.PHONY: cli
cli:
	docker-compose-for-etl -f docker-compose.yml  run --rm airflow-cli bash

.PHONY: ps 
ps:
	docker-compose-for-etl -f docker-compose.yml  ps 