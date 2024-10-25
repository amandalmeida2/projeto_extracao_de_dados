# Projeto Extração de Dados ETL

Um projeto desenvolvido para o curso de Engenharia de Dados do programa Santander Coders 2024 em parceria com a Ada Tech, focado na trilha de extração de dados. 
A ideia principal é criar um pipeline de ETL (Extração, Transformação e Carga) e para isso utilizamos a API do TheMovieDB (TMDB) para extrair informações sobre filmes e séries de TV. 

## 📚 Equipe
Amanda Almeida<br>
Naiara Andrade<br>
## 🎯 Objetivo
O objetivo deste projeto é demonstrar a construção de um pipeline ETL em Python.

## 🔑 Como Obter sua Própria API Key no TMDB
Para utilizar o projeto sem se preocupar com os limites de requisições, recomendamos cada usuário crie sua própria API Key. Siga os passos abaixo:

Acesse o site do TheMovieDB (TMDB).<br>
Crie uma conta gratuita ou faça login, caso já tenha uma.<br>
Navegue até as configurações da sua conta e vá para a seção API.<br>
Solicite uma nova chave de API.<br>
Copie a chave gerada e adicione ao arquivo .env conforme indicado abaixo:<br>

## 🗂️ Configuração do Arquivo .env
Crie um arquivo .env na raiz do projeto e adicione sua chave da API:

``` makefile
TMDB_API_KEY=YOUR_API_KEY_HERE
```
Substitua YOUR_API_KEY_HERE pela sua chave de API.

## 📜 Licença
Este projeto é licenciado sob a licença MIT.
