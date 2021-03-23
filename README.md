# Laboratorio 7: Teorema de Thévenin
Integrantes: Caillamara Leonardo, González Ariel
## 1. OBJETIVOS

### Objetivo general:
* Demostrar el funcionamiento del teorema de Thévenin mediante mediante su aplicación en un circuito resistivo.
### Objetivos específicos:
*	Aplicar el teorema de Thévenin para una mejor comprensión de su uso en distintos circuitos.
*	Comparar valores obtenidos antes y después de la aplicación del teorema tanto en simulación como en cálculos. 

## 2. MARCO TEÓRICO

# Teorema de Thévenin

![](https://github.com/ArielAGH/Laboratorio7/blob/main/Img/MarcoTeorico1.png)

El teorema de Thévenin recibe su nombre gracias al ingeniero en telégrafos León Charles Thévenin en 1883.

Este teorema nos indica que: Cualquier circuito lineal abierto en los terminales a y b, por más complejo que este sea, es posible reemplazarlo por un circuido en el que consta de una fuente de voltaje y una resistencia en serie, unidas a dichos terminales a y b.

El voltaje de dicha fuente recibe el nombre de voltaje de Thévenin (Vth) y el nombre de la resistencia como resistencia de Thévenin (Rth)

Este teorema es utilizado cuando en un circuito existe una carga variable ( llamada resistencia de carga RL ) en un circuito fijo, ya sea un resistor u otro circuito cuyo valor varíe. Por ejemplo, cuando se pone a cargar distintos dispositivos electrónicos a un solo cargador o cuando se conectan distintos electrodomésticos a un tomacorriente. Los circuitos fijos al contrario de los variables estos no varían sus valores y son los que se van a reducir. Un ejemplo claro de estos circuitos es la red eléctrica del hogar. 

![](https://github.com/ArielAGH/Laboratorio7/blob/main/Img/MarcoTeorico2.png)

Aunque los electrodomésticos todos juntos son tomados como circuitos variables, individualmente representan a un circuito fijo como es el caso de un televisor Smart cuyo consumo es distinto a uno de los años 90’s pero individualmente son circuitos con un consumo fijo. 

![](https://github.com/ArielAGH/Laboratorio7/blob/main/Img/MarcoTeorico3.png)

Método de solución:

Para poder aplicar este teorema es necesario tener conocimiento varios métodos estudiados previamente como lo son: resolución de circuitos por medio de mallas y nodos, superposición, resistencia equivalente, etc.

Primero se calcula la resistencia de Thévenin apagando todas las fuentes y al igual que en superposición a las fuentes de voltaje se las remplaza por un corto circuito, mientras que las de corriente se las reemplaza por un circuito abierto. A final se determina la resistencia equivalente en los terminales donde va conectada la resistencia de carga.

Luego se encienden las fuentes para realizar el análisis del circuito a transformar y determinar el valor del voltaje (Vth) entre los terminales a – b donde se ubica RL. 

## 3. EQUIPOS Y MATERIALES

* **TinkerCad:** Programa online de simulación de circuitos.
* **Protoboard:** Es una placa de pruebas en la que se pueden insertar elementos electrónicos y cables con los que se arman circuitos sin la necesidad de soldar ninguno de los elementos.
* **Resistencias eléctricas:** Elemento eléctrico que se opone al paso de corriente.
* **Cables puente:** Cables de ayuda para realizar conexiones provisionales.
* **Multímetro:** Es un instrumento analógico o digital portátil que se usa para medir directamente magnitudes eléctricas.
* **Batería o fuente energética:** Dispositivo que provee energía a un circuito al cual es conectado.

## 4. PROCEDIMIENTO

4.1. Arme el circuito de la figura en TinkerCad

![](https://github.com/ArielAGH/Laboratorio7/blob/main/Img/Circuito.png)

4.2. Mida el voltaje y la corriente en el resistor R5, anote los resultados en la tabla 5.2.

![](https://github.com/ArielAGH/Laboratorio7/blob/main/Img/VoltajeCircuitoCompleto.png)

![](https://github.com/ArielAGH/Laboratorio7/blob/main/Img/CorrienteCircuitoCompleto.png)


4.3. Desconecte el resistor R5 y mida el voltaje en el circuito abierto. Anote el valor medido en la tabla 5.1.

![](https://github.com/ArielAGH/Laboratorio7/blob/main/Img/VoltajeDeThevenin.png)

4.4. Anule el efecto de las fuentes de alimentación. Desconecte R5 y desde el circuito abierto resultante mida la resistencia equivalente. Anote el valor medido en la tabla 5.1.

![](https://github.com/ArielAGH/Laboratorio7/blob/main/Img/ResistenciaDeThevenin.png)

4.5. Implemente el circuito equivalente de Thévenin, agregue el resistor R5 y mida la corriente y el voltaje en el mismo, anote los resultados en la tabla 5.2.

![](https://github.com/ArielAGH/Laboratorio7/blob/main/Img/CorrienteCircuitoThevenin.png)

![](https://github.com/ArielAGH/Laboratorio7/blob/main/Img/VoltajeCircuitoThevenin.png)

## 5. TABLAS DE MEDICIÓN Y CÁLCULOS

![](https://github.com/ArielAGH/Laboratorio7/blob/main/Img/Tabla51.png)

![](https://github.com/ArielAGH/Laboratorio7/blob/main/Img/ErroresTabla51.png)

![](https://github.com/ArielAGH/Laboratorio7/blob/main/Img/Tabla52.png)

![](https://github.com/ArielAGH/Laboratorio7/blob/main/Img/ErroresTabla52.png)

Los cálculos respectivos están en la carpeta denominada Cálculos y para el cálculo del error en cada malla se usa la siguiente fórmula para los casos respectivos.

![](https://github.com/KevinCaillamara/Laboratorio_2/blob/main/Im%C3%A1genes/formula_error.png)

## 6. ANÁLISIS DE RESULTADOS

De las observaciones registradas en la tabla de resultados es posible notar que no existe una variación significativa en los resultados obtenidos, lo que comprueba la efectividad de la aplicación del teorema.  

Al momento de realizar la simulación con el teorema de Thévenin  ya aplicado el propio simulador  no admitió el valor de  5.06 para la fuente de voltaje (Vth) lo que  provoca la variacion entre los valores medidos  tanto en corriente como en voltaje.

## 7. CONCLUSIONES

En conclusión, se pudo observar que el teorema de Thévenin si cumple con su enunciado y es de gran ayuda para el análisis de circuitos complejos con resistencia de carga variable ya que los transforma en un circuito serie de dos resistencias, siendo una de estas la resistencia de carga (RL), también el cálculo de las magnitudes de  la resistencia de carga  se ven facilitados porque resultará sencillo aplicar la ley de ohm en RL a comparación de realizar el respectivo análisis en el circuito original.

## 8. BIBLIOGRAFÍA

* Durán, J. (2012). *Electrotecnia*. Barcelona: Editorial Lexus.
* Fraile, J. (2012). *Circuitos eléctricos*. Madrid: Editorial Pearson.
* Thomas, L. (2007). *Principios de circuitos eléctricos*. México: Editorial Pearson.
* Sadiku, M. (2006). *Fundamentos de circuitos eléctricos*. México: McGraw Hill Interamericana.
