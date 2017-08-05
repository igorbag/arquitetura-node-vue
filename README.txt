Esse projeto é destinado à criação de uma aplicação MEVN (Mongo, Express, Vue.js 2 e Node) 
utilizando os conceitos de arquiteturais HTTP/2 REST.

Frameworks e Tecnologias utilizadas:

BackEnd:
	-NodeJS
	-Express
		

Infraestrutura:
	- Docker
	- MongoDB

FrontEnd:
	- Vue.js V2
	- Vuetify
	

Configurações:
 - Utilizando MLab para armazenar os documentos do MongoDB.

Criando a imagem no Docker:
Vá para o diretório aonde fica o arquivo Dockerfile e execute o seguinte comando, subistituindo o nome de usuário:
$ docker build -t <your username>/node-web-app .

Sua imagem está instalada no Docker:
$ docker images

# Exemplo
REPOSITORY                      TAG        ID              CREATED
node                            boron      539c0211cd76    3 weeks ago
<your username>/node-web-app    latest     d64d3505b0d2    1 minute ago
	
Executando a imagem:
$ docker run -p 49160:8080 -d <your username>/node-web-app


Imprimindo a saida:

# Get container ID
$ docker ps

# Print app output
$ docker logs <container id>

# Example
Running on http://localhost:8080