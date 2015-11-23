% Estudio de procesos de generación, transferencia y recombinación de carga y transferencia de energía en polímeros conjugados nano-estructurados.  
Modelado, simulación y validación.
%Trabajo Final Integrador que será presentado para obtener el grado de  
Especialista en Cómputo de Altas Prestaciones y Tecnologías Grid  
Facultad de Informática  
Universidad Nacional de La Plata
% Versión 2015.11.23.00 (draft)

# Motivación
Los polímeros conjugados son materiales orgánicos semiconductores de gran relevancia debido a su actual aplicación en dispositivos orgánicos-electrónicos tales como celdas solares1,2,3,4,5, diodos emisores de luz (OLED)6,7,8, transistores de efecto campo (OFET)9,10,11,12, memorias moleculares13, etc. El modelo típico de la estructura electrónica de polímeros conjugados considera que las excitaciones electrónicas en cada cadena polimérica se limitan a segmentos relativamente cortos (de 5 a 15 monómeros) denominados cromóforos14,15,16. Estos cromóforos actúan en gran medida de forma independiente de manera tal que una cadena de polímero conjugado es vista como un sistema multi-cromofórico en el que la mayoría de la complejidad electrónica es consecuencia de las interacciones entre cromóforos.  
Consecuentemente, el funcionamiento y desempeño de dispositivos orgánicos-electrónicos basados en polímeros conjugados depende en gran medida de procesos fotofísicos elementales de transferencia de energía (TE), generación, transporte y recombinación de carga (GTRC) que ocurren entre cromóforos en el seno del polímero y en las interfaces orgánicas/inorgánicas (donde ocurre el contacto eléctrico entre polímero y electrodos)17.  
Muchos de estos dispositivos orgánicos-electrónicos se componen de películas ultra delgadas de polímero amorfos con alta a moderada heterogeneidad espacial y temporal. Esta heterogeneidad dificulta un estudio detallado de procesos TE y GTRC en estos materiales por técnicas convencionales que miden promedio de propiedades. El estudio de procesos TE y GTRC a nano-escala en películas poliméricas ultra-delgadas, nanopartículas (NPs) o moléculas poliméricas individuales utilizando técnicas avanzadas de microscopia de fluorescencia (por ejemplo espectroscopia de molécula/partícula individual) permite desentrañar la heterogeneidad mencionada14,15,16. En particular estas técnicas permiten la determinación de la distribución real de propiedades relevantes mediante su medición de a una partícula por vez en lugar de medir el promedio de un gran conjunto de partículas o moléculas. Debido a que las especies cargadas (polarones, cationes radicales o aniones radicales) en polímeros conjugados resultantes de los procesos GTRC son generalmente no fluorescentes su determinación es indirecta y se basa en: a) desactivación de fluorescencia de estados electrónicos excitados (excitones, cromóforos excitados) mediante especies cargadas18,19,20,21,22,23,24,25,26 o b) generación de estados electrónicos excitados emisores mediante recombinación de especies cargadas (electroluminiscencia, EL)20,25,27,28 c) Así mismo también es posible determinar la TE de excitación entre los cromóforos intrínsecos del polímero y cromóforos dopantes incluidos en la matriz polimérica en pequeña cantidad con el fin de ajustar sus propiedades optoelectrónicas. Por otro lado para complementar, contrastar y validar los estudios y resultados experimentales es de gran utilidad la creación de modelos computacionales que permitan simular los procesos de TE y GTRC en esos materiales.

- - -

                              (FALTAN LAS REFERENCIAS)

- - - 

## Objetivos
El objetivo general de este trabajo consiste en presentar el desarrollo completo del aporte en las áreas de modelado, simulación, validación y computación de alto desempeño que se ha realizado a la investigación del Laboratorio de Microscopía Óptica Avanzada (LMOA) de la Facultad de Ciencias Exactas Físico-Químicas y Naturales (CEFQyN) de la Universidad Nacional de Río Cuarto (UNRC).

