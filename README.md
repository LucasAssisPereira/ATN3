# Sistema de Gerenciamento de Biblioteca

## Visão Geral

Este Sistema de Gerenciamento de Biblioteca é uma aplicação cliente-servidor desenvolvida em Java 17, projetada para gerenciar operações básicas de biblioteca, como listar livros, registrar novos livros, alugar livros e devolver livros. O sistema utiliza JSON para armazenamento de dados e a biblioteca Gson para parsing e manipulação de JSON.

## Funcionalidades

- **Listar Livros**: Visualizar a lista de livros disponíveis com detalhes, incluindo título, autor, gênero e número de exemplares.
- **Registrar Livros**: Adicionar novos livros à coleção da biblioteca.
- **Alugar Livros**: Emprestar livros da biblioteca.
- **Devolver Livros**: Devolver livros emprestados à biblioteca.

## Dependências

- **Java 17**: A aplicação é desenvolvida e testada com o Java Development Kit (JDK) 17.
- **Gson**: Biblioteca usada para converter objetos Java em JSON e vice-versa.

## Estrutura do Projeto

src
│
├── main
│ ├── java
│ │ ├── library
│ │ │ ├── client
│ │ │ │ └── LibraryClient.java
│ │ │ ├── server
│ │ │ │ ├── Book.java
│ │ │ │ ├── BookManager.java
│ │ │ │ ├── ClientHandler.java
│ │ │ │ └── LibraryServer.java
│ ├── resources
│ │ └── livros.json



## Executando a Aplicação

1. **Inicie o Servidor**


2. **Execute o Cliente**

## Uso

1. **Listar Livros**:
    - Selecione a opção `1` ou digite `listar`.
    - O sistema exibirá a lista de livros disponíveis.

2. **Registrar um Novo Livro**:
    - Selecione a opção `2` ou digite `registrar`.
    - Siga os prompts para inserir os detalhes do livro (nome, autor, gênero, número de exemplares).

3. **Alugar um Livro**:
    - Selecione a opção `3` ou digite `alugar`.
    - Escolha um livro da lista inserindo o número do índice.
    - Se o livro estiver disponível, ele será alugado.

4. **Devolver um Livro**:
    - Selecione a opção `4` ou digite `devolver`.
    - Escolha o livro a ser devolvido inserindo o número do índice.

5. **Sair do Sistema**:
    - Digite `sair` para sair da aplicação cliente.

## Arquivo de Dados JSON

O arquivo `livros.json` localizado no diretório `resources` contém os dados iniciais para a biblioteca. Ele segue a estrutura abaixo:

```json
{
  "livros": [
    {
      "titulo": "Título do Livro",
      "autor": "Nome do Autor",
      "genero": "Gênero",
      "exemplares": 5
    }
  ]
}
