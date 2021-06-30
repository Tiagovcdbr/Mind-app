# README

This README would normally document whatever steps are necessary to get the
application up and running.

Things you may want to cover:

* Ruby version

* System dependencies

* Configuration

* Database creation

* Database initialization

* How to run the test suite

* Services (job queues, cache servers, search engines, etc.)

* Deployment instructions

* ...

## Passo a passo do projeto mind-app.
=========================================================================================
```
Opicional Criar uma branch para poder trabalhar 
dar o comando 
git checkout -b "nome da branch criada" sem aspas
.......

rodar o comando git branch para checar o que foi criado
* significa que a branch criada é atual que está sendo usada conforme a tela vai mostrar.

.......
rodar o comando git checkout main retorna para a branch principal que no caso é "main"
rodar o comando git checkout - retorna uma branch anterior.
```
=========================================================================================
=========================================================================================
```Aplicação gerada com o comando:

.......

rails new mind-app -d postgresql -T

.......

-T para ignorar a parte de testes e adicionar a gem `rspec-rails
```
=========================================================================================
```
comando vim Gemfile estando em branch master ou main

e incluir # Run against this stable release
group :development, :test do
  gem 'rspec-rails', '~> 5.0.0'
end
```
=========================================================================================
```
dentro do grupo de desenvolvimento abaixo da gem 'byebug'

no caso ficaria assim:
 
group :development, :test do
	gem 'byebug',
	gem  gem 'rspec-rails', ------------------------------
     end
```
=========================================================================================
```
Após inserir a gem no group salve a alteração e para isso execute 

A melhor alternativa seria:

    pressione Escape
    Pressione shift+ Z shift+ Z(capital Zduas vezes).
```
=========================================================================================
```
Agora de o comando 

bundle install 

Caso não tenha esses arquivos note que ao final da linha os arquivos serão notados.
Informando e instalando suas versões ex:

Fetching rspec-support 3.10.2  
Installing rspec-support 3.10.2
Fetching rspec-core 3.10.1
Installing rspec-core 3.10.1
Fetching rspec-expectations 3.10.1
Installing rspec-expectations 3.10.1
Fetching rspec-mocks 3.10.2
Installing rspec-mocks 3.10.2
Fetching rspec-rails 5.0.1
Installing rspec-rails 5.0.1
```
=========================================================================================
```
Em seguida executar o comando 

rails generate rspec:install para trazer os arquivos necessários para o projeto.
No caso são esses arquivos.

create  .rspec
      create  spec
      create  spec/spec_helper.rb
      create  spec/rails_helper.rb
```
=========================================================================================
```
Após a instalação rode o comando "rspec" sem aspas

para apresentar a seguinte mensagem:

No examples found.


Finished in 0.00082 seconds (files took 0.34802 seconds to load)
0 examples, 0 failures
```
=========================================================================================
```
Comandos para subir o projeto ao GitHub

…or create a new repository on the command line

git config --global user.name "Fulano de Tal"
git config --global user.email fulanodetal@exemplo.br

echo "# mind-app" >> README.md
git init
git add README.md
git commit -m "first commit"
git branch -M main
https://github.com/..........................git
git push -u origin main

…or push an existing repository from the command line

git remote add origin https://github.com/......................git
git branch -M main
git push -u origin main

git checkout -b fulano-de-tal = adiciona uma branch para trabalhar com algum projeto

git checkout main  = comando para branch principal
git checkout - retorna uma branch

…or import code from another repository

You can initialize this repository with code from a Subversion, Mercurial, or TFS project.
```
=========================================================================================
```
Adicionando a gem devise

Executar o comando vim Gemfile

e colocar gem 'devise' na linha de documentação
===============================================
Rodar o comando  
bundle install
===============================================
Seguido do
rails generate devise:install
```