El LMOA posee un equipamiento de última generación y RRHH de primer nivel. Desarrolla experimentación básica publicando sus trabajos en las más prestigiosas revistas. Se presenta el necesidad de comenzar a desarrollar simulaciones computacionales para avanzar en las investigaciones.

Parte de los objetivos es el desarrollo de habilidades y capacidades que permitan optimizar el abordaje multidisciplinar requerido cuando se colabora con profesionales de disciplinas diversas, como es el caso de la investigación básica en el laboratorio.

En este contexto, los temas a abordar comprenden el análisis del sistema, la confección del modelo, validación de los resultados y optimización el código usando técnicasy estratégias de programación paralela y HPC.

## Vinculación institucional
Este proyecto de investigación articula la colaboración entre un grupo de trabajo perteneciente a la UNRC, compuesto por personal técnico, personal docente, alumnos de grado y postgrado a la Facultad de Ciencias Exactas Fisicoquímica y Naturales UNRC; docentes e investigadores del HPC4EAS Research Group perteneciente a la Universidad Autónoma de Barcelona y docentes e investigadores del Instituto de Investigación en Informática LIDI perteneciente a la UNLP. El grupo involucra el trabajo coordinado de 8 personas y cuenta con apoyo económico de SECyT UNRC, ANPCyT-MINCyT Argentina, MINCyT Córdoba y CONICET. Así mismo el proyecto está vinculado mediante la formación de estudiantes a los siguientes programas educativos: Licenciatura en Física y Licenciatura en Química UNRC, Doctorado en Ciencias Químicas UNRC, Doctorado en Física UBA y Maestría en Computación de Alto Desempeño UNLP.

## Integrantes

**Alumno**

* Daniel Arnoldo Bellomo, alumno de la Maestría en Computación de alto Desempeño (UNLP).

**Directores**

* Dra. Dolores Isabel Rexachs del Rosario (Universidad Autónoma de Barcelona)
* Dr.  Rodrigo Emiliano Palacios (Universidad Nacional de Río Cuarto)
* ??? (Universidad Nacional de La Plata)
* ??? (Universidad Nacional de La Plata)
* ??? (Universidad Autónoma de Barcelona)
* ??? (Universidad Autónoma de Barcelona)
* Dr. Carlos Alberto Chesta (Universidad Nacional de Río Cuarto)

**Colaboradores**

Integran el equipo del Laboratorio de Microscopía Óptica Avanzada (LMOA) y participan del presente trabajo: Lic. Rodrigo Ponsio (doctorando), Franco Bellomo y Lucas Bellomo (estudiantes de Lic. en Física).

## Resumen
Se desarrolla una herramienta comutacional para calcular la eficiencia de Quenching.

Mediante simulaciones de Monte Carlo se pretende estudiar la eficiencia de Quenching para una nanopartícula (NP) determinada. Estas simulaciones van a ser contrastadas con las mediciones experimentales realizadas en el Laboratorio de Microscopia Optica Avanzada (LMOA) de la Universidad Nacional de Río Cuarto (UNRC).

En principio, son tres los experimentos en los que queremos corroborar la eficiencia de Quenching:

1. En el caso de tener los aceptores distribuidos volumetricamente en la NP.
2. Que los aceptores estén sobre la superficie de la NP.
3. En los dos casos anteriores el fotón es generado mediante un laser. Se quiere estudiar que sucede en el caso de que sea generado mediante una electrólisis química.

El LMOA tiene amplia experiencia en la investigación experimental, pero destaco que este es el primer trabajo científico que desarrollan realizando simulaciones computacionales. Para los científicos del laboratorio se crea un área nueva de trabajo, química computacional, por lo que demuestran un especial interes en el trabajo interdisciplinar. La colaboración que brindan para avanzar en este desarrollo es total, dedicando tiempo, atención y respondiendo un sinnumero de preguntas.

## Publicaciones relacionadas a este trabajo
* XVII Juan José Giambiagi Winter School.
Light and light-based technologies, Departamento de Física J.J. Giambiagi, FCEyN, UBA, August 3-7, 2015.  
Título: *Transferencia de energía en nanopartículas de polímeros conjugados. Modelado y contraste con datos experimentales* (poster)

