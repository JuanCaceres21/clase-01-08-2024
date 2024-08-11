# Clase 29/08/2024 introducción al control digital 

En esta clase se vieron las diferencias entre hacer control de forma análogo y hacer control de forma digital, viendo cada una de sus ventajas y desventajas, y por último viendo como es el funcionamiento de un sistema controlado por procesamiento digital.
## 1. señales análogas y digitales
Podemos diferenciar señales analógicas y digitales de una manera sencilla, las señales analógicas pueden tomar cualquier valor dentro de un rango determinado, y las señales digitales, solo pueden tomar dos valores, esto en referencia a el 1 o 0 que entiende una computadora digital.

## 2. Ventajas del control digital
El control digital, posee en si tres ventajas por encima del control análogo:

### 2.1 Implementación
Un sistema digital, al correr directamente en una computadora, esto hace que en caso de cometer un error o hacer una modificación se más fácil cambiar cualquier parámetro en código, en lugar de cambiar elementos físicos de la computadora como se haría en el control análogo.
###2.2 Flexibilidad
En el caso de las computadoras análogas estas se construyen teniendo en mente la función que van a desempeñar, con esto en cuenta podemos decir que un sistema análogo construido para una planta en específico, no va a funcionar en una planta diferente. El control digital permite ejecutar un sistema u otro, esto otorga la posibilidad de usar una misma computadora en distintas plantas de control.
### 2.3 Costos
Ya que la implementación del control digital es tan simple como ejecutar código en una computadora, este en si es el único elemento que se requiere para esta tarea, abaratando costos y reduciendo la cantidad de elementos necesarios para la implementación.

## 3 Conversión análoga digital
La conversión análoga-digital se compone de 3 pasos principales: el muestreo, la cuantización y la codificación.

###3.1 Muestreo
El muestreo lo podemos definir como la cantidad de tiempo que tarda una computadora en tomar un valor de una señal análoga, entre más alta la tasa de muestro o más bajo el tiempo de muestreo se van a tomar más datos de la señal, por lo tanto, tendremos una señal digitalmente más fiel a la original.

### 3.2 Cuantización
La cuantización consiste en tomar los datos de la señal análoga y darles un valor que se guardara en una variable.

💡**ejemplo1:** si tenemos una señal sinusoidal, y el tiempo de muestreo de  pi/2, los valores guardados serán:

$$valores=[0,1,0,-1,0]$$

### 3.3 Codificación
Ya que tenemos los valores de la señal, estos son traducidos a lenguaje de maquina es decir comúnmente en binario, por lo tanto, el valor máximo de la señal, idealmente debería corresponder al valor máximo que permitan los bits del sistema.

## 4. conversión digital análoga

como ya sabemos el mundo se rige por señales análogas, por la tanto debemos pasar los datos contenidos en un sistema digital, a señales análogas para así controlar variables del mundo real, esto se puede conseguir por medio de dos circuitos diferentes.

### 4.1 Método de resistencias ponderadas:

[Circuito por resistencias ponderadas](C:\Users\juang\Desktop\8vo semestre\control digital\imagen1.PNG)

$$salida=\frac{Entrada1}{R}+\frac{Entrada2}{2R}+\frac{Entrada3}{4R}+\frac{Entrada4}{8R}+\frac{Entrada5}{16R}$$

### 4.2 Método de red escalera

[Circuito por red de escalera](C:\Users\juang\Desktop\8vo semestre\control digital\imagen2.PNG)

$$salida=-(/frac{Rf}{R})(\frac{Entrada1}{16}+\frac{Entrada2}{8}+\frac{Entrada3}{4}+\frac{Entrada4}{2})$$





