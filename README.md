# Estudo de testes e automações de APIs
Teste de API Rest do manual a CI/CD

Link curso na Udemy: [Dominando Postman (2023): Testando e Automatizado APIs](https://www.udemy.com/course/dominando-postman-2023-testando-e-automatizado-apis/)
## O que é
Este repositório foi criado para o bootcamp de Teste de API Rest.
## Tecnologias utilizadas
- Postman versão web
- node version v18.16.1
- newman v5.3.2
- newman-reporter-html
## Documentações
- Doc da API: [Consulte Swagger](https://serverest.dev/#/)
## Como instalar o ambiente
- Primeiro: instale o node em seu computador [baixe aqui](https://nodejs.org/en/download)
- Segundo: realize a instalação do newman de forma global [baixe aqui a dependencia](https://www.npmjs.com/package/newman)
```
npm install -g newman
```
- Terceiro: realize a instalação da dependencia dos relatórios (opcional) [newman-reporter-html
](https://www.npmjs.com/package/newman-reporter-html)
```
npm install -g newman-reporter-html
```
## Como rodar os testes
### Pelo Postman web ou desktop
- Import a collection e o environment
- Execute os teste de forma manual ou automatizada
### Pelo newman
- Abra o console de preferência
- Execute a seguinte linha de comando para rodar os testes
```
newman run ServeRest.postman_collection.json -e serveRest_env.postman_environment.json -r cli
```
- Execute os teste com relatório
```
newman run ServeRest.postman_collection.json -e serveRest_env.postman_environment.json -r cli,htmlextra
```
### Report
Se você optou por rodar os teste com o report htmlextra, você gerou um arquivo html com o resultado dos testes, e para verificar as validações você pode abrir a pasta **newman** que foi criada no local em que os arquivos de collection e enviroment se encontram.

## Entre em contato
e-mail: gustavomorenosiqueira86@gmail.com

LinkedIn: https://www.linkedin.com/in/gustavo-moreno-5803a0229
