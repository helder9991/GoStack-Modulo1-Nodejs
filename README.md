# Explicação

Este código foi desenvolvido a partir do bootcamp da Rocketseat durante o módulo 1, onde busca apresentar os conceitos iniciais para o desenvolvimento do backend em NodeJS. Em sua base, o código utiliza em seu conceito a biblioteca Express (presente no NodeJS) para o desenvolvimento das regras de negócio da aplicação.

# Conceitos

Está aplicação se baseia nos repositórios presente na ferramenta GitHub, no qual dentro desta aplicação é possivel realizar a listagem de todos os repositórios cadastrados previamente, cadastrar um novo repositório, atualizar informações (title, url e techs) e fazer a remoção do mesmo. Outro feito possivel é a realização de um 'cadastro' de um novo like em um repositório já existente. Para o manuseio das informações apresentadas previamente foi utilizado as seguintes estruturas para os repositórios:
```
  -id: Identificador Único
  -title: Titulo do repositório
  -url: Link onde se encontra o repositório
  -techs: Tecnologias presentes no repositório
  -likes: Quantidade de likes que o repositório possui
```

# Rotas

O backend foi desenvolvido a partir da arquitetura API REST, no qual para o manejo das regras de negócio utiliza-se
os seguintes métodos HTTP:
  
  - ```GET /repositories```: Lista todos os usuarios cadastrados na aplicação.
  - ```POST /repositories```: Realiza o cadastro de um usuario.
  - ```POST /repositories/:id/like``` Realiza o 'cadastro' de um novo like
  a partir de um ID.
  - ```PUT /repositories/:id```: Altera informações referentes ao title, url e techs a partir de um ID. 
  - ```DELETE /repositories/:id```: Remove usuário a partir de um ID.
  
  
# Utilização do repositório e realização de testes automatizados
  
  Para utilizar o repositório basta clonar os arquivos em sua maquina e executar o comando **yarn** para que ele
  baixe as bibliotecas presente no **node_modules**.
  
  Observação: Para isso é necessario ter o Node instalado em sua maquina e o yarn.
  
  Para realizar os testes automatizados basta digitar o commando:
  ```yarn test```
  


