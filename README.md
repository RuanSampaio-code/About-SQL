# Welcome to About-SQL
![Banco de dados imagem](https://d1lc5plzz0mq74.cloudfront.net/wp-content/uploads/2021/11/28145724/Banco-de-dados.jpg)
 My studies in Mysql
 # Banco de dados MySQL

Banco de dados são conjuntos de tabelas tabelas, tabelas são um conjunto de Registro, registros são um conjunto de campos.

Composição: base de dados, sistema gerenciador de banco de dados(SGBD, DMS), linguagem de exploração,programas adicionai

## Modelo de banco de dados

- Modelo hierárquico
- Modelo em rede
- Modelo relacional. (Atualmente)
    - Os dados tem uma relação mais intrinseca.

## Linguagem de exploração

SQL - Structured Query Language

Exemplos: mySql, SQL server, mariadb,

## Grupos de comandos

DDL - linguagem de definição. 

- Create table, create database.

DML - comandos de manipulação dos dados

- INSERT into

DCL - Linguagem de controle

SQL - Consulta de dados (SELECT)

## Criar banco de dados

CREATE DATABASE cadastro;

## Criar tabela

CRATE TABLE pessoas (

Campo1 varchar(30),

Campo1 tinyint,

Campo3 char,

Campo4 float,

 );

## Tipos primitivos banco de dados MySQL

- Númerico
    - Inteiro
        - TinyInt, SmallInt, Int, MediumInt, BigInt.
    - Real
        - Decimal, float, double, real
    - Lógico
        - Bit, boolean.

- Data tempo
    - Date, datetime, timestamp, time year, year
- Literal
    - Caráctere
        - Var e varchar
    - Texto
        - TinyText, text, medium text, long text
    - Binário
        - TinyBlob, Blob, MediumBlob..
    - Coleção
        - Enum e Set
- Espacial
    - Geometry, polygon, Point.

## Remover um banco

DROP DATABASE nomedobanco;

## Usar um banco e aplicar mudanças

USE banco;

## Remover tabela

DROP TABLE tabela;

## Alterar uma tabela (ADICIONANDO COLUNA(

ALTER TABLE nometabela ADD COLUM nomecoluna tipo( );

~adicina coluna no final

## Escolhendo posição na coluna

ALTER TABLE tabela

ADD COLUMN nomecoluna after nomecolunaexistente;

~adiciona uma coluna depois de um coluna predeterminada.

## Coluna no começo

ALTER TABLE nometabela

ADD nomecoluna INT FIRST

## Modificando definições

Pode alterar tipos primitivos do campo e alterar CONSTRAINS.

ALTER TABLE nometabela

MODIFY COLUM nomecoluna VARCHAR(10);

## Alterando nome de uma coluna

ALTER TABLE nometabela

CHANGE COLUMN nameold namenew CONSTRAINS;

## Alterando nome da tabela

ALTER TABLE nomeantigo

RENAME TO nomenovo;

## Selecionar todos os dados de tabela

SELECT * FROM nometabela;

## Selecionar dados específicos

SELECT dadoespecifico FROM nometabela;

## CRUD

C = create = INSERT

R = read = SELECT (WHERE)

U = update

D = Delete 

## Inserir dados na tabela

INSERT INTO tabela (nome,salário,data)

VALUES (“nome1” , 5000,“ ano-mes-dia”)

## Inserir dados mais específicos

SELECT * FROM nometabela

WHERE dados > 5000;

## UPDATE

UPDATE nometabela SET coluna;

//SET é para delimitar a coluna

## Remover dados da tabela

DELETE FROM tabela WHERE coluna = dado;

## CONSTRAINS (restrições)

Usadas para especificar regras para dados em uma tabela. Usado pra limitar os tipos de dados.

- PRIMARY KEY - identifica exclusivamente cada linha.
- NOT NULL - não ter dados null.
- UNIQUE  -
- FOREIGN KEY - relaciona tabelas, é um campo q aponta pra uma chave primária de outra tabela
- DEFAULT - valor padrão pra uma coluna.

## SOBRE JOIN

Consulta entre duas ou mais tabelas por meio de uma relação .

Tipos :

In
