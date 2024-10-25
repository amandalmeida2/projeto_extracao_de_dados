# Projeto Extração de Dados ETL

Um projeto desenvolvido para o curso de Engenharia de Dados do programa Santander Coders 2024 em parceria com a Ada Tech, focado na trilha de extração de dados. <br>
Este projeto demonstra a construção de um pipeline ELTL (Extração, Carga Intermediária, Transformação e Carga Final) em Python, utilizando a API do TheMovieDB (TMDB).
O objetivo é extrair dados sobre filmes, gêneros e popularidade de pessoas do cinema, processá-los e armazená-los em um formato adequado para análise. 
A configuração de ELTL permite uma carga intermediária, onde os dados brutos são salvos no data lake antes de serem transformados e enviados ao data warehouse.
## 📚 Equipe
Amanda Almeida<br>
Naiara Andrade<br>

## 📑 Descrição
O pipeline consiste nas seguintes etapas:<br>

**Extração:** Coleta dados de filmes, gêneros e pessoas populares do TMDB.<br>

**Carga Intermediária:** Armazena os dados brutos no data lake.<br>

**Transformação:** Converte e organiza os dados em um formato padronizado, aplicando alterações de datas e juntando informações de gêneros.<br>

**Carga Final:** Salva os dados transformados em um data warehouse.<br>

## 🚀 Funcionalidades

### Métodos Principais
**extract:** Extrai dados de filmes populares do TMDB e retorna um DataFrame com os resultados.<br> 

**intermediate_load:** Armazena os dados extraídos de filmes brutos no data lake em formato Parquet.<br>

**transform:** Realiza a transformação dos dados de filmes extraídos, incluindo a formatação das datas, a remoção de colunas desnecessárias e a junção com o DataFrame de gêneros.<br>

**final_load:** Salva o DataFrame transformado em um data warehouse no formato Parquet.<br>

**run:** Executa o pipeline completo de ELTL, desde a extração até a carga final dos dados.

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
