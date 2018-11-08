# BDD Utilizando Behave

O Behave é uma biblioteca Python que permite a escrita de specs em linguagem humana, e a execução dos cenários através de asserts em "linguagem de programação".

## Instalação
#### 1. ChromeDriver:
* `sudo apt-get install chromium-chromedriver`
* `echo  'export PATH=$PATH:/usr/lib/chromium-browser/' >> ~/.bashrc`<br>
Como root (`sudo su`) executar o seguinte comando:
* `curl -o allure-2.6.0.tgz -Ls https://dl.bintray.com/qameta/generic/io/qameta/allure/allure/2.6.0/allure-2.6.0.tgz && tar -zxvf allure-2.6.0.tgz -C /opt/ && ln -s /opt/allure-2.6.0/bin/allure /usr/bin/allure && allure --version`

#### 2. Criar virtualenv:
* Você pode criar seu virtualenv como preferir, ou executar o seguinte comando:
* `make venv`

#### 3. Dependências:
* `make install`

## Execução
Após seguir os passos da instalação, executar o jupyter</br>
`jupyter notebook`