# projeto-oficina
DIO Projeto Oficina
# Projeto Conceitual de Banco de Dados para Oficina Mecânica

Este projeto consiste na criação de um esquema conceitual para um banco de dados de oficina mecânica, utilizando o modelo Entidade-Relacionamento Estendido (EER). O objetivo é modelar as principais entidades e seus relacionamentos, com ênfase na correta especificação de chaves primárias (PK) e chaves estrangeiras (FK).

## Narrativa

O modelo abrange as seguintes entidades:

* **Cliente**: Informações dos clientes que levam seus veículos à oficina.
* **Veículo**: Dados dos veículos dos clientes.
* **Mecânico**: Informações dos mecânicos que trabalham na oficina.
* **Equipe**: Agrupamento de mecânicos responsáveis por uma OS.
* **Ordem de Serviço (OS)**: Detalhes dos serviços a serem executados nos veículos.
* **Serviço**: Descrição dos serviços realizados.
* **Peça**: Detalhes das peças utilizadas nos serviços.

## Observações

* A entidade "Equipe" foi adicionada para representar o agrupamento de mecânicos responsáveis por uma OS.
* As entidades "OS\_Servico" e "OS\_Peca" foram criadas para representar os relacionamentos N:M entre OS e Serviço, e OS e Peça, respectivamente.
* A tabela de referência de mão-de-obra foi modelada como a entidade "Servico", com o atributo "Valor\_Mao\_Obra".
* Os atributos opcionais como "Numero\_Cartao", "Data\_Validade" e "Nome\_Titular" foram adicionados na entidade pagamento, pois são dados opcionais.
* A entidade Item\_Pedido foi removida, pois ela não faz parte dessa narrativa.

## Próximos Passos

* Implementar o esquema em um SGBD relacional.
* Adicionar restrições de integridade ao banco de dados.
* Criar consultas SQL para recuperar e manipular os dados.
* Desenvolver uma aplicação para interagir com o banco de dados.
