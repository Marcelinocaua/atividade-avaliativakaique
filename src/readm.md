
## Sobre o projeto
O projeto consiste em um aplicativo para gerenciar estoque.

## Tecnologias

 "body-parser": "^1.20.2",
    "chokidar": "^3.6.0",
    "connect-livereload": "^0.6.1",
    "ejs": "^3.1.10",
    "express": "^4.19.2",
    "express-session": "^1.18.0",
    "livereload": "^0.9.3",
    "md5": "^2.3.0",
    "mysql2": "^3.11.3",
    "nodemon": "^3.1.4",
    "pg": "^8.12.0"


## Criar banco e tabela do projeto

```sql

use app_estoque_mvc;

/** COLUNAS PARA TABELA DE PRODUTOS **/  

CREATE TABLE produto (
  id int primary key auto_increment,  
   produto varchar(255),   
   fornecedor varchar(255),  
   quantidade varchar(255),  
   criadoEm date
); 



/** COLUNAS PARA TABELA DE USUARIOS **/  

CREATE TABLE usuarios (      
  id int primary key auto_increment,   
  nome varchar(255),    
  email varchar(255) unique,  
  senha varchar(255),   
  criadoEm date
);


select * from produto;

select * from usuarios;

select * from usuarios where email = "cauamarceliino0682@gmail.com";

```

## Como executar o projeto

```bash
## Clone o projeto
git clone https://github.com/Marcelinocaua/atividade-avaliativakaique.git

## Entre na pasta do projeto
cd GERENCIADOR-ESTOQUE-MVC

## Instale as dependências
npm install

## Inicie o projeto
npm start
```

Made with ♥ by [Cauã Marcelino](www.linkedin.com/in/cauã-marcelino-573200294) :wave: