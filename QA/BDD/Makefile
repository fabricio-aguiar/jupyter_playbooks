SHELL := /bin/bash

default: help

.PHONY: venv
venv:  ## cria um virtualenv
	python3 -m venv venv;

.PHONY: install
install: ## instala as dependencias do projeto
	( \
       source ./venv/bin/activate; \
       pip install -r requirements.txt; \
    )

.PHONY: run
run:  ## exibe o comando para executar o jupyter notebook
	printf '\n\nRode o seguinte comando:\nbash -c "source ./venv/bin/activate && jupyter notebook"\n\n'


.PHONY: help
help:  ## menssagem de ajuda
	@grep -E '^[a-zA-Z_-]+:.*?## .*$$' $(MAKEFILE_LIST) | sort | awk 'BEGIN {FS = ":.*?## "}; {printf "\033[36m%-30s\033[0m %s\n", $$1, $$2}'
