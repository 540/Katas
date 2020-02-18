# Kata BirthdayGreetings

## Objetivos

Aprender sobre arquitectura hexagonal, la cual es una buena forma para estructurar una aplicación, aislando el modelo de dominio de las apis y sistemas externos.

## Pre-requisitos

No es un ejercicio básico. Se suponen ciertos conocimientos sobre TDD, testing y refactoring.

## Formatos

Se puede resolver de dos formas:

- Refactoring: Partiendo del código base.
  - [Código base en java](https://github.com/540/java-birthday-greetings-kata)
  
- Practicando TDD: Arrancar desde 0 y resolverla.

## Enunciado

Escribe un programa que:
Carga un listado de emplaedos desde un fichero plano.
Envía agradecimientos a todos los empleados que cumplen años hoy.
El fichero plano es una secuencia de registros, separados por saltos de línea, estos son los primeros:
last_name, first_name, date_of_birth, email
Doe, John, 1982/10/08, john.doe@foobar.com
Ann, Mary, 1975/09/11, mary.ann@foobar.com

El email de agradecimiento contiene el siguiente texto:
```
Subject: Happy birthday!

Happy birthday, dear John!
```

Con el nombre del empleado sustituido por "John"

El programa debería estar invocado de una manera del tipo:

```
    ...
    BirthdayService birthdayService = new BirthdayService(employeeRepository, emailService);
    birthdayService.sendGreetings(today());
    ....
```

Ten en cuenta que a birthdayService se le inyectan los colaboradores. Idealmente el código de dominio nunca debería hacer new. El new se usa fuera para construir una agregación de objetos que colaboran entre ellos.

## Solución

## Créditos

[Kata original](http://matteo.vaccari.name/blog/archives/154)
