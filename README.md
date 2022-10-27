# README

Aqui vai a doc dessa API

API criada com RAILS 6 e RUBY 3

API de exemplo aqui sera uma API de nomes de super herois

PASSO A PASSO ->

1 Criar projeto com o comando -> rails new nome_projeto --api
esse comando cria um projeto completo Rails voltado para API Backend, nao criando arquivos desnecessarios de front

2 LInkar projeto ao seu repositorio online

3  Rodar o comando para criar sua primeira MIGRATION -> Criar tabelas : 
    rails g scaffold NOME_TABELA name:string
 para tornar um campo da tabela obrigario (NOT NULL) ir ate a migrate gerada e adicionar ao codigo , null: false

4 Criar banco de dados
o RAILS cria de forma automatica o DB TESTER e o DB DEV, entao é so rodar -> rails db:create

5 Rodar sua migration criada no passo 3 para popular seu banco recem criado
comando -> rails db:migrate

6 Startar aplicacao -> rails s

obs.: o Rails te permite instanciar a classe que cria sua tabela no console, e popular sua tabela por ali tbm de forma simples
seria como:

rails c
myclass = Class new
myclass.name = "meu nome novo"
myclass.save