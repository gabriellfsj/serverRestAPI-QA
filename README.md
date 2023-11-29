# serverRestAPI-QA
Criação de testes de API utilizando postman, newman e newman-htmlextra

## O que é 
Este repositório foi criado para os estudos de automação de API rest usando a API serverRest

## Tecnologias utilizadas
- Postman
- Newman v6.0.0
- Newmanhtmlextra
- node v20.10.0

## Documentação
- Análise Técnica: Análise/
- Doc da API: [Consultar Swagger](https://serverest.dev/#/)


## Como instalar o ambiente 
- Instalar o Node
- Instalar o newman de forma global
  ```
  npm install -g newman
  ```
- Instalar a dependencia dos relatórios
  ```
  npm install -g newman-reporter-htmlextra
  ```
## Como rodar os testes

### Pelo postman
- Importar a collection e o enviroment
- Executar os testes de forma manual ou automatizada

### Pelo newman
- Abra o console de preferência
- Execute o comando:
 ```
   newman run ServeRest_sem_produtos.postman_collection.json -e ServeRest.postman_environment.json -r cli
  ```
- Executar os testes com o relatório Html Extra
 ```
  newman run ServeRest_sem_produtos.postman_collection.json -e ServeRest.postman_environment.json -r cli,htmlextra
  ```
