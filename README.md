# README - Front-End React

## Visão Geral

Este é o repositório do front-end da aplicação, desenvolvido em **React** como **Single Page Application (SPA)**. O front-end consome a API do back-end via **Axios** e gerencia autenticação com **JWT** armazenado em **localStorage**.

## Tecnologias Utilizadas

* React 18+
* Axios
* React Router DOM
* CSS customizado
* localStorage para gerenciamento de estado simples (token JWT)

## Estrutura de Pastas

```
/src
  /components  # Componentes reutilizáveis (botões, cards, formulários)
  /pages       # Páginas principais (Login, Cadastro, Usuários, Chamados)
  /services    # Configuração do Axios e chamadas API
  /App.css     # Estilos globais
  /App.jsx     # Componente principal
```

## Funcionalidades

1. **Autenticação**

   * Tela de login e cadastro.
   * Armazenamento do token JWT no localStorage.
   * Redirecionamento para área autenticada.
   * Logout que limpa o token.

2. **Gerenciamento de Usuários (apenas admin)**

   * Listagem de usuários.
   * Criação de novos usuários.
   * Edição de usuários existentes.
   * Exclusão de usuários com confirmação.
   * Mensagens de sucesso/erro.

3. **Chamados de Suporte**

   * Listagem de chamados abertos.
   * Criação, edição e exclusão de chamados.
   * Mensagens de feedback claras.

4. **Tratamento de erros**

   * Token inválido ou expirado redireciona para login.
   * Campos obrigatórios não preenchidos exibem mensagens.
   * Erros de comunicação com o servidor são exibidos ao usuário.

5. **Layout e UX**

   * Responsivo para desktop e mobile.
   * Navegação clara entre páginas.
   * Padrão visual consistente (cores, botões, tipografia).

## Como Rodar Localmente

1. Clone o repositório:

```bash
git clone <URL_DO_REPOSITORIO_FRONT>
```

2. Entre na pasta do projeto:

```bash
cd nome-do-projeto-front
```

3. Instale as dependências:

```bash
npm install
```

4. Configure a URL da API no arquivo `/services/api.js`.

5. Rode a aplicação:

```bash
npm start
```

6. Acesse via navegador em `http://localhost:3000`.

## Deploy

O front-end pode ser publicado em serviços como **Vercel** ou **Netlify**.

* Exemplo de deploy no Vercel:

```bash
vercel deploy
```

* Certifique-se de que a URL do front-end esteja apontando para a API em produção.

## Observações

* O front-end depende de um back-end com rotas de autenticação e CRUD funcionando.
* Para testes locais, garanta que o back-end esteja rodando e acessível.

## Contato

* Desenvolvido por Felipe Barcelos Rafaeli Falk
