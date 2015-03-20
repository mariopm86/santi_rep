-- Concatenacion Interna --

-- solo mostrara las autores que tengan libros
select nombre_autor "Autor", count(cod_libro) "cantidad de libros"
from libro, autor
where libro.cod_autor=autor.cod.autor
group by nombre_autor;

-- muestra todos los autores (aun que tengan 0 libros)
select nombre_autor "Autor", count(cod_libro) "cantidad de libros"
from libro natural left join autor -- para forzar la tabla a la izquierda
where libro.cod_autor=autor.cod:autor
group by nombre_autor;

-- muestra todos los autores y los libros
select nombre_autor "Autor", count(cod_libro) "cantidad de libros"
from libro natural full join autor -- para forzar las dos tablas
where libro.cod_autor=autor.cod:autor
group by nombre_autor;
