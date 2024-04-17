# Banco de dados Postgresql e Prisma

## Introdução

Este projeto é um exemplo de como criar e se conectar com um banco de dados utilizando o PostgreSQL através do WSL e conectando através do Prisma com o Next.js para o desenvolvimento do site.  

## Pré-requisitos

- [Node.js](https://nodejs.org/en/)
- [WSL](https://docs.microsoft.com/pt-br/windows/wsl/install) (recomendado o Ubuntu 20.04)
- [git](https://git-scm.com/)

## Instalação e configuração do banco de dados

1. Abra terminal do windows e inicie o WSL com o comando `wsl`
2. Verifique se há alguma atualização disponível com o comando `sudo apt update`
3. Instale o PostgreSQL com o comando `sudo apt install postgresql`
4. Inicie o serviço do PostgreSQL com o comando `sudo service postgresql start`
5. Mude a senha do usuário `postgres` com o comando `sudo passwd postgres` e digite a nova senha
6. Crie um banco de dados com o nome `fullstack` com o comando `sudo -u postgres createdb fullstack`

## Instalação e configuração do Next.js com Prisma

1. Clone o repositório através do comando `git clone https://github.com/gabu322/fullstack-base.git`
2. Entre na pasta do projeto `cd fullstack-base`
3. Instale as dependências do projeto `npm install`
4. Utilize o comando a seguir para se conectar com o banco de dados e criar as tabelas `npx prisma migrate dev --name init`
5. Rode o programa com o comando `npm run dev`
6. Abra o navegador e acesse `http://localhost:3000/` e comece a testar o site
