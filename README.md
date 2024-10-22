# Integrantes:

- **João Pedro Moura Tuneli RM:93530**

- **Enzo Massayuki Obayashi RM:95634**

# Cadastro de Usuários e Produtos

Este projeto consiste em uma aplicação web para gerenciamento de usuários e produtos, com o objetivo de implementar e testar funcionalidades de front-end usando o framework de testes [Cypress](https://www.cypress.io/).

## Funcionalidades

A aplicação oferece as seguintes funcionalidades:

- **Cadastro de Usuários**:
  - Criação de um novo usuário com informações como nome, e-mail, senha e outros dados pessoais.
  - Validação de campos obrigatórios e formato de dados (ex.: e-mail válido, senha com critérios de segurança).
  
- **Login de Usuários**:
  - Autenticação de usuários cadastrados na aplicação.
  
- **Cadastro de Produtos**:
  - Adicionar novos produtos ao catálogo, com detalhes como nome, descrição, preço e quantidade disponível.
  - Validação de campos como nome e preço do produto.

- **Listagem de Produtos**:
  - Exibição de uma lista de produtos cadastrados com a possibilidade de editar e remover itens.

## Tecnologias Utilizadas

- **Front-end**: 
  - HTML, CSS e JavaScript (ou frameworks como React/Vue.js, se aplicável)
  
- **Back-end**:
  - Node.js com Express (ou outro framework/backend utilizado para a API)

- **Banco de Dados**:
  - MongoDB, MySQL, ou outro banco de dados de sua escolha.

- **Testes Automatizados**:
  - [Cypress](https://www.cypress.io/)

## Instalação e Configuração

### Instale as dependências:

```bash
npm install
```

### Configure as variáveis de ambiente (se aplicável):

Crie um arquivo `.env` baseado no `.env.example` e preencha com suas configurações.

### Inicie o servidor de desenvolvimento:

```bash
npm start
```

A aplicação estará disponível em `http://localhost:3000` (ou outro host configurado).

## Executando os Testes com Cypress

Para rodar os testes automatizados de front-end, siga os passos abaixo:

### Instale as dependências do Cypress:

```bash
npm install cypress --save-dev
```

### Abra a interface gráfica do Cypress para executar os testes:

```bash
npx cypress open
```

Ou, para rodar os testes em modo headless (sem interface gráfica):

```bash
npx cypress run
```

O Cypress vai rodar os testes definidos na pasta `cypress/integration`.

## Estrutura dos Testes

Os testes de front-end incluem cenários para validar as seguintes funcionalidades:

### Cadastro de Usuários:
- Testes de preenchimento correto dos campos.
- Testes de validação de erros para campos obrigatórios e inválidos.

### Login de Usuários:
- Testes de autenticação com credenciais válidas e inválidas.

### Cadastro de Produtos:
- Verificação de inserção correta de produtos.
- Testes de validação de campos obrigatórios e de preços válidos.

### Listagem e Manipulação de Produtos:
- Testes para garantir que a lista de produtos seja exibida corretamente.
- Testes de edição e exclusão de produtos.

## Estrutura do Projeto

```bash
├── cypress/                # Pasta contendo os testes do Cypress
│   ├── fixtures/           # Arquivos de dados de teste (opcional)
│   ├── integration/        # Arquivos de testes
│   └── support/            # Configurações globais do Cypress
├── public/                 # Arquivos estáticos da aplicação
├── src/                    # Código-fonte do front-end
│   ├── components/         # Componentes reutilizáveis da aplicação
│   ├── pages/              # Páginas da aplicação
│   ├── services/           # Serviços de comunicação com o back-end
│   └── styles/             # Estilos CSS
├── package.json            # Arquivo de configuração de dependências
└── README.md               # Documentação do projeto
```

## Contribuição

Se você quiser contribuir com o projeto, siga estas etapas:

1. Faça um fork do repositório.
2. Crie uma branch para a sua feature: `git checkout -b minha-feature`.
3. Commit suas mudanças: `git commit -m 'Adicionar nova feature'`.
4. Faça um push para a branch: `git push origin minha-feature`.
5. Abra um Pull Request.

## Licença

Este projeto está licenciado sob a licença MIT - veja o arquivo [LICENSE](LICENSE) para mais detalhes.

Esse é o texto completo no formato Markdown, pronto para ser salvo como `README.md`.
