# Taller-Junit

# Tabla principal

| Caso de Prueba y Propósito               | Entradas de Datos | Valor Esperado | Resultado |
| ---------------------------- | ----------------- | -------------- | --------- |
| Probar la generación de fórmulas aleatorias        | N/A (Método estático)              | Una fórmula válida con 1-3 operaciones y números aleatorios              | Pasó      |
| Probar la resolución de fórmulas simples (suma)   | "5+3"              | "5+3=8"            | Pasó      |
| Probar la resolución de fórmulas simples (resta)   | "10-4"               | "10-4=6"              | Pasó      |
| 	Probar la resolución de fórmulas simples (multiplicación)   | "8*2"               | "8*2=16"              | Pasó      |
| 	Probar la resolución de fórmulas simples (división)   | "16/4"               | "16/4=4"              | Pasó      |
| Probar la resolución de fórmulas con múltiples operaciones   | "5+3*2"               | "5+3*2=11"              | Pasó      |
| Probar la resolución de fórmulas con paréntesis   | "(5+3)*2"               | "(5+3)*2=16"              | Pasó      |
| Probar la resolución de fórmulas con división por cero   | "10/0"               | Excepción de tipo ArithmeticException              | Pasó      |
| Probar la resolución de fórmulas con números negativos   | "-5+3"               | "-5+3=-2"              | Pasó      |
| Probar el manejo de fórmulas inválidas  | "5++3"               | Excepción de tipo NumberFormatException o IllegalArgumentException              | Pasó      |


# Prueba Unitaria de la Suma

| Caso de Prueba               | Entradas de Datos | Valor Esperado | Resultado |
| ---------------------------- | ----------------- | -------------- | --------- |
| Suma Normal                  | 2,3               | 5              | Pasó      |
| Suma con Numeros Negativos   | -2,3              | -5             | Pasó      |
| Suma con Numeros Positivos   | 2,3               | 5              | Pasó      |

## Suma Normal

