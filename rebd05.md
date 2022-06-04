# C5: SQL

USE `test`;

CREATE TABLE `cliente` (
`id` int(2),
`nome` varchar(7),
`email`varchar(19)
);

INSERT INTO cliente (id, nome, email)
VALUES 
(1, 'Sofia', 'sofia01@gmail.com'),
(2, 'Miguel', 'miguel02@gmail.com'),
(3, 'Mafalda', 'mafalda03@gmail.com'),
(4, 'Filipa', 'filipa04@gmail.com'),
(5, 'João', 'joao05@gmail.com'),
(6, 'Diogo', 'diogo06@gmail.com'),
(7, 'Inês', 'ines07@gmail.com'),
(8, 'Daniel', 'daniel08@gmail.com'),
(9, 'Joana', 'joana09@gmail.com'),
(10, 'Luísa', 'luisa10@gmail.com'),
(11, 'Rui', 'rui11@gmail.com');

CREATE TABLE `livro` (
`nrSerie` int(3),
`titulo` varchar(20),
`genero` varchar(20),
`ano` int(4),
`preco` int(2),
`nomeAutor` varchar(45),
`stock` varchar(2)
);

INSERT INTO livro (nrSerie, titulo, genero, ano, preco, nomeAutor, stock)
VALUES 
(424, 'A hipótese do Amor', 'romance', 2022, 17, 'Ali Hazelwood', 10),
(992, 'Os 100', 'ação/mistério', 2014, 16, 'Kass Morgan', 5),
(403, 'Verity', 'thriller', 2018, 16, 'Colleen Hoover', 15),
(749, 'Morte no Nilo', 'mistério', 2022, 10, 'Agatha Christie', 20),
(859, 'Aquorea', 'fantasia/romance', 2021, 17, 'M.G. Ferrey', 7),
(989, 'Um de nós mente', 'thriller/mistério', 2017, 19, 'Karen M. McManus', 2),
(598, 'Harry Potter', 'fantasia/mistério', 2020, 14, 'J.K. Rolling', 5),
(818, 'Divergente', 'ação', 2011, 16, 'Veronica Roth', 10),
(216, 'Heartstopper', 'romance', 2021, 14, 'Alice Oseman', 3),
(493, 'Principe Cruel', 'fantasia', 2018, 20, 'Holly Black', 20),
(912, 'Quando a neve cai', 'romance', 2014, 18, 'John Green/Maureen Johnson/Lauren Myracle', 13),
(572, 'Amor Cruel', 'romance', 2015, 16, 'Colleen Hoover', 15),
(559, 'Caçadores de Sombras', 'ação', 2007, 18, 'Cassandra Clare', 20),
(508, 'Maze Runner', 'ação/aventura', 2009, 20, 'James Dashner', 8);

CREATE TABLE `armazem` (
`nome` varchar(15),
`morada` char(20)
);

INSERT INTO armazem (nome, morada)
VALUES 
('Porto Livros', 'Rua do Leitor 345'),
('Lisboa Livros', 'Rua do Escritor 543');

CREATE TABLE `compra` (
`nrCompra` int(2),
`dataEnvio` varchar(10),
`dataRececao` varchar(10)
);

INSERT INTO compra (nrCompra, dataEnvio, dataRececao)
VALUES 
(1, '04/06/2022', '13/06/2022'),
(2, '04/06/2022', '13/06/2022'),
(3, '04/06/2022', '13/06/2022'),
(4, '04/06/2022', '13/06/2022'),
(5, '05/06/2022', '14/06/2022'),
(6, '05/06/2022', '14/06/2022'),
(7, '05/06/2022', '14/06/2022'),
(8, '06/06/2022', '15/06/2022'),
(9, '06/06/2022', '15/06/2022'),
(10, '07/06/2022', '16/06/2022'),
(11, '07/06/2022', '16/06/2022'),
(12, '08/06/2022', '17/06/2022'),
(13, '08/06/2022', '17/06/2022'),
(14, '09/06/2022', '18/06/2022'),
(15, '10/06/2022', '19/06/2022'),
(16, '11/06/2022', '20/06/2022'),
(17, '11/06/2022', '20/06/2022'),
(18, '12/06/2022', '21/06/2022'),
(19, '12/06/2022', '21/06/2022'),
(20, '12/06/2022', '21/06/2022'),
(21, '13/06/2022', '22/06/2022'),
(22, '13/06/2022', '22/06/2022'),
(23, '14/06/2022', '23/06/2022'),
(24, '15/06/2022', '24/06/2022'),
(25, '15/06/2022', '24/06/2022'),
(26, '01/07/2022', '11/07/2022'),
(27, '01/07/2022', '11/07/2022'),
(28, '02/07/2022', '12/07/2022'),
(29, '03/07/2022', '13/07/2022'),
(30, '03/07/2022', '13/07/2022');
