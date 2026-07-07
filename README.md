# Projeto-Conceitual-de-Banco-de-Dados---E-commerce
Este projeto foi desenvolvido como parte do desafio de modelagem de banco de dados da formação SQL da DIO.

O projeto representa a modelagem conceitual de um sistema de ecommerce. 
O sistema possui clientes (PF ou PJ), pedidos, produtos, fornecedores, 
vendedores, pagamentos e entregas. Um cliente realiza pedidos, os pedidos possuem produtos,
formas de pagamento e entrega. Os produtos podem ser fornecidos por diferentes fornecedores
e vendidos por vendedores terceiros.

Contexto:

Sitema de Ecommerce com diferenciação de clientes PF e PJ. 
Controle de pedidos e entregas com código de rastreio.

O cliente pode ser PF ou PJ, mas não pode ser os dois ao mesmo tempo.
O pedido pode ter múltiplos produtos.
Os produtos podem ter mais de um fornecedor e vice e versa.
O pedido pode ter mais de uma forma de pagamento.
A entrega contém status e código de rastreio.
Os produtos podem ser vendidos por vendedores(terceiros).

Principais entidades:
Cliente
Cliente PF
Cliente PJ
Fornecedor
Entrega
Estoque
Pagamento
Pedido
Produtos
Vendedor(Terceiro)

Relacionamentos
Cliente 1:n Cliente PJ
Cliente 1:n Cliente PF
Cliente n:m Pedido
Pedido 1:n Pagamento
Pedido 1:1 Entrega
Pedido n:m Produtos
Produtos n:m Estoque
Produtos n:m Vendedor(Terceiro)
Produtos n:m Fornecedor

