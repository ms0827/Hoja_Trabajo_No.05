# Hoja_Trabajo_No.05

## Numpy, Pandas, Vectorización
### Presentado por: Margerys Salgado

-- Desarrollar los siguientes ejercicios y subir el Notebook actualizado a su repositorio de GitHub. 
-- El entregable debe ser el link del archivo en su repositorio, cualquier otra forma de entregable no será aceptada.

### Numpy

Ejercicio 1: Crear un conjunto de datos lineal
Crear un conjunto de datos simple que consta de una sola característica y una etiqueta de la siguiente manera:

Asigne una secuencia de números enteros del 6 al 20 (incluyendo 20) a un arreglo de NumPy llamado característica. Asigne 15 valores a un arreglo de NumPy llamado etiqueta de manera que:

etiqueta = (3) (característica) + 4

Por ejemplo, el primer valor de etiqueta debería ser:

etiqueta = (3) (6) + 4 = 22

Ejercicio 2: agregar ruido al conjunto de datos
Inserte un ruido aleatorio en cada elemento de la matriz etiqueta que ya creó.

Para ser más precisos, modifique cada valor asignado a etiqueta agregando un valor "floating-point" aleatorio diferente entre -2 y +2. No utilice broadcasting. En su lugar, cree un arreglo de ruido que tenga la misma dimensión que etiqueta.

### Pandas

Ejercicio 3: Crear un DataFrame
Cree un pandas DataFrame de 10x3 (10 filas x 3 columnas) en el que las columnas se denominen "Data Warehouse", "Python in Data Science", y "Estadística Aplicada". Llene cada una de las 30 celdas del DataFrame con un número entero aleatorio entre 0 y 100, incluyendo 100.

Despliegue lo siguiente:

1)	Todo el DataFrame
2)	Las primeras 5 filas del DataFrame
3)	Las ultimas 5 filas del DataFrame
4)	El valor en la celda de la fila # 1 de la columna "Data Warehouse"
5)	El valor en la celda de la fila # 3 de la columna "Estadistica Aplicada"
6)	Cree una cuarta columna llamada "Promedio", que se rellena con el promedio fila por fila de las otras 3 columnas ("Data Warehouse", "Python in Data Science", y "Estadistica Aplicada"). Debe de usar la funcion de Numpy para calcular el promedio.

Para completar esta parte, es útil entender los conceptos básicos de NumPy cubiertos en clase y en la sección anterior.

### Vectorización

A continuación, se le presenta un problema el cual deberá resolver de dos formas distintas.

1)	La primera es utilizando un for loop, 
2)	la segunda usando vectorización.

Luego debe de comparar el resultado de ambas implementaciones, tanto el valor resultante de la operación, como el tiempo que toma la ejecución de cada una.

Problema:
Dada una secuencia de precios históricos para una acción, y suponiendo que solo se le permite realizar una compra y una venta, ¿cuál es la ganancia máxima que se puede obtener?

Por ejemplo, dados los precios = (20, 18, 14, 17, 20, 21, 13), el beneficio máximo sería 7, de comprar a 14 y vender a 21. 

Notar que el arreglo es una secuencia, por lo tanto, no es factible solo utilizar los valores menores y mayores, ya que el valor mayor debe de estar obligatoriamente en una posición futura al menor, por eso el mejor precio de compra es 14 y no 13.

Para este ejemplo utilice el siguiente código para generar el dataset (secuencia de precios históricos), asegúrese de también incluir el "random seed" para obtener reproducibilidad.
