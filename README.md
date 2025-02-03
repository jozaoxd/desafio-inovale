# Teste de Estágio Inovale

Este projeto é uma aplicação web para interação e controle com um objeto renderizado 3D. Permite que o usuário ajuste as propriedades como intensidade da luz, cor de fundo e a posição do objeto, podendo estas configurações serem salvas e carregas usando o JSON Server.

## Como rodar a aplicação:

### 1. Requisitos
Node.js (com npm).  
JSON Server (para simular um backend).  
Web Browser de sua preferência.

### 2. Inicializando o Projeto

1. Abra o projeto em uma IDE de sua preferência (recomendado Visual Studio Code).  
2. No terminal instale o JSON server com o comando "npm install -g json-server".  
3. Inicie o servidor com o comando "json-server --watch db.json --port 3000".  
4. Coloque para rodar a aplicação.

## Estrutura do Projeto:
O index.html contém todo o frontend da página web e a criação do objeto 3D com three.js, realizando operações de alteração de propriedades, salvamento e carregamento das configurações do usuário. Já o db.json define a coleção de dados que quero armazenar no servidor JSON.

## Explicação sobre a comunicação Frontend-backend:
A comunicação entre o frontend e o backend é feita através de requisições HTTP utilizando a API RESTful criada pelo JSON Server. O frontend realiza operações de GET para carregar as configurações e PUT para salvar as alterações feitas pelo usuário.

## Possível Melhorias futuras:
1. Escolher entre configurações salvas: O projeto atualmente só armazena uma configuração por vez e a substitui caso outra seja feita, o próximo passo seria armazenar mais de uma configuração salva e criar um menu para que o usuário escolha entre elas.  
2. Interface mais agradável: O projeto não utiliza css e é feito de forma simples, podendo ser implementado alguns recursos visuais para que o site tenha um melhor feedback visual.  
3. Suporte a vários tipos de modelo 3D: O projeto conta somente com o modelo 3D de um cubo gerado pelo three.js, porém se implementada a ferramenta, contará com um carregamento de modelos 3D.