## Formación de RRHH en programación científica
Se trabaja con alumnos de la carrera de Física para desarrollar capacidades de programación científica y HPC aplicadas a física computacional. Esta actividad pemitite la integración por parte de los alumnos en proyectos reales de la facultad, permitiendo formar parte de grupos de investigación y hacer aportes desde su área estecífica de formación desarrollando modelos computacionales.

# Marco teórico del fenómeno

## Modelo conceptual

## Probabilidad de decaimiento en $[0, t]$

La tasa de cambio de la población de cromóforos excitados $N$ es proporcional a la cantidad de cromóforos excitados, por lo que se puede escribir como

\begin{equation}
\label{eq:decaimiento}
\frac{dN}{dt} = -kN
\end{equation}

Donde $k$ es la constante de decaimiento total. La solución de esta ecuación diferencial es

\begin{equation}
\label{eq:N}
N = N_0e^{-kt}
\end{equation}

Ésta ecuación dice cuantos cromóforos excitados hay en cualquier tiempo $t$. Queremos determinar cuál es la probabilidad de que un cromóforo decaiga en un intervalo de tiempo $[0, t]$. Para esto, con la ayuda de (2), podemos escribir una función que sea el número de decaimientos en el intervalo $[0, t]$ como el número total de cromóforos excitados menos la cantidad de cromóforos existentes en el tiempo $t$

\begin{equation}
\label{eq:alpha}
\alpha = N_0-N_0e^{-kt}=N_0(1-e^{-kt})
\end{equation}

Podemos asignar ahora la probabilidad de un cromóforo de decaer en $[0, t]$ como el cociente de la cantidad de decaimientos en $[0, t]$ y el número total de cromóforos

\begin{equation}
\label{eq:P}
P=\frac{\alpha}{N_0} = 1-e^{-kt}
\end{equation}

## Cálculo del Exciton Diffusion Length 1 dimensión

Consideremos una caminata aleatoria unidimensional, que en cada paso recorre una distancia , y que tiene la misma probabilidad de caminar hacia la izquierda que hacia la derecha. La distancia entre el origen y $N$ pasos después es

\begin{equation}
\label{eq:X}
X=\sum_{i=1}^{N} x_i
\end{equation}

Donde $x_i$ puede ser $\epsilon$ con probabilidad $p$ o $-\epsilon$ con probabilidad $q$, siendo $p = q$. Si queremos ver cuánto vale $X$ promediando en muchas caminatas de este tipo debemos calcular el valor esperado de $X$. Esto es

\begin{equation}
\label{eq:E}
E(X) = \sum_{i=1}^{N} E(x_i)= \sum_{i=1}^{N} (p\epsilon - q\epsilon) =  0
\end{equation}

Ésto no arroja información respecto al Exciton Diffusion Length. La pregunta que nos hacemos entonces es: ¿cuánto va a diferir típicamente $X$ del su valor esperado? Definimos $r$ como la diferencia entre el valor $X$ de una caminata particular y el valor esperado de $X$

\begin{equation}
\label{eq:r}
r = X - E(X) = X
\end{equation}

Claramente no tiene sentido preguntarse por el valor esperado de $r$ ya que va a dar cero, de acuerdo con (6) y (7). Esto es debido a que r puede resultar positivo o negativo con la misma probabilidad, y al sumar estos valores en promedio se compensan, resultando cero su valor esperado. Por esto es útil preguntarse por el valor esperado del valor absoluto (siempre positivo) de $r$. Para esto calculamos el valor esperado de $r$ al cuadrado como

\begin{equation}
\label{eq:E1}
E(r^2) = E((X - E(X))^2) = E(X^2) = E\left[\left(\sum_{i=1}^{N}x_i\right)^2\right] = Var(x)
\end{equation}

