# Angular6Bootstrap4Model

This project was generated with [Angular CLI](https://github.com/angular/angular-cli) version 6.0.8.

## Dicas de comandos para Instalação/Configuração

criando projeto com sistema de rotas
	ng new Angular6-Bootstrap4-model --routing

rodando app para verificar instalacao
	dentro do novo diretorio
		ng serve --open		->> '--open' opcional para abrir navegador
		
parando execucao do servidor/app
	control + c
	S
	
instalando/configurando Bootstrap
	1.Antes:
		observe q dentro do diretorio 'ng_modules' não existe a pasta 'bootstrap'
	
	2.comando para instalacao:
		npm install --save bootstrap	->> '--save' opcional para grava no package.json
		
	3.Apos a instalacao:
		verifique dentro do diretorio 'ng_modules' se existe a pasta 'bootstrap'
		
	4.verifique no arquivo 'package.json' que foi incluido a dependencia:
		ex: "bootstrap": "^4.1.1",
		
	5.dentro do arquivo 'angular.json
		antes da alteracao:			
			"styles": [
              "src/styles.css"
            ],
			
		adicione a linha
			"node_modules/bootstrap/dist/css/bootstrap.min.css"
			
		depois da alteracao fica assim:
			"styles": [
              "src/styles.css",
			  "node_modules/bootstrap/dist/css/bootstrap.min.css"
            ],
		
instalndo/configurando jQuery
	npm install --save jquery
	
	dentro do arquivo 'angular.json'
		"scripts": [
            "node_modules/jquery/dist/jquery.slim.min.js",
			"node_modules/bootstrap/dist/js/bootstrap.bundle.min.js"
		]
	
	nota: o arquivo 'bootstrap.bundle.min.js' 
		eh utilizado pq o 'bundle' jah inclui o 'popper' necessario para integrar bootstrap com jquery
		na utilizacao de 'dropdown' por exemplo
		
	
criando componente com Angular/CLI
	ng genarete component my-new-component
	ng g c my-new-component

	
	
	