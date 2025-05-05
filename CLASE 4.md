# Modelación de sistemas eléctricos e hidráulicos 
## Analisis de circuitos con aimplificadores operacionales
En dinámica de sistemas, el análisis de circuitos con amplificadores operacionales se centra en modelar y entender cómo estos dispositivos controlan la relación entre señales de entrada y salida en diferentes configuraciones. Los amplificadores operacionales ideales se caracterizan por tener impedancia de entrada infinita, impedancia de salida cero y una ganancia de voltaje infinita, lo que implica que no hay corriente en las entradas y que los voltajes en las terminales  y son prácticamente iguales si existe retroalimentación negativa. El análisis consiste en aplicar estas propiedades ideales junto con las leyes de Kirchhoff y la ley de Ohm para plantear ecuaciones que describan el comportamiento dinámico del sistema. Dependiendo de su configuración, los amplificadores operacionales pueden funcionar como amplificadores inversores, no inversores, sumadores, integradores o derivadores, permitiendo la construcción de modelos matemáticos que representan ecuaciones diferenciales o relaciones algebraicas entre las señales. Así, los amplificadores operacionales se utilizan en dinámica de sistemas para modelar, analizar y diseñar sistemas de control, filtros, y otros circuitos que afectan la dinámica de señales eléctricas.
### Amplificador no inversor 
Un amplificador operacional no inversor es una configuración de un amplificador operacional (op-amp) donde la señal de entrada se aplica al terminal no inversor del op-amp (marcado como +), y el terminal inversor (marcado como−) se conecta a través de una red de resistencias que establece la ganancia del circuito.

💡**Ejemplo 1:** amplificador operacional

<img src="images/AO3.JPG"  width="300"/>

$$i_1 - i_2 = 0$$
$$\frac{e_o - e_i}{R_2} - \frac{e_i}{R_1} = 0$$
$$\frac{e_o}{R_2} = e_i \left( \frac{1}{R_2} + \frac{1}{R_1} \right)$$
$$e_o = e_i \left( 1 + \frac{R_2}{R_1} \right)$$

💡**Ejemplo 2:** amplificador operacional

<img src="images/AO2.JPG"  width="300"/>

$$i_1 - i_2 - i_3 = 0$$

$$\frac{e_i - e'}{R_1} - \frac{e' - e_o}{R_2} - C \frac{d(e' - e_o)}{dt} = 0$$

$$\frac{e_i}{R_1} - \frac{-e_o}{R_2} - C \frac{d(-e_o)}{dt} = 0$$

$$\frac{e_i}{R_1} = -\frac{e_o}{R_2} - C \frac{d(e_o)}{dt}$$

💡**Ejemplo 3:** amplificador operacional

<img src="images/AO1.JPG"  width="300"/>

## Analisis de sistemas hidráulicos
En dinámica de sistemas, los sistemas hidráulicos se modelan como analogías de otros tipos de sistemas físicos, como los eléctricos o los mecánicos, para entender cómo se comportan dinámicamente bajo diversas condiciones. Un sistema hidráulico es aquel en el que el movimiento o almacenamiento de un fluido (generalmente un líquido) se utiliza para transmitir, almacenar o controlar energía. En dinámica de sistemas, se estudia cómo variables como la presión, el caudal y el volumen cambian con el tiempo, basándose en principios de conservación de masa, energía y leyes físicas análogas.

### Modelo de un tanque 
Un modelo de un tanque en sistemas hidráulicos es una representación matemática simplificada del comportamiento de un recipiente diseñado para almacenar fluidos. Este modelo se fundamenta en el principio de conservación de masa (o volumen, para fluidos incompresibles), estableciendo una relación dinámica entre los caudales de entrada y salida del tanque y la variación del nivel del líquido en su interior con respecto al tiempo.

$$\begin{align*}
q_i, q_o \colon \text{Flujos de entrada y salida de líquido} \\
R_1 \colon \text{Resistencia al flujo} \\
A_1 \colon \text{Área transversal del tanque} \\
h_1 \colon \text{Nivel de líquido en el tanque}
\end{align*}$$
$$\begin{align*}
q_1 = \frac{h_1}{R_1} \\
A_1 \frac{dh_1}{dt} = q_i - q_1 \\
h_1 = q_1 \cdot R_1 \\
R_1 A_1 \frac{dq_1}{dt} = q_i - q_1
\end{align*}$$
### Modelo de dos tanques
Un modelo de dos tanques no interconectados describe el comportamiento independiente de dos recipientes de almacenamiento de fluidos, donde cada tanque tiene sus propias entradas y salidas que se puede relacionar con las ecuaciones anteriores. Cada tanque se modela individualmente mediante un balance de volumen que relaciona el caudal de entrada, el caudal de salida y la variación del nivel del líquido en función del tiempo, sin considerar ningún flujo que pase de un tanque al otro. posteriormente se busca una variable que pueda relacionar las ecuaciones en funcion de construir un modelo
### Modelos de dos tanques interconectados 
Un modelo de dos tanques interconectados describe la dinámica de almacenamiento y transferencia de fluido entre dos recipientes, considerando los caudales de entrada al primer tanque, de salida del segundo, y el flujo que se establece entre ellos a través de una conexión. Este flujo intermedio, que depende de la diferencia de nivel y la resistencia de la interconexión. 

$$\begin{align*}
q_1 &= \frac{h_1 - h_2}{R_1} \\
q_2 &= \frac{h_2}{R_2} \\
A_1 \frac{dh_1}{dt} &= (q_i - q_1) \\
A_2 \frac{dh_2}{dt} &= (q_1 - q_2)
\end{align*}$$

$$\begin{align*}
R_2 A_2 \frac{dq_2}{dt} = (q_1 - q_2) \\
R_2 A_2 \frac{dq_2}{dt} + q_2 = q_1 \\
A_1 \frac{dh_1}{dt} = \left( q_i - R_2 A_2 \frac{dq_2}{dt} + q_2 \right) \\
R_1 q_1 + h_2 = h_1 \\
R_1 \left( R_2 A_2 \frac{dq_2}{dt} + q_2 \right) + R_2 q_2 = h_1
\end{align*}$$

$$A_1 \frac{d \left( R_1 \left( R_2 A_2 \frac{dq_2}{dt} + q_2 \right) + R_2 q_2 \right)}{dt} = \left( q_i - R_2 A_2 \frac{dq_2}{dt} + q_2 \right)$$

$$\begin{align*}
A_1 \frac{d \left( R_1 \left( R_2 A_2 \frac{dq_2}{dt} + q_2 \right) + R_2 q_2 \right)}{dt} = \left( q_i - R_2 A_2 \frac{dq_2}{dt} + q_2 \right) \\
A_1 R_1 R_2 A_2 \frac{d^2 q_2}{dt^2} + (A_1 R_1 + A_1 R_2 + R_2 A_2) \frac{dq_2}{dt} - q_2 = q_i
\end{align*}$$


