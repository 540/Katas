# String Calculator

## Antes de comenzar

* Intenta no leer el enunciado completo antes de empezar, ve leyendo poco a poco mientras lo resuelves.
* Haz sólo una tarea a la vez. El truco está en aprender a trabajar de forma incremental.
* Asegúrate de testear únicamente las entradas correctas. No es necesario testear las entradas incorrectas para esta kata.

## Funcionalidad deseada

1. Crea una String Calculator con el método: int Add(string numbers)
    * El parámetro del método puede contener 0, 1 o 2 números y devolverá su suma (para un string vacío devolverá 0). Por ejempo: "" o "1" o "1,2"
    * Compieza por un test simple para un string vacío y luego para 1 y 2 números.
    * Recuerda resolver el problema de la manera más simple posible para que te fuerce a escribir las pruebas que aún no se te habían ocurrido.
    * Recuerda refactorizar después de conseguir pasar cada test.
2. Permite al metodo "Add" manejar cualquier cantidad de números.
3. Permite al método "add" manejar saltos de línea entre números en lugar de usar comas.
    * La siguiente entrada es correcta: "1\n2,3" (el resultado será 6)
    * La siguiente entrada NO es correcta: "1,\n" (no hace falta que la pruebes, es simplemente para clarificar)
4. Soporta diferentes delimitadores
    * Para cambiar un delimitador, el comienzo del string debe contener una línea separada que sea como esta: "//[delimitador]\n[números...]". Por ejemplo: "//;\n1;2" debe dar como resultado 3 donde el delimitador por defecto es ";".
    * La primera línea es opcional. Todos los escenarios existentes hasta ahora, deben estar soportados.
5. Llamar al método "Add" con números negativos deberá lanzar una excepción con el texto "negativos no soportados" y el número negativo que ha sido pasado. Si hay múltiples números negativos, muestra todos ellos en el mensaje de la excepción.
6. Los numeros mayores de 1000 deben ser ignorados. Por ejemplo "2,1001" dará como resultado 2.
7. Los delimitadores pueden ser de cualquier longitud con el siguiente formato: "//[delimiter]\n". Por ejemplo: "`//[***]\n1***2***3`" debe dar como resultado 6.
8. Permite múltiples delimitadores de la siguiente manera: "//[delim1][delim2]\n". Por ejemplo: "`//[*][%]\n1*2%3`" debe dar como resultado 6.
9. Asegúrate de que puedes manejar delimitadores de cualquier longitud mayor de un caracter.

## Créditos

[Kata original](http://osherove.com/tdd-kata-1/)
