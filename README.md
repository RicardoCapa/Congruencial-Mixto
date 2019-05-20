# Congruencial-Mixto
Por Angel Capa Curso: "A

Congruencial Mixto
Los generadores congruenciales lineales generan una secuencia de números pseudoaleatorios en la cual el próximo número pseudoaleatorio es determinado a partir del último número generado, es decir, el número pseudoaleatorio Xn+1 es derivado a partir del número pseudoaleatorio Xn.
La relación de recurrencia para el generador congruencial mixto es Xn+1 =(a Xn+c) mod m, en donde: 
      • X0 = es la semilla 
      • a =el multiplicador 
      • c = constante aditiva 
      • m = el modulo (m > X0, a,c)
      • X0, a, c >0 
Esta relación de recurrencia nos dice que Xn+1 es el residuo de dividir a Xn+c entre el modulo. Lo anterior significa que los valores posibles de Xn+1 son 0,1,2,3 ....m-1, es decir, m representa el número posible de valores diferentes que pueden ser generados. 
Para ello se ha implementado un programa en java para calcular el congruencial mixto.
Para esto se tomo en cuenta las siguientes condiciones:
• a debe ser un número impar, no divisible ni por 3 ni por 5, a continuación tenemos el método desarrollado en java para esta condición.









• Xo el valor de la semilla es irrelevante
• c usualmente puede ser cualquier constante.
• m debe ser el número entero primo más grande y a su vez que sea menor que p^d donde p = 2 y d = 32 para una computadora en sistema binario.
-Primero se comprueba que el numero sea primo con el siguiente método implementado en java.











- Luego controlamos que sea menor que  p^d donde p = 2 y d = 32 para una computadora en sistema binario.


• Por ultimo establecemos las condiciones iniciales de X0, a, c  >0, además de m > a, Xo, c. Usando el condicional if queda de la siguiente manera.




Una vez establecidas estas condiciones se puede desarrollar el programa.
1. Primero declaramos las variables necesarias.








2. Luego declaramos un ciclo for para la generación de números, básicamente dentro de este ciclo for se realizara la aplicación de la formular para congruencial mixto ((a*xo)+c)/m, además se usa una variable de tipo String llamada cad para concatenar la respuesta .












3. Una vez realizado el proceso se procede a presentar los resultados con la ayuda de JoptionPane.showMessageDialog.







4. A continuación se realizara una demostración del programa en ejecución con el resultado obtenido.
    • Primero ingresamos el valor de la semilla en este caso sera de 5.
      








    • Luego ingresamos el valor del multiplicador este debe ser impar, además de no ser divisible para 3 y 5 en este caso ingresamos el valor de 13.  






    • A continuación ingresamos el valor de c (constante aditiva), le damos un valor de 17.








    • Finalmente ingresamos el valor de la semilla, el cual tuvo un valor de 37 siedo impar y menor a  p^d donde p = 2 y d = 32.







    • A continuación presentamos los resultados obtenidos.
      
