
# Sistema de Biblioteca

## Apresentação

Sistema desktop desenvolvido em Java para o gerenciamento de livros, com interface gráfica e integração com banco de dados MySQL.

O projeto foi desenvolvido como atividade prática da disciplina de Programação, com a finalidade de aplicar conceitos de programação orientada a objetos, desenvolvimento de interfaces gráficas, manipulação de dados e integração com bancos de dados relacionais.

## Funcionalidades

- Cadastro de livros;
- Consulta e listagem de livros;
- Edição de informações;
- Exclusão de registros;
- Pesquisa por título ou autor.

## Tecnologias utilizadas

- Java 21;
- Java Swing;
- MySQL;
- JDBC;
- Apache NetBeans.

## Banco de dados

O banco de dados `biblioteca` utiliza a tabela `livros` para armazenar os registros, com os campos de identificação, título, autor, gênero e ano de publicação. A comunicação entre a aplicação e o MySQL é realizada por meio do JDBC.

Para criar a estrutura necessária, execute no MySQL Workbench:

```sql
CREATE DATABASE biblioteca;

USE biblioteca;

CREATE TABLE livros (
    id INT AUTO_INCREMENT PRIMARY KEY,
    titulo VARCHAR(150) NOT NULL,
    autor VARCHAR(150) NOT NULL,
    genero VARCHAR(100) NOT NULL,
    ano_publicacao INT NOT NULL
);
```

## Execução

1. Clone o repositório:
   ```bash
   git clone https://github.com/sofiasdorneles/biblioteca-livros.git
   ```
2. Crie o banco de dados conforme as instruções.
3. Configure as credenciais do MySQL em `Conexao.java`.
4. Abra o projeto no Apache NetBeans.
5. Execute a classe `Biblioteca.java`.

## Estrutura do projeto

- `Biblioteca.java` — classe principal;
- `TelaInicial.java` — tela de apresentação;
- `TelaBiblioteca.java` — interface de gerenciamento;
- `Livro.java` — representação dos livros;
- `Conexao.java` — conexão com o banco de dados.# Sistema de Biblioteca

## Apresentação

Sistema de gerenciamento de biblioteca desenvolvido em Java, com interface gráfica e integração com banco de dados MySQL.

## Funcionalidades

- Cadastro de livros;
- Consulta e listagem de livros;
- Edição de informações;
- Exclusão de registros;
- Pesquisa por título ou autor.

## Tecnologias utilizadas

- Java 21;
- Java Swing;
- MySQL;
- JDBC;
- Apache NetBeans.

## Banco de dados

O banco de dados `biblioteca` utiliza a tabela `livros` para armazenar os registros, com os campos de identificação, título, autor, gênero e ano de publicação. A comunicação entre a aplicação e o MySQL é realizada por meio do JDBC.

Para criar a estrutura necessária, execute no MySQL Workbench:

```sql
CREATE DATABASE biblioteca;

USE biblioteca;

CREATE TABLE livros (
    id INT AUTO_INCREMENT PRIMARY KEY,
    titulo VARCHAR(150) NOT NULL,
    autor VARCHAR(150) NOT NULL,
    genero VARCHAR(100) NOT NULL,
    ano_publicacao INT NOT NULL
);
```

## Execução

1. Clone o repositório:
   ```bash
   git clone https://github.com/sofiasdorneles/biblioteca-livros.git
   ```
2. Crie o banco de dados conforme as instruções.
3. Configure as credenciais do MySQL em `Conexao.java`.
4. Abra o projeto no Apache NetBeans.
5. Execute a classe `Biblioteca.java`.

## Estrutura do projeto

- `Biblioteca.java` — classe principal;
- `TelaInicial.java` — tela de apresentação;
- `TelaBiblioteca.java` — interface de gerenciamento;
- `Livro.java` — representação dos livros;
- `Conexao.java` — conexão com o banco de dados.