Esto es por definición la varianza de $X$. El cuadrado de la sumatoria en (8) está compuesto de $N$ términos del tipo $x_i^2$, y $N(N - 1)$ términos cruzados del tipo $x_i x_j$ con $i$ distinto de $j$

\begin{equation}
\label{eq:E2}
E(r^2) = E\left(\sum_{i=1}^{N}x_i^2\right) + E\left(\sum_{i\neq1}x_i x_j\right)
\end{equation}

Notemos que

\begin{equation}
\label{eq:E3}
E\left(\sum_{i=1}^{N} x_i^2\right) = E\left(\sum_{i=1}^{N} \epsilon^2\right) = E(N \epsilon^2) = N \epsilon^2
\end{equation}

Y que

\begin{equation}
\label{eq:E4}
E\left(\sum_{i\neq j} x_i x_j\right) = 0
\end{equation}

Debido a que los términos de la sumatoria pueden tener resultados $\epsilon^2$ o $-\epsilon^2$ probabilidad. De (9), (10) y (11) se obtiene que

\begin{equation}
\label{eq:E5}
E(r^2) = N \epsilon^2 = Var(X)
\end{equation}

Tomando la raíz cuadrada de (12) podemos calcular la Desviación Standard $\sigma$ de $X$

\begin{equation}
\label{eq:sigma}
\sigma = \sqrt{N} \epsilon
\end{equation}

Ésta es una buena medida de la distancia entre el punto inicial y final de la caminata en N pasos, así que asignamos este valor al Exciton Difussion Length $L_D$

\begin{equation}
\label{eq:LD}
L_D = \sqrt{N} \epsilon
\end{equation}

## Cálculo del Exciton Diffusion Length 3 dimensiones

En tres dimensiones la situación es matemáticamente más compleja pero arroja el mismo resultado. Supongamos una caminata aleatoria tridimensional con la misma probabilidad de caminar hacia todas las direcciones. Supongamos que el largo de cada paso es $\epsilon$, de modo que las componentes cartesianas de cada paso $i$ deben cumplir

\begin{equation}
\label{eq:epsilon2}
x_i^2 + y_i^2 + z_i^2 = \epsilon^2
\end{equation}

El vector distancia entre el origen y $N$ pasos después de la caminata es entonces

\begin{equation}
\label{eq:R}
\vec{R}= \sum_{i=1}^{N} \vec{r_i}
\end{equation}

Donde $\vec{r_i} = x_i \hat{i} + y_i \hat{j} + z_i \hat{k}$. Al igual que en el caso unidimensional $E(\vec{R}) = 0$, por lo que calculamos

\begin{equation}
\label{eq:EvecR}
E(\vec{R^2}) = E\left[\left(\sum_{i=1}^{N} \vec{r_i}\right)^2\right] = E \left(\sum_{i=1}^{N} \vec{r_i}^2\right) + E \left(\sum_{i \neq 1} \vec{r_i} \vec{r_j}\right)
\end{equation}

El segundo término de la ecuación (17) es

\begin{equation}
\label{eq:E6}
E\left(\sum_{i \neq j} \vec{r_i} \vec{r_j}\right) = E \left(\sum_{i \neq j} (x_i x_j + y_i y_j + z_i z_j)\right) = 0
\end{equation}

Este término es cero debido a que los valores de $x_i, y_i,$ y $z_i$ pueden ser tanto negativos como positivos, y tienen la misma probabilidad de ser negativos que positivos. Cuando se computa la esperanza teniendo en cuenta todos los valores posibles de estas variables y su probabilidad, ésta da cero.

