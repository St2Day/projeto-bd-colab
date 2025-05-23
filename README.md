# projeto-bd-colab
Exercício de criação e manipulação de um BD em SQLite usando Google Colab
## Descrição do Projeto

Este repositório contém um projeto de banco de dados SQLite desenvolvido no Google Colab, demonstrando conceitos fundamentais de modelagem de dados e SQL. O projeto implementa um sistema simples de registro de vendas, com tabelas para pessoas, produtos e vendas, utilizando chaves primárias e estrangeiras para estabelecer relacionamentos entre as entidades.

## Estrutura do Projeto

- **Notebook**: [Projeto-BD-SQLite.ipynb](./Projeto-BD-SQLite.ipynb) - Contém todo o código Python e SQL para criação e manipulação do banco de dados.
- **Diagrama ER**: [docs/diagrama_er.png](./docs/diagrama_er.png) - Modelo conceitual representando as entidades e seus relacionamentos.

## Funcionalidades Implementadas

- Criação de tabelas com chaves primárias e estrangeiras
- Inserção de dados nas tabelas
- Consultas SQL simples e com JOIN
- Análise de dados com funções de agregação
- Visualização de dados com gráficos
- Tratamento de erros em operações de banco de dados

## Modelo de Dados

O banco de dados consiste em três tabelas principais:

1. **Pessoas**: Armazena informações sobre os clientes
   - id (PRIMARY KEY)
   - nome
   - idade

2. **Produtos**: Armazena informações sobre os produtos disponíveis
   - id (PRIMARY KEY)
   - descricao
   - estoque
   - preco

3. **Vendas**: Registra as transações realizadas
   - id_venda (PRIMARY KEY)
   - id_pessoa (FOREIGN KEY → Pessoas)
   - id_produto (FOREIGN KEY → Produtos)
   - quantidade
