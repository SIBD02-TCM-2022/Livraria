# C1: Introdução

## Descrição do Trabalho
Para o nosso trabalho, pretendemos criar uma base de dados de uma livraria. Existem três dados principais— as nossas entidades— os livros, os armazéns, e os clientes.
Os livros estão registados na base de dados com o seu número de série, título, ano de lançamento, género, nome do autor, preço, e stock, sendo que é possível filtrar e procurá-los através de todos estes elementos.

Os clientes compram os livros. Ao comprar um livro, o cliente tem de disponibilizar os seu nome e email. Após a compra, é-lhes automaticamente atribuído um número interno (ID) que ficará registado na base de dados juntamente com os dados fornecidos pelo cliente.

Após cada compra, fica registado na base de dados o número da compra, a data de envio, e a data de receção.

Existem dois armazéns, um no Porto e outro em Lisboa, que enviam os livros para os clientes. Os armazéns encontram-se registados na base de dados com o nome e morada; quando um armazém envia um livro, fica registado o nome e morada do armazém que o enviou e o número de série dos livros enviados.

### Descrição dos requisitos do utilizador
- Os únicos géneros de livros existentes na livraria são romance, ação, aventura, thriller, mistério e fantasia. 
- A livraria só tem livros que foram lançados a partir de 2007. 
- Os clientes podem comprar a quantidade de livros que quiserem.
