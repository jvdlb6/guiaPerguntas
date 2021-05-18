# guiaPerguntas
PRSys - Guia de Instalação

Etapas

1 - Baixar e instalar o NodeJs de nodejs.org/en - Usar a versão LTS mais recente;

2 - Criar a pasta do projeto;

3 - Descompactar o arquivo GuiaPerguntas.zip;

4 - No prompt comando executar >npm init 

5 - O mysql deve estar instalado e rodando. Crie um banco de dados localhost chamado ‘guiaperguntas’ 

6 - Edite o arquivo database.js e altere colocando a sua senha root conforme destacado.


const Sequelize = require('sequelize');

const connection = new Sequelize('guiaperguntas','root','suaSenhaRoot',{
    host: 'localhost',
    port: '3306',
    dialect: 'mysql'
});

module.exports = connection;

7 - Execute o servidor, no prompt de comando, >node index.js 


Na primeira vez que o servidor é executado, as tabelas são criadas automaticamente. Use seu navegador e acesse a página localhost:8080.

