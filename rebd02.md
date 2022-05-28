# C2: Esquema Conceptual

## Entidades
  - LIVRO (nrSerie, titulo, ano, genero, autor, preco)
  - FUNCIONARIO (nrBI, nome, dataNasc, telemovel, email, morada)
  - CLIENTE (nrBI, nome, dataNasc, email, morada)
  - ARMAZEM (nome, morada)
  - PEDIDO (nrPedido, peso, precoPorte)
 
  
## Associações
- Contacta (FUNCIONARIO, ARMAZEM) 1/N T/T
- Procura (FUNCIONARIO, LIVRO) 1/1 T/T
- Distribui (ARMAZEM, PEDIDO) M/N T/P
- Armazena (ARMAZEM, LIVRO) M/N T/T
- Efetua (CLIENTE, PEDIDO) 1/N P/P
- Aluga (CLIENTE, LIVRO) 1/1 P/T


## Modelo E/A

![EsquemaConceptual_Livraria](https://user-images.githubusercontent.com/83698988/170834942-9e6bf15d-2285-435d-b4d6-5d4ca02b4e04.png)
