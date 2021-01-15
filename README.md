# Crie um aplicativo CRUD simples com Python, Flask e React

Este tutorial mostra como construir um aplicativo CRUD básico (Criar, Ler, Atualizar e Excluir) usando Python com Flask como API e React para front-end.

Para quem apresentar problemas como 'PORT' não é reconhecido como um comando interno, modifique seu arquivo package.json para "start": "set PORT=8080 && react-scripts start"

Se você deseja simplesmente clonar este repo e configurá-lo com as configurações do Okta, estas são as etapas abreviadas:

1. Crie uma [conta de desenvolvedor Okta] (https://developer.okta.com/signup) se ainda não tiver uma.


2. Crie um novo aplicativo Web e um aplicativo SPA no Okta com as configurações padrão. Coloque as configurações do aplicativo da web em client_secrets.json 
Para o aplicativo SPA, coloque suas configurações em
`app/http/web/app/src/Main/index.js`. 


3. Inicie o MongoDB com Docker Compose:

       docker-compose up
       export MONGO_URL=mongodb://mongo_user:mongo_secret@0.0.0.0:27017/
       

4. Inicie o back-end Python:

       FLASK_APP=$PWD/app/http/api/endpoints.py FLASK_ENV=development pipenv run python -m flask run --port 4433


5. Inicie o front-end React:

       cd app/http/web/app
       npm i
       npm start
        
       


