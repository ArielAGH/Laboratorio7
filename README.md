# Laboratorio 7: Teorema de Thévenin
Integrantes: Caillamara Leonardo, González Ariel
## 1. OBJETIVOS

### Objetivo general:
* Demostrar el funcionamiento del teorema de Thévenin mediante mediante su aplicación en un circuito resistivo.
### Objetivos específicos:
*	Aplicar el teorema de Thévenin para una mejor comprensión de su uso en distintos circuitos.
*	Comparar valores obtenidos antes y después de la aplicación del teorema tanto en simulación como en cálculos. 

## 2. MARCO TEÓRICO

![](https://github.com/ArielAGH/Laboratorio6/blob/main/Img/Osciloscopio.png)

El osciloscopio es un instrumento de medida con el que visualizamos, por medio de una pantalla, la forma de las señales eléctricas que atraviesan un circuito en un periodo de tiempo.

El osciloscopio consta de dos ejes, el eje x es del tiempo y el eje y es para los valores de voltaje medidos.

Dependiendo de su diseño pueden analizar señales con mayor frecuencia de operación en el orden de: Hz, MHz, GHz.

![](https://github.com/ArielAGH/Laboratorio6/blob/main/Img/Osciloscopio2.png)
![](https://github.com/ArielAGH/Laboratorio6/blob/main/Img/Onda.png)

### Partes del Osciloscopio

Partes externas

![](https://github.com/ArielAGH/Laboratorio6/blob/main/Img/PartesExternas.png)

Partes internas

![](https://github.com/ArielAGH/Laboratorio6/blob/main/Img/PartesInternas.png)

### Tipos de Osciloscopios

Existen dos tipos marcados de osciloscopios:

1. Analógicos.- Es un instrumento que utiliza tubos de rayos catódicos para proyectar lecturas en una pantalla con recubrimiento de fósforo.
2. Digitales.- Este instrumento usa un conversor analógico digital para representar las mediciones en un display LCD.

### Aplicaciones

El osciloscopio es utilizado para determinar las realizar análisis y testeo de señales ya que a simple vista no podemos visualizar la forma de estas señales. Un ejemplo muy claro es determinar si un circuito que transforma corriente alterna en continua de verdad cumple con su función o existe algún desperfecto.

Otro uso importante es al momento de medir un circuito y no se sabe la frecuencia de operación de este no es posible tomar medidas con un polímetro es necesario utilizar un osciloscopio.

En la parte de visualización de imágenes con este dispositivo de medida es posible retener señales y analizarlas en escalas sin alterar la frecuencia a la que trabaja el circuito. En modelos más actuales el osciloscopio puede captar dos señales eléctricas. 

## 3. EQUIPOS Y MATERIALES

* **Generador de funciones:** Discpositivo capaz de modificar la forma de la señal de entrada.
* **Protoboard:** Es una placa de pruebas en la que se pueden insertar elementos electrónicos. En este caso Proteus utiliza un plano infinito como protoboard.
* **Resistencias eléctricas:** Elemento eléctrico que se opone al paso de corriente.
* **Cables puente:** Cables de ayuda para realizar conexiones provisionales.
* **Multímetro:** Es un instrumento analógico o digital portátil que se usa para medir directamente magnitudes eléctricas.
* **Osciloscopio:** Instrumento de medida capaz de graficar ondas de señales eléctricas.

## 4. PROCEDIMIENTO

4.1. Implemente el circuito que se presenta en la figura 7.1

![](https://github.com/ArielAGH/Laboratorio6/blob/main/Img/Circuito.png)

4.2. Ajuste el generador de funciones, para que proporcione una señal de 20 Vpp a
una frecuencia de 2.5 Khz.

4.3. Conecte el osciloscopio al resistor de carga RL. Observe la señal que aparece en
el osciloscopio.

### 4.4. Responda las siguientes preguntas:

![](https://github.com/ArielAGH/Laboratorio6/blob/main/Img/DCACLab.png)

##### ¿Cuántas divisiones por cuadro abarca la amplitud pico de la señal de salida?
Abarca 3 voltios por cuadro.

##### ¿En qué valor está posicionada la perilla VOLTS/DIV?
En el valor de 3.

##### ¿Cuántas divisiones por cuadro abarca el ciclo completo de la señal de salida?
Abarca 4 divisiones.

##### ¿En qué valor está posicionada la perilla TIME/DIV?
En 0.1 mili segundos.

### 4.5. ¿Cuál es la amplitud de voltaje y el período de la señal que aparece en la pantalla del osciloscopio?
<pre><code>
Amplitud de voltaje: 6.83 (V).
Período: 0.4 (ms).
</code></pre>

### 4.6. Determine la frecuencia natural (Hz) y la frecuencia angular (rad/s) de la señal de salida.
<pre><code>
f: 2500 (Hz)
w: 15707.96 (rad/s)
</code></pre>

### 4.7. Con el multímetro digital mida el voltaje de salida de RL:
Es de 4.8 (V).

### 4.8. Compare el voltaje medido en el punto 4.5. y el obtenido en el punto 4.7. ¿Coinciden? ¿Por qué?
Los valores no coinciden debido a que el voltaje del numeral 4.5. está medido desde el osciloscopio, lo que significa que es un valor de voltaje pico. Por otro lado, el voltaje del numeral 4.7. es menor puesto que el multímetro usado para su medición nos muestra el voltaje rms.

## 5. CONCLUSIONES

El osciloscopio es un instrumento de medición útil para el análisis de distintos tipos de señales ya que es posible determinar la frecuencia y periodo de la señal mediante los datos proporcionados por las perillas de ajuste del osciloscopio y la grafica proporcionada por este mismo. Además, es posible determinar voltajes en distintos puntos de la función y es posible observar gráficamente la forma se cada señal.

## 9. BIBLIOGRAFÍA

* Durán, J. (2012). *Electrotecnia*. Barcelona: Editorial Lexus.
* Hetpro. (2018). *Osciloscopio ¿Qué es? y ¿Cómo se usa?* Obtenido de: https://hetpro-store.com/TUTORIALES/osciloscopio/
* ToolBoom. (2015). *Osciloscopios: historia y clasificación.* Obtenido de: https://toolboom.com/es/articles-and-video/oscilloscopes-history-and-classification/
