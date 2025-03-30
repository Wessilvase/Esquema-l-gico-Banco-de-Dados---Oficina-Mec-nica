# Esquema Lógico para Banco de Dados de Controle de Ordens de Serviço em Oficina Mecânica

Este repositório contém o **esquema lógico** de um banco de dados desenvolvido para controlar e gerenciar ordens de serviço em uma oficina mecânica. O sistema visa automatizar o processo de recebimento de veículos, execução de serviços e controle de peças, equipes e mecânicos.

## Descrição

O projeto foi desenvolvido com base em uma narrativa fornecida, onde clientes levam seus veículos para serem consertados ou revisados. Cada ordem de serviço gerada contém informações sobre os serviços realizados, os mecânicos responsáveis, as peças utilizadas e os valores envolvidos.

## Entidades

- **Cliente**: Armazena informações sobre os clientes da oficina.
- **Veículo**: Contém dados dos veículos que são levados para reparo.
- **Ordem de Serviço (OS)**: Registra os serviços realizados, valores e status da ordem.
- **Equipe**: Representa um grupo de mecânicos responsáveis por uma ordem de serviço.
- **Mecânico**: Contém informações sobre os mecânicos e suas especialidades.
- **Serviço**: Registra os serviços realizados, incluindo descrição e valor da mão de obra.
- **Peça**: Contém as peças utilizadas nos serviços, incluindo nome e valor.

## Relacionamentos

O banco de dados possui os seguintes relacionamentos entre as entidades:
- **Cliente** - **Veículo** (1:N) → Um cliente pode ter vários veículos.
- **Veículo** - **Ordem de Serviço** (1:N) → Um veículo pode ter várias ordens de serviço.
- **Ordem de Serviço** - **Equipe** (N:1) → Uma ordem de serviço é atribuída a uma equipe.
- **Equipe** - **Mecânico** (1:N) → Uma equipe pode ter vários mecânicos.
- **Ordem de Serviço** - **Serviço** (N:M) → Uma ordem de serviço pode conter vários serviços.
- **Serviço** - **Peça** (N:M) → Um serviço pode utilizar várias peças.

## Tecnologias Utilizadas

- MySQL Workbench
- SQL

## Como Rodar

1. Clone o repositório.
2. Importe o arquivo SQL no MySQL Workbench.
3. Execute os scripts para criar o banco de dados e as tabelas.

## Licença

Este projeto está licenciado sob a [Licença XYZ].

