# CatalogoLibrosLiterAlura

Se requiere realizar un catálogo de libros en el cual la persona usuaria puede registrar libros en una base de datos y recibir información sobre estos libros que ya están registrados en la base de datos. Se trabajara con las tecnologías Java, Spring Data JPA y Postgres 

## OBJETIVO:
Desarrollar un Catálogo de Libros que ofrezca interacción textual (vía consola) con los usuarios, proporcionando al menos 5 opciones de interacción. Los libros se buscarán a través de una API específica. 

## Los requisitos básicos de esta aplicación involucran cinco funcionalidades. 

1.	La primera funcionalidad es la de buscar libro por título. La persona usuaria debe ingresar el nombre del libro que desea buscar. Es una aplicación solo de consola. No deben preocuparse por el frontend. 
Entonces, la persona usuaria busca un libro por su nombre, por ejemplo: Pride (Orgullo). Un libro en inglés. Es lo que busco. Vamos a ver. Y, en este caso, la aplicación debe ir a la API, buscar las información sobre este libro y registrarlo en la base de datos. Aquí tenemos el resultado de la operación. 
Título Pride and Prejudice (Orgullo y Prejuicio). Es un libro de Jane Austen. Es importante notar que primero se ve el apellido del autor o de la autora. Y después su primer nombre. El idioma es EN, que es inglés. Y el número de descargas es 6493. Ahora ya tienen otro libro en su base de datos. Y, a partir de esto, pueden comenzar a hacer operaciones con la base de datos.

Los cuatro métodos que siguen son métodos que trabajan con la base de datos. 
2.	Van a listar los libros registrados en la base de datos, cuando elijan el número 2. Aquí tenemos varios libros. Tenemos Don Quixote (Don Quijote), Emma, un diccionario de la lengua portuguesa, Pride and Prejudice (Orgullo y Prejuicio), Romeo and Juliet (Romeo y Julieta) y un libro de filosofía, también de Nietzsche. 
3.	Podemos listar los autores registrados. Aquí tenemos todos los autores registrados en la plataforma. Pueden ver que Jane Austen solo aparece una vez, pero con dos libros. También podemos listar los autores vivos en un determinado año. Por ejemplo, el año de 1600. Es un año en que Cervantes y Shakespeare estaban vivos. No sé si pueden ver a los dos. 
4.	También se puede listar los libros por idioma. Aquí tenemos una opción más simple. Pero pueden implementar opciones más elegantes para esta funcionalidad. Aquí elegimos una más simple. La persona usuaria tendrá que ingresar ES, EN, FR o PT para buscar el idioma del libro. Vamos a buscar por ES. Y solo tenemos un libro en español en nuestra base de datos hasta ahora.

También es importante manejar la posibilidad de que la persona usuaria escriba algo que no existe en el catálogo de la API. Por ejemplo, ingrese el nombre del libro que desea buscar. La persona usuaria puede escribir algo sin sentido, como Q, O, Q, O, Q, O, Q, O, Q, O, E. No podrá encontrar nada. El libro no fue encontrado. Es importante mostrar a la persona usuaria este mensaje de que el libro no fue encontrado. 

5. Además, la persona usuaria tampoco debe ser capaz de insertar el mismo libro dos veces en la base de datos. Por ejemplo, si intento ingresar otra vez PRIDE, buscará por PRIDE & PREJUDICE (Orgullo y Prejuicio). Espero. No puede insertar el mismo libro más de una vez.

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


# La API que vamos a consumir se llama Gutendex este es un ejemplo en el uso:  
https://gutendex.com/books/?

Es una API que se basa en el proyecto Gutenberg, que es una biblioteca digital con más de 70 mil libros que pueden descargar gratis. La documentación está en inglés, pero pueden usar esta funcionalidad aquí de Google Chrome y cambiarla a español si no les gusta leer en inglés. Y podemos leer aquí toda la documentación. Es importante tener acceso a esta documentación, leerla lo mejor que puedan para saber cómo implementar sus métodos, cómo hacer una lista de libros, los datos del autor, la fecha de su nacimiento, cómo se presentará este dato a ustedes, cómo trabajar con estos datos.

Requerimos  construir un catálogo de libros: que llamaremos  LiterAlura.  Y aprender a realizar solicitudes a una API de libros, a manipular datos JSON, guardarlos en una base de datos y, finalmente, a filtrar y mostrar los libros y autores de interés.



