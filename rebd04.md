# C4: Esquema Relacional

- Entidades-Tipo

#### Livro 
| nrSerie       | titulo               | genero             | ano  | preco | nomeAutor                                    | stock | 
| ------------- | -------------------- | ------------------ | ---- | ----- | -------------------------------------------- | ----- | 
| 9789899096424 | A hipótese do Amor   | romance            | 2022 | 17,50 | Ali Hazelwood                                | 10    | 
| 9789898491992 | Os 100               | ação, mistério     | 2014 | 15,90 | Kass Morgan                                  | 5     | 
| 9789896687403 | Verity               | thriller           | 2018 | 15,95 | Colleen Hoover                               | 15    | 
| 9789892352749 | Morte no Nilo        | mistério           | 2022 | 9,90  | Agatha Christie                              | 20    | 
| 9789897841859 | Aquorea              | fantasia, romance  | 2021 | 17,50 | M.G. Ferrey                                  | 7     | 
| 9789892341989 | Um de nós mente      | thriller, mistério | 2017 | 18,90 | Karen M. McManus                             | 2     | 
| 9789722365598 | Harry Potter         | fantasia, mistério | 2020 | 14,30 | J.K. Rolling                                 | 5     | 
| 9789720043818 | Divergente           | ação               | 2011 | 16,60 | Veronica Roth                                | 10    | 
| 9789899039216 | Heartstopper         | romance            | 2021 | 14,30 | Alice Oseman                                 | 3     | 
| 9789896688493 | Principe Cruel       | fantasia           | 2018 | 19,95 | Holly Black                                  | 20    | 
| 9789898626912 | Quando a neve cai    | romance            | 2014 | 17,80 | John Green,  Maureen Johnson, Lauren Myracle | 13    | 
| 9789898800572 | Amor Cruel           | romance            | 2015 | 15,95 | Colleen Hoover                               | 15    | 
| 789897772559  | Caçadores de Sombras | ação               | 2007 | 17,95 | Cassandra Clare                              | 20    | 
| 9789722348508 | Maze Runner          | ação, aventura     | 2009 | 19,90 | James Dashner                                | 8     | 

#### Cliente
| ID | nome    | email               |
| -- | ------- | ------------------- |
| 1  | Sofia   | sofia01@gmail.com   |
| 2  | Miguel  | miguel02@gmail.com  |
| 3  | Mafalda | mafalda03@gmail.com |
| 4  | Filipa  | filipa04@gmail.com  |
| 5  | João    | joao05@gmail.com    |
| 6  | Diogo   | diogo06@gmail.com   |
| 7  | Inês    | ines07@gmail.com    |
| 8  | Daniel  | daniel08@gmail.com  |
| 9  | Joana   | joana09@gmail.com   |
| 10 | Luísa   | luisa10@gmail.com   |
| 11 | Rui     | rui11@gmail.com     |

#### Armazém
| nome | morada |
| ---- | ------ |
| Porto Livros | Rua do Leitor 345 |
| Lisboa Livros | Rua do Escritor 543 |

#### Compra
| nrCompra | dataEnvio | dataReceção |
| -------- | --------- | ----------- |
| 1 | 04/06/2022 | 13/06/2022 |
| 2 | 04/06/2022 | 13/06/2022 |
| 3 | 04/06/2022 | 13/06/2022 |
| 4 | 04/06/2022 | 13/06/2022 |
| 5 | 05/06/2022 | 14/06/2022 |
| 6 | 05/06/2022 | 14/06/2022 |
| 7 | 05/06/2022 | 14/06/2022 |
| 8 | 06/06/2022 | 15/06/2022 |
| 9 | 06/06/2022 | 15/06/2022 |
| 10 | 07/06/2022	| 16/06/2022 |
| 11 | 07/06/2022	| 16/06/2022 |
| 12 | 08/06/2022	| 17/06/2022 |
| 13 | 08/06/2022	| 17/06/2022 |
| 14 | 09/06/2022	| 18/06/2022 |
| 15 | 10/06/2022	| 19/06/2022 |
| 16 | 11/06/2022	| 20/06/2022 |
| 17 | 11/06/2022	| 20/06/2022 |
| 18 | 12/06/2022	| 21/06/2022 |
| 19 | 12/06/2022	| 21/06/2022 | 
| 20 | 12/06/2022	| 21/06/2022 |
| 21 | 13/06/2022	| 22/06/2022 |
| 22 | 13/06/2022	| 22/06/2022 |
| 23 | 14/06/2022	| 23/06/2022 |
| 24 | 15/06/2022	| 24/06/2022 |
| 25 | 15/06/2022	| 24/06/2022 |
| 26 | 01/07/2022	| 11/07/2022 |
| 27 | 01/07/2022	| 11/07/2022 |
| 28 | 02/07/2022	| 12/07/2022 |
| 29 | 03/07/2022	| 13/07/2022 |
| 30 | 03/07/2022	| 13/07/2022 |


