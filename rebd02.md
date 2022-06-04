# C2: Esquema Conceptual

## Entidades
- LIVRO (nrSerie, titulo, ano, nomeAutor, género, preco, stock)
- CLIENTE (numero, nome, email)
- ARMAZEM (morada, nome)
- COMPRA (nrCompra, dataEnvio, dataReceção)

 
  
## Associações
- Compra (CLIENTE, LIVRO) 1:N P/T
- Envia (ARMAZEM, LIVRO) M:N T/T
- Regista (ARMAZEM, COMPRA) M:N T/P



## Modelo E/A

![EsquemaConceptual_Livraria](https://user-images.githubusercontent.com/83698988/171970701-aca9b855-1092-46e7-adac-a6a5d6e38ec0.png)
