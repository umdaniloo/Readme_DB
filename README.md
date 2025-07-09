Modelagem abaixo apresentada na aula de Modelagem de BD de E-commerce 

![image](https://github.com/user-attachments/assets/1690c771-6b3e-4712-b980-9b63b7c84419)


Relacionamentos principais
1.	Cliente → Pedido
o	Um cliente (Cliente) pode fazer vários pedidos (Pedido).
o	Relacionamento de 1:N (um para muitos).
2.	Pedido → Relacao_Produto_Pedido → Produto
o	Cada pedido pode conter vários produtos (relacionamento N:N).
o	Essa relação é intermediada pela tabela Relacao_Produto_Pedido, que funciona como uma tabela associativa.
3.	Produto → Fornecedor
o	Cada produto tem um fornecedor (Fornecedor).
o	Relacionamento de N:1 (muitos produtos para um fornecedor).
4.	Fornecedor → Disponibilizando_um_Produto → Produto
o	Essa tabela representa os produtos que um fornecedor está disponibilizando.
o	Relacionamento de N:N usando tabela associativa.
5.	Produto → produtos por vendedor (terceiro) → Terceiro - Vendedor
o	Permite que vendedores terceiros também ofereçam produtos.
o	Relacionamento de N:N com quantidade específica para cada produto.
6.	Produto → Produto_has_Estoque → Estoque
o	Um produto pode estar associado a vários locais de estoque com diferentes quantidades.
o	Relacionamento de N:N via tabela associativa.


Abaixo fizermos algumas melhorias 

Padronização dos nomes das tabelas (evitar espaços, acentuação)
Inclusão da tabela Pagemento

![image](https://github.com/user-attachments/assets/545acc66-feab-46b5-b137-5ed2aa14cc02)
