## Requisitos

* Node.js 20 ou superior
* MySQL 8 ou superior

## Como rodar o projeto baixado

Criar a base de dados "api" no MySQL<br>
Alterar as credencias do banco de dados no arquivo ".env"<br>
Para a funcionalidade recuperar senha funcionar, necessário alterar as credenciais do servidor de envio de e-mail no arquivo .env.<br>

Instalar todas as dependencias indicada pelo package.json
```
npm install
```

Executar as migrations
```
npx sequelize-cli db:migrate
```

Executar as seeders
```
npx sequelize-cli db:seed:all
```

Rodar o projeto
```
node app.js
```

Rodar o projeto usando o nodemon
```
nodemon app.js
```

Abrir o endereço no navegador para acessar a página inicial
```
http://localhost:8080
```


## Sequencia para criar o projeto
Criar o arquivo package
```
npm init
```

Gerencia as requisições, rotas e URLs, entre outra funcionalidades
```
npm install --save express
```

Rodar o projeto
```
node app.js
```

Instalar a dependência de forma global, "-g" significa globalmente. Executar o comando através do prompt de comando, executar somente se nunca instalou a dependência na maquina, após instalar, reiniciar o PC.
```
npm install -g nodemon
```

Instalar a dependência como desenvolvedor para reiniciar o servidor sempre que houver alteração no código fonte.
```
npm install --save-dev nodemon
```

Rodar o projeto usando o nodemon
```
nodemon app.js
```

Abrir o endereço no navegador para acessar a página inicial
```
http://localhost:8080
```

Comando SQL para criar a base de dados
```
CREATE DATABASE celke CHARACTER SET utf8mb4 COLLATE utf8mb4_unicode_ci;
```

Sequelize é uma biblioteca Javascript que facilita o gerenciamento do banco de dados SQL
```
npm install --save sequelize
```

Instalar o drive do banco de dados
```
npm install --save mysql2
```

Sequelize-cli interface de linha de comando usada para criar modelos, configurações e arquivos de migração para bancos de dados
```
npm install --save-dev sequelize-cli
```

Iniciar o Sequelize-cli e criar o arquivo config
```
npx sequelize-cli init
```

Manipular variáveis de ambiente
```
npm install dotenv --save
```

Criar a Models situacao
```
npx sequelize-cli model:generate --name Situations --attributes nameSituation:string
```

Criar a Models usuários
```
npx sequelize-cli model:generate --name Users --attributes name:string,email:string,situationId:integer
```

Executar as migrations
```
npx sequelize-cli db:migrate
```

Criar seeders situations
```
npx sequelize-cli seed:generate --name demo-situations
```

Criar seeders users
```
npx sequelize-cli seed:generate --name demo-users
```

Executar as seeders
```
npx sequelize-cli db:seed:all
```

Criar a migration
```
npx sequelize-cli migration:generate --name alter-users-password
```

Instalar o módulo para criptografar a senha
```
npm install --save bcryptjs
```

Executar down - rollback - Permite que seja desfeita a migration, permitindo a gestão das alterações do banco de dados, versionamento.
```
npx sequelize-cli db:migrate:undo --name nome-da-migration
```

Instalar a dependencia JWT
```
npm install --save jsonwebtoken
```

Validar formulário
```
npm install --save yup
```

Permitir requisição externa
```
npm install cors
```

Criar a migration alterar a tabela users e acrescentar nova coluna
```
npx sequelize-cli migration:generate --name alter-users-image
```

Multer é um middleware node.js para manipulação multipart/form-data, usado para o upload de arquivos. 
```
npm install --save multer
```

Biblioteca para salvar log
```
npm install --save winston
```

Criar a migration alterar a tabela users e acrescentar nova coluna
```
npx sequelize-cli migration:generate --name alter-users-recover-password
```

Módulo para enviar e-mail
```
npm install --save nodemailer
```

## Fazer o merge do projeto no GitHub

Criar nova branch no PC
```
git checkout -b <branch>
```
```
git checkout -b main
```

Mudar de branch
```
git switch <branch>
```
```
git switch main
```

Mesclar o histórico de commits de um branch em outra branch
```
git merge <branch_name>
```
```
git merge dev-master
```

Fazer o push dessas alterações
```
git push origin <branch_name>
```
```
git push origin main
```
