
export COMPOSE_PROJECT_NAME=osm


up:
	@docker-compose up -d

down:
	@docker-compose down


imposm-logs:
	@docker-compose logs -f --tail=30 imposm

reset-db: down
	@docker volume rm osm_osm-postgis-data
	@docker-compose up -d

restart-imposm:
	@docker-compose restart imposm
