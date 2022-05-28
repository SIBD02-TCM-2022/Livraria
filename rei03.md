# C3: Esquema Conceptual

## Entidades
  - LIVRO (nrSerie, titulo, ano, genero, autor, preco)
  - FUNCIONARIO (nrBI, nome, dataNasc, telemovel, email, morada)
  - CLIENTE (nrBI, nome, dataNasc, email, morada)
  - ARMAZEM (nome, morada)
  - PEDIDO (nrPedido, peso, precoPorte)
 
  
## Associações
  - Contacta (FUNCIONARIO, ARMAZEM) 1/N T/T
  - Procura (FUNCIONARIO, LIVRO) 1/N T/T
  - Distribui (ARMAZEM, PEDIDO) M/N T/P
  - Armazena (ARMAZEM, LIVRO) M/N T/T
  - Efetua (CLIENTE, PEDIDO) 1/N P/P
  - Aluga (CLIENTE, LIVRO) 1/1 P/P
  
## Modelo E/A

 ![modelo ea](https://github.com/SIBD02-TCM-2022/Livraria/blob/main/EsquemaConceptual_Livraria.png)