Se asegura de que la operación básica de suma esté funcionando correctamente con números positivos. En este caso, utilizamos una prueba de unidad que emplea el método "AssertEquals" para comparar directamente el valor esperado con el resultado obtenido de la función.
![Captura de pantalla (2104)](https://github.com/DanielMateoOrellana/Taller-Junit/assets/107369011/6774b8a0-864f-44b0-ad7f-be32304f62ee)

## Suma con número negativo

Se garantiza que la función de suma maneje adecuadamente la suma de dos números negativos. En este caso, hemos creado una prueba de unidad utilizando el método "AssertEquals" para comparar directamente el valor esperado con el resultado obtenido de la función.
![Captura de pantalla (2105)](https://github.com/DanielMateoOrellana/Taller-Junit/assets/107369011/fdc3a2c9-43c5-4860-93f1-67b564d85e8d)


## Suma con número positivo

Se asegura de que la función de suma retorne el valor correcto al sumar dos números positivos. En esta prueba de unidad, utilizamos el método "AssertEquals" para comparar directamente el valor esperado con el resultado obtenido de la función.
![Captura de pantalla (2107)](https://github.com/DanielMateoOrellana/Taller-Junit/assets/107369011/b0d04889-c282-460c-a972-cc4002ba4049)

# Prueba Unitaria de la Resta

| Caso de Prueba               | Entradas de Datos | Valor Esperado | Resultado |
| ---------------------------- | ----------------- | -------------- | --------- |
| Resta Normal                  | 4,3               | 1              | Pasó      |
| Resta con Numeros Negativos   | -2,3              | -1             | Pasó      |
| Resta con Numeros Positivos   | 4,3               | 1              | Pasó      |

## Resta Normal

Se asegura de que la operación básica de resta funcione correctamente con números positivos. Al restar dos números, se espera obtener un resultado específico. Utilizaremos el método AssertEquals para comparar directamente el valor esperado con el resultado obtenido de la función de resta.
![Captura de pantalla (2108)](https://github.com/DanielMateoOrellana/Taller-Junit/assets/107369011/002a3662-a46c-4ca1-82d9-1d3993d131cf)

## Resta con Numeros Negativos

Se asegura de que la función de resta maneje correctamente la resta de dos números negativos. Al restar un número negativo con otro número negativo, se espera obtener un resultado específico. Utilizaremos el método AssertEquals para comparar directamente el valor esperado con el resultado obtenido de la función de resta.
![Captura de pantalla (2109)](https://github.com/DanielMateoOrellana/Taller-Junit/assets/107369011/bc4d6090-3ec7-42ef-afa9-813c5dec1fb0)

## Resta con numeros Positivos 

Se asegura de que la función de resta retorne el valor correcto al restar un número positivo con otro número positivo. La resta de dos números positivos debe dar un resultado específico. Utilizaremos el método AssertEquals para comparar directamente el valor esperado con el resultado obtenido de la función de resta.
![Captura de pantalla (2110)](https://github.com/DanielMateoOrellana/Taller-Junit/assets/107369011/98180b46-ddb1-4942-8821-947f954c179d)

# Prueba Unitaria de la Multiplicacion 
   
| Caso de Prueba                                       | Entradas de Datos | Valor Esperado | Resultado |
| ---------------------------------------------------- | ----------------- | -------------- | --------- |
| Multiplicacion Normal                                | 5,5               | 25             | Pasó      |
| Multiplicacion entre Numeros positivos y negativos   | -2,3              | -6             | Pasó      |
| Multiplicacion entre dos numeros negativos        | -4,-6             | 24             | Pasó      |
| Multiplicacion por 0                                 | 5,0               | 0              | Pasó      |

## Multiplicacion Normal 

Se asegura que la operacion basica de la multiplicacion funcione correctamente con los numeros positivos. Al multiplicar ambos numeros se espera obtener un resultado especifico. Se utilizara el metodo AsserEquals para comparar el resultado obtenido con el especificado anteriormente.

![image](https://github.com/DanielMateoOrellana/Taller-Junit/assets/136995519/a78a4021-4786-4edc-acd3-22ee4a154279)

## Multiplicacion entre Numeros positivos y negativos

Se asegura que la operacion entre numeros negativos y positivos de la multiplicacion funcione correctamente. Al multiplicar ambos numeros (negativo y positivos) se espera obtener un resultado especifico. Se utilizara el metodo AsserEquals para comparar el resultado obtenido con el especificado anteriormente.

![image](https://github.com/DanielMateoOrellana/Taller-Junit/assets/136995519/bfb0c3e4-6480-4962-9445-827bfac116b4)

## Multiplicacion entre dos numeros negativos

Se asegura que la operacion entre numeros negativos de la multiplicacion funcione correctamente. Al multiplicar ambos numeros(ambos negativos) se espera obtener un resultado especifico. Se utilizara el metodo AsserEquals para comparar el resultado obtenido con el especificado anteriormente.

![image](https://github.com/DanielMateoOrellana/Taller-Junit/assets/136995519/019bece4-aef4-4653-b95d-e8e00df5be4c)

## Multiplicacion por 0

Se asegura que la operacion entre el numero cero y cualquier otro numero ya sea positivo o negativo funcione correctamente. Al multiplicar ambos numeros se espera obtener un resultado especifico. Se utilizara el metodo AsserEquals para comparar el resultado obtenido con el especificado anteriormente.

![image](https://github.com/DanielMateoOrellana/Taller-Junit/assets/136995519/15ea5b13-5c56-4cad-aaf4-bce242c32689)

# Prueba Unitaria de la División 
   
| Caso de Prueba                                       | Entradas de Datos | Valor Esperado | Resultado |
| ---------------------------------------------------- | ----------------- | -------------- | --------- |
| División básica                                | 20,4              | 5             | Pasó      |
| División entre 0   | 20, 5              | Error            | Pasó      |
| División de numero negativo por positivo        | -10, 5             | -2             | Pasó      |

## División Básica

Se asegura que se pueda realizar una división básica, esperando un resultado exacto, dividiendo 20 para 4, que debería ser igual a 5.

![image](https://github.com/DanielMateoOrellana/Taller-Junit/assets/107244270/d1c14eef-d08b-4ab3-ac07-f2d1711f45ff)

## División entre 0

Se asegura que se pueda dividir un numero entre 0, lo cual debería arrojar un error, y por eso usamos assertThrows().

![image](https://github.com/DanielMateoOrellana/Taller-Junit/assets/107244270/b18f47f8-1062-462f-b0e9-e0348b54e04c)

## División de numero negativo por positivo

Se asegura que se pueda dividir un número negativo por uno positivo, se espera un resultado exacto, dividiendo –10 para 5 el resultado debería ser –2.

![image](https://github.com/DanielMateoOrellana/Taller-Junit/assets/107244270/edabc5d0-9e0b-455c-961a-2dcadcc11f64)
