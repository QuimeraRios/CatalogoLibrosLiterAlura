# CatalogoLibrosLiterAlura

Se requiere realizar un catálogo de libros en el cual la persona usuaria puede registrar libros en una base de datos y recibir información sobre estos libros que ya están registrados en la base de datos. Se trabajara con las tecnologías Java, Spring Data JPA y Postgres 

## OBJETIVO:
Desarrollar un Catálogo de Libros que ofrezca interacción textual (vía consola) con los usuarios, proporcionando al menos 5 opciones de interacción. Los libros se buscarán a través de una API específica. 

## Los requisitos básicos de esta aplicación involucran cinco funcionalidades. 

1.	La primera funcionalidad es la de buscar libro por título. La persona usuaria debe ingresar el nombre del libro que desea buscar. Es una aplicación solo de consola.

2.	Van a listar los libros registrados en la base de datos.
3.	listar los autores registrados. 
4.	listar los libros por idioma. La persona usuaria tendrá que ingresar ES, EN, FR o PT para buscar el idioma del libro. 

5. Insertar o ingresar un libro nuevo

## Las dependencias a usar son:
   <dependency>
      <groupId>org.springframework.boot</groupId>
      <artifactId>spring-boot-starter-data-jpa</artifactId>
    </dependency>

    <dependency>
      <groupId>org.postgresql</groupId>
      <artifactId>postgresql</artifactId>
      <scope>runtime</scope>
    </dependency>
    <dependency>
      <groupId>org.springframework.boot</groupId>
      <artifactId>spring-boot-starter-test</artifactId>
      <scope>test</scope>
    </dependency>


# La API que vamos a consumir se llama Gutendex:  
https://gutendex.com/books/?

## Sobre Gutendex
Es una API que se basa en el proyecto Gutenberg, que es una biblioteca digital con más de 70 mil libros que se puede descargar gratis.

Requerimos  construir un catálogo de libros: que llamaremos  LiterAlura.  Y aprender a realizar solicitudes a una API de libros, a manipular datos JSON, guardarlos en una base de datos y, finalmente, a filtrar y mostrar los libros y autores de interés.