- Associações 1:N
#### Compra(CLIENTE, LIVRO) 1:N
- chave primária: ID
- chave estrageira: #ID --> Cliente

#### Livro 
| nrSerie       | titulo               | genero             | ano  | preco | nomeAutor                                    | stock | #ID --> Cliente |
| ------------- | -------------------- | ------------------ | ---- | ----- | -------------------------------------------- | ----- | --------------- |
| 9789899096424 | A hipótese do Amor   | romance            | 2022 | 17,50 | Ali Hazelwood                                | 10    | 1, 4, 5, 11     |
| 9789898491992 | Os 100               | ação, mistério     | 2014 | 15,90 | Kass Morgan                                  | 5     | 2, 10           |
| 9789896687403 | Verity               | thriller           | 2018 | 15,95 | Colleen Hoover                               | 15    | 3               |
| 9789892352749 | Morte no Nilo        | mistério           | 2022 | 9,90  | Agatha Christie                              | 20    | 3               |
| 9789897841859 | Aquorea              | fantasia, romance  | 2021 | 17,50 | M.G. Ferrey                                  | 7     | 6, 8, 9         |
| 9789892341989 | Um de nós mente      | thriller, mistério | 2017 | 18,90 | Karen M. McManus                             | 2     | 7               |
| 9789722365598 | Harry Potter         | fantasia, mistério | 2020 | 14,30 | J.K. Rolling                                 | 5     | 1, 7            |
| 9789720043818 | Divergente           | ação               | 2011 | 16,60 | Veronica Roth                                | 10    | 4               |
| 9789899039216 | Heartstopper         | romance            | 2021 | 14,30 | Alice Oseman                                 | 3     | 11              |
| 9789896688493 | Principe Cruel       | fantasia           | 2018 | 19,95 | Holly Black                                  | 20    | 5               |
| 9789898626912 | Quando a neve cai    | romance            | 2014 | 17,80 | John Green,  Maureen Johnson, Lauren Myracle | 13    | 1, 11           |
| 9789898800572 | Amor Cruel           | romance            | 2015 | 15,95 | Colleen Hoover                               | 15    | 11              |
| 789897772559  | Caçadores de Sombras | ação               | 2007 | 17,95 | Cassandra Clare                              | 20    | 2               |
| 9789722348508 | Maze Runner          | ação, aventura     | 2009 | 19,90 | James Dashner                                | 8     | 2, 4            |

- Associações M:N
#### Envia (ARMAZEM, LIVRO) M:N T/T
- chaves primárias: nome, morada, nrSerie
- chaves estrangeiras: #nome --> Armazém, #morada --> Armazém, #nrSerie --> Livro

#### Envia
| #nome --> Armazém | #morada --> Armazém | #nrSerie --> Livro |
| ----------------- | ------------------- | ------------------ |
| Porto Livros | Rua do Leitor 345 | 9789898491992, 9789722348508, 9789898491992, 789897772559, 9789896687403, 9789898800572, 9789892352749 |
| Lisboa Livros | Rua do Escritor 543 | 9789897841859, 9789892341989, 9789722365598, 9789720043818, 9789899039216, 978989668849, 9789898626912 |


#### Regista (ARMAZEM, COMPRA) M:N T/P
- chaves primárias: nome, morada, nrCompra
- chaves estrangeiras: #nome --> Armazém, #morada --> Armazém, #nrCompra --> Compra

#### Envia
| #nome --> Armazém | #morada --> Armazém | #nrCompra --> Compra |
| ----------------- | ------------------- | ------------------ |
| Porto Livros | Rua do Leitor 345 | 1, 3, 5, 7, 9, 11, 13, 15, 17, 19, 21, 23, 25, 27, 29 |
| Lisboa Livros | Rua do Escritor 543 | 2, 4, 6, 8, 10, 12, 14, 16, 18, 20, 22, 24, 26, 28, 30 |



