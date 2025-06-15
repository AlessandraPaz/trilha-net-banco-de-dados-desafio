# 🎬 Desafio de Banco de Dados SQL Server: Site de Filmes (DIO .NET)

Este repositório contém a solução do desafio de banco de dados do módulo SQL Server da trilha .NET da Digital Innovation One (DIO). O projeto simula o gerenciamento de dados de filmes e atores, com foco em consultas SQL.

---

## 🗄️ Modelo do Banco de Dados

O banco de dados `Filmes` é composto pelas seguintes tabelas:

* **`Filmes`**: Detalhes dos filmes (`Id`, `Nome`, `Ano`, `Duracao`).
* **`Atores`**: Informações dos atores (`Id`, `PrimeiroNome`, `UltimoNome`, `Genero`).
* **`Generos`**: Categorias de filmes (`Id`, `Genero`).
* **`ElencoFilme`**: Relacionamento muitos-para-muitos entre `Filmes` e `Atores`, incluindo o `Papel` do ator (`Id`, `IdAtor`, `IdFilme`, `Papel`).
* **`FilmesGenero`**: Relacionamento muitos-para-muitos entre `Filmes` e `Generos` (`Id`, `IdGenero`, `IdFilme`).

---


## 🔍 Consultas Implementadas

O arquivo `db/queries.sql` contém a resolução das seguintes consultas:

1.  Buscar o nome e ano dos filmes.
2.  Buscar o nome e ano dos filmes, ordenados por ano crescente.
3.  Buscar informações do filme "De Volta para o Futuro" (nome, ano, duração).
4.  Listar filmes lançados em 1997.
5.  Listar filmes lançados APÓS o ano 2000.
6.  Buscar filmes com duração entre 100 e 150 minutos, ordenando pela duração.
7.  Contar a quantidade de filmes lançados por ano, agrupando e ordenando por ano.
8.  Listar Atores do gênero masculino.
9.  Listar Atores do gênero feminino, ordenando pelo PrimeiroNome.
10. Buscar o nome do filme e seu gênero.
11. Buscar o nome do filme e o gênero "Mistério".
12. Buscar o nome do filme, seus atores e o papel desempenhado por cada um.

---

## 🛡️ Licença

Este projeto está sob a [MIT License](LICENSE).
