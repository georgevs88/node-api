# node-api
Curso NodeJS - Rocketseat

Instalar node
Para consultar se está ok e exibir versao: 
node -v

npm (gerenciador de pacote) já deve estar instalado tbm, para conferir:
npm -v

executar o comando para inicializar o projeto:
npm init -y

vai gerar o arquivo package.json, que serve para guardar as informacoes das dependencias do projeto

instalar a dependencia express - framework para ajudar a lidar com rotas (endereços) e views (visualizacoes):
npm install express 
vai adicionar a propriedade exprees no package.json

para executar um arquivo por exemplo:
node server.js

NODEMON - serve para reinicializar automaticamente o servidor qnd houver uma atualizacao do codigo
para instalar (o "-D" é para instalar como dependencia de desenvolvimento):
npm install -D nodemon

na instalacao vai adicionar no package.json o "devDependencies", sao dependencias que é usada apenas no ambiente de desenvolvimento, e nao vai instalar qnd jogar em producao
para utilizar podemos criar um script "dev" no package.json:
		  "scripts": {
			"test": "echo \"Error: no test specified\" && exit 1",
----->    	"dev": "nodemon server.js"
			},
			
daí passamos a rodar assim:
npm run dev

--------------------------------------------

instalar mongo...
instalar mongoose (ORM - encapsula as operacoes do BD no código - transforma as tabelas do BD em objetos no javascript):
npm install mongoose

para não precisar dar um require em cada Schema do banco como abaixo:
require('./src/models/Product')
Instalamos o require-dir:
npm install require-dir

e utilizamos para fazer o require da pasta toda (pasta de models que criamos):
requireDir('./src/models')

			
