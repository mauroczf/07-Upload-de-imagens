# ignite-reactjs-upload-de-imagens
[Ignite: React.js] - Chapter IV - Desafio: Upload de imagens

www.notion.so/desafio-02-upload-de-imagens-4cf1c3b1c1ad4a66961b6e48558cc3b8

## Como executar essa aplicação localmente?

####  Pré-requisitos:
Antes de começar, você vai precisar ter instalado em sua máquina as seguintes ferramentas: [Git](https://git-scm.com/), [Node.js](https://nodejs.org/en/), [Yarn](https://yarnpkg.com/). 

Além de um editor de código como o [VSCode](https://code.visualstudio.com/).

[Criar uma conta](https://imgbb.com/login) no ImgBB e [criar a sua chave](https://api.imgbb.com/) da API.

Copiar o valor dessa chave e colar no seu `.env.local` da seguinte forma: `NEXT_PUBLIC_IMGBB_API_KEY=VALOR_DA_CHAVE_COPIADA`.

Criar um banco no [FaunaDB](https://docs.fauna.com/fauna/current/learn/quick_start/quick_start) 
com um nome de sua preferência que **precisa** ter uma coleção chamada `images`. Com o banco e coleção criados, basta você criar e copiar a chave do banco no seu arquivo `.env.local` da seguinte forma: `FAUNA_API_KEY=VALOR_DA_CHAVE_COPIADA`

    # Clone o repositório em sua máquina
    $ git clone git@github.com:kaiquezimerer/ignite-reactjs-upload-de-imagens.git
    
    # Acesse a pasta do projeto pelo terminal/cmd
    $ cd ignite-reactjs-upload-de-imagens/
    
    # Instale as dependências
    $ yarn install
    
     # Copie o arquivo .env-sample para .env.local
    $ cp .env-sample .env.local

    # Altere o .env.local com os dados do repositório do ImgBB e Fauna (via nano, vim ou qualquer editor)
    $ nano .env.local
    
    # Em outro terminal/cmd, inicialize o projeto em modo de desenvolvimento
    $ yarn dev
    
    # A aplicação iniciará na porta :3000- acesse http://localhost:3000
    
## Como executar os testes automatizados?

    # Na pasta do projeto, execute o comando para rodar todos os testes
    $ yarn test
