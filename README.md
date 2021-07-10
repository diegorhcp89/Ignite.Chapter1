# Ignite.Chapter1
Fundamentos do NodeJS

## Criando o Projeto

- No terminar digitar "yarn init -Y" para criar o arquivo package.json.

## Adicioanando o Express
- No terminar digitar "yarn add express" para criar a pasta node_modules

- Criar a pasta "src" e dentro arquivo "index.js"

    const express = require("express");

    const app = express();

    app.get("/", (request, response) => {
        return response.json({message: "Hello Word Ignite!"});
    });

    //localhost:3333
    app.listen(3333);

## Adicionando o Nodemon na aplicação

- No terminar digitar "yarn add nodemon -D" no package.json após o "licence" criar o script abaixo

    "scripts": {
    "dev": "nodemon src/index.js"
    },

- No terminal digitar "yarn dev" para iniciar a aplicação.

## Métodos HTTP

* GET - Buscar uma informação dentro do servidor
* POST - Inserir uma informação no servidor
* PUT - Alterar uma informação no servidor
* PATCH - Alterar uma informação especifica
* DELETE - Deletar uma informação no servidor

## Tipos de parâmetros

* Route Params => Indentificar um recurso editar/deletar/buscar
* Query Params => Paginação / Filtro
* Body Params => Os objetos inserção/alteração (JSON)