SHELL=/bin/bash
api-server/%: ## api-server/${lang}docker-compose up with mysql and api-server
	docker-compose -f docker-compose/$(shell basename $@).yaml stop
	docker-compose -f docker-compose/$(shell basename $@).yaml up --build

isuumo/%: ## isuumo/${lang} docker-compose up with mysql and api-server frontend nginx
	docker-compose -f docker-compose/$(shell basename $@).yaml stop -v
	docker-compose -f docker-compose/$(shell basename $@).yaml up

