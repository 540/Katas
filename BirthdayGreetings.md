# Kata BirthdayGreetings

## Objetivos

Aprender sobre arquitectura hexagonal, la cual es una buena forma para estructurar una aplicación, aislando el modelo de dominio de las apis y sistemas externos.

### Pre-requisitos

No es un ejercicio básico. Se suponen ciertos conocimientos sobre TDD, testing y refactoring.

### Forma de resolverla

Se puede resolver de dos formas:

- **Refactoring:** Partiendo del código base.
  - [Código base en Java](https://github.com/540/java-birthday-greetings-kata)
  - [Código base en PHP](https://github.com/540/php-birthday-greetings-kata)  
  - [Código base en Typescript](https://github.com/540/ts-birthday-greetings-kata)
  
- **TDD:** Arrancar desde 0 y resolverla.

### Enunciado

Escribe un programa que:
Carga un listado de empleados desde un fichero plano.
Envía felicitaciones a todos los empleados que cumplen años hoy.
El fichero plano es una secuencia de registros, separados por saltos de línea, estos son los primeros:

| last_name | first_name | date_of_birth | email               |
| --------- | ---------- | ------------- | ------------------- |
| Doe       | John       | 1982/10/08    | john.doe@foobar.com |
| Ann       | Mary       | 1975/09/11    | mary.ann@foobar.com |

El email de felicitación contiene el siguiente texto:

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

### Objetivo de la solución

La solución debería ser:

- Testable: Debería poderse testear la lógica interna sin enviar un email real.
- Flexible: Deberíamos anticipar que en el futuro la fuente de datos podría cambiar (ddbb, api). También nos anticipamos a que el cliente de email cambie y pueda ser otro sistema de email o de mensajería como Facebook, notificación push, etc.
- Correcta: Separar claramente la lógica de dominio de la de infraestructura.

### Complicación adicional

Si se quiere avanzar en la lógica de dominio, se puede tener en cuenta una regla especial para la gente que haya nacido el 29 de febrero. Se les debería mandar la felicitación el 28 de febrero, excepto en el año bisiesto, que la recibirían el 29.

## Créditos

[Kata original](http://matteo.vaccari.name/blog/archives/154)
