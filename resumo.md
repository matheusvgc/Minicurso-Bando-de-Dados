# INTRODUÇÃO A ABANCO DE DADOS COM MySQL E PQPMyAdmin

## SQL

Structured Query Language - Linguagem de pesquisa declarativa padrão para banco de dados relacional

## MySQL

Sistema de gerenciamento de banco de dados que utiliza SQL como interface

## phpMyAdmin

- Aplicação PHP para administração do MySQL pela internet
- Permite: criar e remover bases de dados; remover e alterar tabelas, editar campos, executar códigos SQL


## Operações CRUD

Create, Read, Update and Delete

## SQL é dividida em:

### DML - Linguagem de Manipulação de Dados

Permite adicionar, atualizar e apagar dados

-INSERT, UPDATE, DELETE

### DDL - Linguagem de Definição de Dados

Permite criar e alterar dados

-CREATE TABLE, ALTER TABLE, DROP TABLE

### DQL - Linguagem de Consulta de Dados

Permite realizar buscas nas tabelas dos bancos de dados

-SELECT

#### Buscas podem ser melhoradas com cláusulas:

-FROM, WHERE, GROUP BY, ORDER BY

#### Buscas podem ser combinadas com operadores lógicos:

-AND, OR, NOT

#### E condicionais

-<, >, <=, >=, =, <>

## Criando Banco de Dados

### Comandos

#### Criar

-CREATE DATABASE nome_da_base_de_dados

-CREATE TABLE nome_da_tabela(
    nomeDoCampo tipoDeDados,
    nomeDoCampo tipoDeDados,
    ID INT NOT NULL AUTO_INCREMENT PRIMARY KEY
)

#### Renomeando

-RENAME TABLE nome_da_tabela TO novo_nome_da_tablea

#### Apagar

-DROP TABLE nome_da_tabela -> para apagar tabelas
-DELETE -> para apagar dados das tabelas

#### Inserir

-INSERT nome_da_tabela(campo1,campo2,...,campoN)
 VALUES("valor do campo 1", "valor do campo 2", "valor do campo N")

#### Busca com operadores lógicos

-SELECT * FROM nome_da_tabela WHERE nome_do_campo_desejado > "valor"

#### Busca com operadores lógicos e relacionais

-SELECT * FROM nome_da_tabela WHERE nome_do_campo_desejado > "valor" AND nome_do_campo LIKE "%valor%"

#### Atualizar

-UPDATE nome_da_tabela SET nome_do_campo = "novo valor do campo" WHERE ID = id do dado a ser alterado

#### Busca Combinada

SELECT nome_da_tabela1.nome_do_campo_desejado, nome_da_tabela2.nome_do_campo_desejado
FROM nome_da_tabela1, nome_da_tabela2, nome_da_tabela3
WHERE nome_da_tabela1.nome_do_campo_desejado = nome_da_tabela3.nome_do_campo_desejado AND nome_da_tabela2.nome_do_campo_desejado = nome_da_tabela3.nome_do_campo_desejado