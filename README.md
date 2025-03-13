# Esquema Conceitual para Banco de Dados de Controle de Ordens de Serviço em Oficina Mecânica

Este repositório contém o **esquema conceitual** de um banco de dados desenvolvido para controlar e gerenciar ordens de serviço em uma oficina mecânica. O sistema visa automatizar o processo de recebimento de veículos, execução de serviços e controle de peças e mecânicos. 

## Descrição

O projeto foi desenvolvido com base em uma narrativa fornecida, onde clientes levam seus veículos para serem consertados ou revisados. Cada ordem de serviço gerada contém informações sobre os serviços, mecânicos, peças e valores envolvidos.

## Entidades

- **Cliente**: Armazena informações sobre os clientes da oficina.
- **Veículo**: Informações sobre os veículos que são levados para reparo.
- **Ordem de Serviço (OS)**: Detalha os serviços solicitados e sua execução.
- **Mecânico**: Contém informações sobre os mecânicos da oficina e suas especialidades.
- **Serviço**: Serviços realizados, como consertos ou revisões.
- **Peça**: Peças usadas nos serviços.

## Relacionamentos

O banco de dados possui relacionamentos entre as entidades, como:
- Cliente-`Veículo` (1:N)
- Ordem de Serviço-`Serviço` (N:M)
- Ordem de Serviço-`Peça` (N:M)
- Mecânico-`Equipe` (N:M)

## Tecnologias Utilizadas

- MySQL Workbench
- SQL

## Como Rodar

1. Clone o repositório.
2. Importe o arquivo SQL no MySQL Workbench.
3. Execute os scripts para criar o banco de dados e as tabelas.

## License

Este projeto está licenciado sob a [Licença XYZ].