Otra forma de visualizar esto es imaginarse una esfera de radio $\epsilon$ y fijar arbitrariamente el vector $\vec{r_i}$ apuntando hacia arriba (ver figura). Luego se observa que el producto punto entre $\vec{r_i}$ y cualquier $\vec{r_j}$ del hemisferio superior de la esfera da un número positivo (debido a la definición de producto punto y que el ángulo entre ellos es menor a 90°), y el producto entre $\vec{r_i}$ y cualquier $\vec{r_j}$ del hemisferio inferior da negativo (debido a que el ángulo es mayor a 90°). Es posible sumar todos los productos punto correspondientes al hemisferio superior y obtener un valor positivo, y por otro lado sumar todos los productos punto correspondientes al hemisferio inferior y obtener un valor negativo. Debido a la simetría esférica de la situación, la magnitud del valor positivo y negativo deben ser iguales, por lo que cuando se sumen se obtendrá cero. Luego se repite este proceso para todo $\vec{r_i}$ (nuevamente dará cero) y finalmente se suman, dando el resultado final cero debido a que todos los términos son cero.

![](img/esfera.png)

Entonces

\begin{equation}
\label{eq:E7}
E(\vec{R}^2) = E \left(\sum_{i=1}^{N} \vec{r_i}^2 \right) = E \left(\sum_{i=1}^{N} \epsilon ^2\right) = N \epsilon ^2
\end{equation}

Y el Exciton Diffusion Length es igual que para el caso de una dimensión

\begin{equation}
\label{eq:E8}
L_D = \sqrt{N} \epsilon
\end{equation}

## Artículo de referencia

Changfeng Wu, Yueli Zheng, Craig Szymanski, and Jason McNeill, Energy Transfer in a Nanoscale Multichromophoric System: Fluorescent Dye-Doped Conjugated Polymer Nanoparticles, J. Phys. Chem. C 2008, 112, 1772-1781. American Chemical Society.

# Estado del arte

## Modelización

## Simulación

## Computación de altas prestación

# Propuesta

## modelo conceptual

## modelo computacional

## simulación de altas prestaciones

# Desarrollo computacional
Se consideran dos desarrollos

* diseño del simulador
* paralelismo

## Diseño del simulador
- mejoras en el diseño original (paper)
- fundamentos teóricos (teoría de simulación).
- en función del funcionamiento se realizan un modelo mejorado (en función de lo que observan los Químicos). El modelo original tienen restricciones teóricas que se van eliminando a medida que se avanza en el trabajo mediante la interacción con los Químicos.
- etapas de construcción (refinación) del modelo.
- validación de la simulación.
- fenómeno físico/químico a modelar desde el punto de vista computacional (detallar, explicar).

## Tipo de simulación
- ¿estática o dinámica? estática
- Montecarlo
- la simulación original es serial
- detalle de la simulación.
- marco teórico computacional.
- como se ha hecho la simulación.

## Tipo de escalabilidad
- fuerte / débil.
- se ejecuta muchas veces para luego calcular promedio y desviaciones.
- calcular tiempo de recursos (profile), ejecución, memoria, etc.

## Paralelismo
- ¿por qué?
- ¿para qué?
- multicore / cluster / GPGPU / cloud
- mejorar tiempos y/o mejorar precisión.
- mayor volumen de datos
- mayor cantidad de "doops"
- mayor cantidad de experimentos.
- speedup

# Validación experimental

## diseño de los experimentos

## entorno experimental

 Raspberry Pi para el desarrollo y validación

## experimentos y discusión. (precisión y speedup)

# Conclusiones y trabajos futuros

# Bibliografía
- Changfeng Wu, Yueli Zheng, Craig Szymanski and Jason McNeill: Energy Transfer in a Nanoscale Multichromophoric System: Fluorescent Dye-Doped Conjugated Polymer Nanoparticles. The Journal of Physical Chemistry C (ACS Publications).

- C. A. Chung, Simulation Modeling Handbook: a Practical Approach, 2004, ISBN-10: 0849312418

- Giancarlo Zaccone, Python Parallel Programming Cookbook, Packt, 2015, ISBN: 1785289586

- Gabriele Lanaro, Python High Performance Programming, Packt, 2013, ISBN: 1783288450

- Jesse M. Kinder Philip Nelson, A Student's Guide to Python for Physical Modeling, 2015, ISBN: 0691170509

- L. Felipe Martins, IPython Notebook Essentials, Packt, 2014,ISBN: 1783988347

# Anexos