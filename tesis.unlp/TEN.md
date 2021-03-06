\begin{figure}[!bp]
	\centering
	\includegraphics[width=17.5cm]{img/first+draft.jpg}
\end{figure}

# Introducción

> **Nota de Lola**  
> planteamiento general del tema

Los polímeros conjugados son materiales orgánicos semiconductores de gran relevancia debido a su actual aplicación en dispositivos orgánicos-electrónicos tales como celdas solares [@Lindstrom2006], diodos emisores de luz (OLED) [@Kulkarni2004], transistores de efecto campo (OFET) [@Mabeck2006], memorias moleculares [@Scott2007], etc. El modelo típico de la estructura electrónica de polímeros conjugados considera que las excitaciones electrónicas en cada cadena polimérica se limitan a segmentos relativamente cortos (de 5 a 15 monómeros) denominados cromóforos [@Lupton2010]. Estos cromóforos actúan en gran medida de forma independiente de manera tal que una cadena de polímero conjugado es vista como un sistema multi-cromofórico en el que la mayoría de la complejidad electrónica es consecuencia de las interacciones entre cromóforos.  
Consecuentemente, el funcionamiento y desempeño de dispositivos orgánicos-electrónicos basados en polímeros conjugados depende en gran medida de procesos fotofísicos elementales de transferencia de energía (TE), generación, transporte y recombinación de carga (GTRC) que ocurren entre cromóforos en el seno del polímero y en las interfaces orgánicas/inorgánicas (donde ocurre el contacto eléctrico entre polímero y electrodos) [@Zhu2009].  

## Motivación

> **Nota de Lola**  
> razones por las que el autor ha decidido trabajar sobre el tema

Muchos de estos dispositivos orgánicos-electrónicos se componen de películas ultra delgadas de polímero amorfos con alta a moderada heterogeneidad espacial y temporal. Esta heterogeneidad dificulta un estudio detallado de procesos TE y GTRC en estos materiales por técnicas convencionales que miden promedio de propiedades. El estudio de procesos TE y GTRC a nano-escala en películas poliméricas ultra-delgadas, nanopartículas (NPs) o moléculas poliméricas individuales utilizando técnicas avanzadas de microscopia de fluorescencia (por ejemplo espectroscopia de molécula/partícula individual) permite desentrañar la heterogeneidad mencionada [@Lupton2012]. En particular estas técnicas permiten la determinación de la distribución real de propiedades relevantes mediante su medición de a una partícula por vez en lugar de medir el promedio de un gran conjunto de partículas o moléculas.

## Objetivos

> **Nota de Lola**  
> Objetivos:  
> * general  
> * especificos  
> descripcion gral del trabajo (resumen)  
> estructura de la memoria

El objetivo general de este trabajo consiste en proponer un modelo (integral) computacional para el estudio de procesos de generación, transferencia y recombinación de carga y transferencia de energía en polímeros conjugados nano-estructurados. Este modelo comprende el proceso de modelización, simulación, validación y técnicas de computación de alto desempeño para calcular la energía de Quenching y poder así continuar las investigaciones del tema que realiza el Laboratorio de Microscopía Óptica Avanzada (LMOA) de la Facultad de Ciencias Exactas Físico-Químicas y Naturales (FCEFQyN) de la Universidad Nacional de Río Cuarto (UNRC).

Dentro de los objetivos específicos se tiene el lograr maximizar el speedup considerando una utilización eficiente de los recursos computacionales con que contamos.

Parte de los objetivos es el desarrollo de habilidades y capacidades que permitan optimizar el abordaje multidisciplinar requerido cuando se colabora con profesionales de disciplinas diversas, como es el caso de la investigación básica en el laboratorio.

En este contexto, los temas a abordar comprenden el análisis del sistema, la confección del modelo, validación de los resultados y optimización el código usando técnicas y estratégias de programación paralela y HPC.

## Vinculación institucional

Este proyecto de investigación articula la colaboración entre un grupo de trabajo perteneciente a la UNRC, compuesto por personal técnico, personal docente, alumnos de grado y postgrado a la Facultad de Ciencias Exactas Fisicoquímica y Naturales UNRC; docentes e investigadores del HPC4EAS Research Group perteneciente a la Universidad Autónoma de Barcelona y docentes e investigadores del Instituto de Investigación en Informática LIDI perteneciente a la UNLP. El grupo involucra el trabajo coordinado de 8 personas y cuenta con apoyo económico de SECyT UNRC, ANPCyT-MINCyT Argentina, MINCyT Córdoba y CONICET. Así mismo el proyecto está vinculado mediante la formación de estudiantes a los siguientes programas educativos: Licenciatura en Física y Licenciatura en Química UNRC, Doctorado en Ciencias Químicas UNRC, Doctorado en Física UBA y Maestría en Computación de Alto Desempeño UNLP.

## Resumen
Se desarrolla un software para realizar simunaciones computacionales que permitan estudiar los procesos de TE y GTRC en los materiales descriptos.

Mediante simulaciones de Montecarlo se estudia la eficiencia de Quenching para una nanopartícula (NP) determinada. Estas simulaciones serán contrastadas con las mediciones experimentales realizadas en el Laboratorio de Microscopia Óptica Avanzada (LMOA) de la Universidad Nacional de Río Cuarto (UNRC).

En principio, son tres los experimentos en los que queremos corroborar la eficiencia de Quenching:

1. En el caso de tener los aceptores distribuidos volumetricamente en la NP.
2. Que los aceptores estén sobre la superficie de la NP.
3. En los dos casos anteriores el fotón es generado mediante un laser. Se quiere estudiar que sucede en el caso de que sea generado mediante una electrólisis química.

El LMOA tiene amplia experiencia en la investigación experimental, pero destaco que este es el primer trabajo científico que desarrollan realizando simulaciones computacionales. Para los científicos del laboratorio se crea un área nueva de trabajo, química computacional, por lo que demuestran un especial interes en el trabajo interdisciplinar. La colaboración que brindan para avanzar en este desarrollo es total, dedicando tiempo, atención y respondiendo un sinnumero de preguntas.

## Publicaciones relacionadas a este trabajo
* 11º Encuentro Regional de Probabilidades y Estadística Matemática ERPEM  
Departamento de Matemáticas, FCEFQyN, UNRC, 2-3 de diciembre, 2015 \footnote{11º Encuentro Regional de Probabilidades y Estadística Matemática (ERPEM), FCEFQyN UNRC. \url{http://intra.exa.unrc.edu.ar/eventos/erpem}}  
Titulo: *Transferencia de energía en nanopartículas de polímeros conjugados. Modelización y validación con datos experimentales* (poster) \url{https://github.com/pewen/ten.extras/raw/master/2015_ERPEM/poster_TEN_ERPEM_2015_comprimido.pdf}

* XVII Juan José Giambiagi Winter School. Light and light-based technologies.  
Departamento de Física J.J. Giambiagi, FCEyN, UBA, 3-7 de agosto, 2015 \footnote{XVII Giambiagi Winter School, Departamento de Física, FCEyN UBA. \url{http://giambiagi2015.df.uba.ar}}  
Título: *Transferencia de energía en nanopartículas de polímeros conjugados. Modelado y contraste con datos experimentales* (poster) \url{https://github.com/pewen/ten.extras/raw/master/2015_Giambiagi/poster_Giambiani.compressed.pdf}

## Formación de RRHH en programación científica
Se trabaja con alumnos de la carrera de Física para desarrollar capacidades de programación científica y HPC aplicadas a física computacional. Esta actividad pemitite la integración por parte de los alumnos en proyectos reales de la facultad, permitiendo formar parte de grupos de investigación y hacer aportes desde su área estecífica de formación desarrollando modelos computacionales.

## Estructura de la monografía

El **capítulo 2** desarrolla el marco teórico del fenómeno, resaltando los atecedentes y el modelo conceptual.

El **capítulo 3** muestra los conceptos teóricos de la modelizacion, simulación, la computación de altas prestaciones y los lenguajes de programación coentífica que consideramos para este trabajo, justificando nuestra elección.

El **capítulo 4** detalla la propuesta que se lleva a cabo: modelo conceptual, modelo computacional, simulaciones de Monte Carlo y simulaciones de altas prestaciones.

El **capítulo 5** desarrolla el modelo computacional, el diseño del simulador, el tipo de simulación, la escalabilidad y el paralelismo.

El **capítulo 6** desarrolla la valicación experimental mostrando el desarrollo de los experimentos y el entorno experimental.

El **capítulo 7** detalla las conclusiones y trabajos futuros.

El **capítulo 8** tiene los anexos (integrantes del laboratorio, licencia del código).

\begin{figure}[!bp]
	\centering
	\includegraphics[width=10cm]{img/stamp-draft.jpg}
\end{figure}

# Marco teórico del fenómeno

Debido a que las especies cargadas (polarones, cationes radicales o aniones radicales) en polímeros conjugados resultantes de los procesos GTRC son generalmente no fluorescentes su determinación es indirecta y se basa en:

a. Desactivación de fluorescencia de estados electrónicos excitados (excitones, cromóforos excitados) mediante especies cargadas [@Palacios2009_2] o 
b. Generación de estados electrónicos excitados emisores mediante recombinación de especies cargadas (electroluminiscencia, EL) [@Nothaft2012_2]
c. Así mismo también es posible determinar la TE de excitación entre los cromóforos intrínsecos del polímero y cromóforos dopantes incluidos en la matriz polimérica en pequeña cantidad con el fin de ajustar sus propiedades optoelectrónicas.

Por otro lado para complementar, contrastar y validar los estudios y resultados experimentales es de gran utilidad **el desarrollo de modelos computacionales que permitan simular los procesos** de TE y GTRC en esos materiales.

El LMOA posee un equipamiento de última generación y un grupo de investigación de primer nivel. Desarrolla experimentación básica publicando sus trabajos en prestigiosas revistas y congresos. Se presenta el necesidad de comenzar a desarrollar simulaciones computacionales para avanzar en las investigaciones.

## Antecedentes

Para realizar el trabajo se toma como antecedente el paper [@McNeill2008]

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

Ésta ecuación dice cuantos cromóforos excitados hay en cualquier tiempo $t$. Queremos determinar cuál es la probabilidad de que un cromóforo decaiga en un intervalo de tiempo $[0, t]$. Para esto, con la ayuda de \ref{eq:N}, podemos escribir una función que sea el número de decaimientos en el intervalo $[0, t]$ como el número total de cromóforos excitados menos la cantidad de cromóforos existentes en el tiempo $t$

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

**Caminata aleatoria 1d.**

Consideremos una caminata aleatoria unidimensional, que en cada paso recorre una distancia $\epsilon$, y que tiene la misma probabilidad de caminar hacia la izquierda que hacia la derecha. La distancia entre el origen y $N$ pasos después es

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

Claramente no tiene sentido preguntarse por el valor esperado de $r$ ya que va a dar cero, de acuerdo con \ref{eq:E} y \ref{eq:r}. Esto es debido a que r puede resultar positivo o negativo con la misma probabilidad, y al sumar estos valores en promedio se compensan, resultando cero su valor esperado. Por esto es útil preguntarse por el valor esperado del valor absoluto (siempre positivo) de $r$. Para esto calculamos el valor esperado de $r$ al cuadrado como

\begin{equation}
\label{eq:E1}
E(r^2) = E((X - E(X))^2) = E(X^2) = E\left[\left(\sum_{i=1}^{N}x_i\right)^2\right] = Var(x)
\end{equation}

Esto es por definición la varianza de $X$. El cuadrado de la sumatoria en \ref{eq:E1} está compuesto de $N$ términos del tipo $x_i^2$, y $N(N - 1)$ términos cruzados del tipo $x_i x_j$ con $i$ distinto de $j$

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

**Caminata aleatoria 3d.**

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

El segundo término de la ecuación $\ref{eq:EvecR}$ es

\begin{equation}
\label{eq:E6}
E\left(\sum_{i \neq j} \vec{r_i} \vec{r_j}\right) = E \left(\sum_{i \neq j} (x_i x_j + y_i y_j + z_i z_j)\right) = 0
\end{equation}

Este término es cero debido a que los valores de $x_i, y_i,$ y $z_i$ pueden ser tanto negativos como positivos, y tienen la misma probabilidad de ser negativos que positivos. Cuando se computa la esperanza teniendo en cuenta todos los valores posibles de estas variables y su probabilidad, ésta da cero.

\begin{wrapfigure}{r}{0.4\textwidth}
	\centering
	\includegraphics[width=0.4\textwidth]{img/esfera.png}
	\caption{\label{fig:esfera} esfera de radio $\epsilon$ y $\vec{r_i}$} \noindent \hrulefill
\end{wrapfigure}

Otra forma de visualizar esto es imaginarse una esfera de radio $\epsilon$ y fijar arbitrariamente el vector $\vec{r_i}$ apuntando hacia arriba (ver figura \ref{fig:esfera}). Luego se observa que el producto punto entre $\vec{r_i}$ y cualquier $\vec{r_j}$ del hemisferio superior de la esfera da un número positivo (debido a la definición de producto punto y que el ángulo entre ellos es menor a 90°), y el producto entre $\vec{r_i}$ y cualquier $\vec{r_j}$ del hemisferio inferior da negativo (debido a que el ángulo es mayor a 90°). Es posible sumar todos los productos punto correspondientes al hemisferio superior y obtener un valor positivo, y por otro lado sumar todos los productos punto correspondientes al hemisferio inferior y obtener un valor negativo. Debido a la simetría esférica de la situación, la magnitud del valor positivo y negativo deben ser iguales, por lo que cuando se sumen se obtendrá cero. Luego se repite este proceso para todo $\vec{r_i}$ (nuevamente dará cero) y finalmente se suman, dando el resultado final cero debido a que todos los términos son cero.

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

\begin{figure}[!bp]
	\centering
	\includegraphics[]{img/draft_1.jpg}
\end{figure}

# Estado del arte

## Modelización

## Simulación

## Computación de altas prestación

**GPU**

Las unidades de procesamiento gráfico, GPU, se han convertido en una parte integral de los sistemas actuales de computación. El bajo costo y marcado incremento del rendimiento, permitieron su fácil incorporación al mercado. En los últimos años, su evolución implicó un cambio, dejó de ser un procesador gráfico potente para convertirse en un co-procesador apto para el desarrollo de aplicaciones paralelas de propósito general con demanda de anchos de banda de procesamiento y de memoria sustancialmente superiores a los ofrecidos por la CPU.  
La rápida adopción de las GPU como computadora paralela de propósito general se vio favorecida por el incremento tanto de sus capacidades como de las facilidades y herramientas de programación. Actualmente la GPU se ha posicionado como una alternativa atractiva a los sistemas tradicionales de computación paralela [@Piccoli2011:_GPU].


## Lenguajes de programación científica

**Fortran**

La comunidad científica ha usado Fortran desde siempre (las primeras versiones del lenguaje son de la década del 50, época de las tarjetas perforadas). Sin dudas, es el lenguaje más usado para resolver problemas científicos. Posee una amplia comunidad de usuarios y programas desarrollados hace décadas todavía son usados. La bibliografía y documentación es extensa.  
Existen librerias optimizadas, serial y paralela, y fuertemente probadas para realizar virtualmente todos los cálculos necesarios. Las versiones de OpenMP y MPI soportan nativamente Fortran.
Si el factor que va a desidir la elección del lenguaje de programación es el tiempo de ejecución, entendemos que Fortran es la elección correcta.

**Python**

Lenguaje creado a en el año 1991 (por lo que podemos considerarlo "moderno" comparandolo con Fortran).

Ecosistema científico: IPython/Jupyter [@PER-GRA:2007], Numpy, Matplotlib, Scipy. Entorno de programación interactivo de vanguardia, simple, libre, gratuito y multiplataforma.

Numpy brinda funcionalidades para trabajar con matrices.

Scipy es la biblioteca científica.

Matplotlib 

**Julia**

Fue diseñado para computación distribuida y en paralelo, 

**CUDA C**

**OpenCL**

**PyCUDA y PyOpenCL**
[@kloeckner_pycuda_2012]

**MPI4Python**
[@Dalcin2005] 

\begin{figure}[!bp]
	\centering
	\includegraphics[]{img/draft_1.jpg}
\end{figure}

# Propuesta

## Modelo conceptual

## Modelo computacional

## Simulaciones de Monte Carlo

## Simulación de altas prestaciones

\begin{figure}[!bp]
\centering
\includegraphics[width=10cm]{img/draft-stamp.jpg}
\end{figure}

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

\begin{figure}[!bp]
	\centering
	\includegraphics[]{img/draft_1.jpg}
\end{figure}

# Validación experimental

## Diseño de los experimentos

### Puntos aleatorios en la esfera

**En la superficie**

```python
n = 3000
R = 5

theta = np.random.uniform(low = 0, high = 2 * np.pi, size = n)
phi = np.random.uniform(low = 0, high = np.pi, size = n)

x = np.sin(phi) * np.cos(theta)
y = np.sin(phi) * np.sin(theta)
z = np.cos(phi)

fig = plt.figure(figsize=(12,12))
ax = fig.add_subplot(111, projection='3d')
ax.scatter(x, y, z)
```

\begin{figure}[!htb]
	\centering
	\includegraphics[width=13cm]{img/ptos_en_superficie_1.png}
	\caption{\label{fig:ptos_en_superficie_1} distribución no uniforme}
\end{figure}

en la figura \ref{fig:ptos_en_superficie_1} se muestra que la distribución no es uniforme, se ve claramente la concentración de puntos en los polos.

Entonces, necesitamos mejorar la distribución para hacerla uniforme:

```python
n = 3000
theta = 2 * np.pi * np.random.uniform(size=n)
phi = np.arccos(2 * np.random.uniform(size=n) - 1)

x = np.sin(phi) * np.cos(theta)
y = np.sin(phi) * np.sin(theta)
z = np.cos(phi)

fig = plt.figure(figsize=(12,12))
ax = fig.add_subplot(111, projection='3d')
ax.scatter(x, y, z)
```

\begin{figure}[!htb]
	\centering
	\includegraphics[width=15cm]{img/ptos_en_superficie_2.png}
	\caption{\label{fig:ptos_en_superficie_2} distribución uniforme}
\end{figure}

Ahora la distribición es uniforme en la superficie. Continuamos trabajando en el interior de la superficie.

**En el interior**

definimos el radio como una variable

```python
n = 3000
theta = 2 * np.pi * np.random.uniform(size=n)
phi = np.arccos(2 * np.random.uniform(size=n) - 1)

#theta = np.random.uniform(low=0, high = 2 * np.pi, size=n)
#phi = np.arcsin(2 * np.random.uniform(low=0, high = 2 * np.pi, size=n) - 1)
u = np.random.uniform(low=0, high=10, size=n)

x = np.sin(phi) * np.cos(theta) * u
y = np.sin(phi) * np.sin(theta) * u
z = np.cos(phi) * u

fig = plt.figure(figsize=(12,12))
ax = fig.add_subplot(111, projection='3d')
ax.scatter(x, y, z)
```

\begin{figure}[!htb]
	\centering
	\includegraphics[width=15cm]{img/ptos_en_interior_1.png}
	\caption{\label{fig:ptos_en_interior_1} distribución no uniforme}
\end{figure}

se agrega el *IF*

```python
n = 3000 
R = 5
a = 0

x_l = []
y_l = []
z_l = []

t = time.time()

while a <= n:
    x = np.random.uniform(low = -R, high = R, size=1)
    y = np.random.uniform(low = -R, high = R, size=1)
    z = np.random.uniform(low = -R, high = R, size=1)
    if x * x + y * y + z * z <= R * R:
        a += 1
        x_l.append(x)
        y_l.append(y)
        z_l.append(z)

print("time =",time.time() - t)

fig = plt.figure(figsize=(12,12))
ax = fig.add_subplot(111, projection='3d')
ax.scatter(x_l, y_l, z_l)
```

\begin{figure}[!htb]
	\centering
	\includegraphics[width=15cm]{img/ptos_en_interior_2.png}
	\caption{\label{fig:ptos_en_interior_2} distribución uniforme}
	\end{figure}

lo que funciona correctamente pero demasiado lento.

**El método eficiente**

El el foro de matemática \href{https://math.stackexchange.com/questions/87230/picking-random-points-in-the-volume-of-sphere-with-uniform-probability}{math.stackexchange.com} encontramos el método eficiente para obtener puntos al azar en el volumen de esfera con probabilidad uniforme \footnote{Picking random points in the volume of sphere with uniform probability http://tiny.cc/nycy6x}.

Suponemos la esfera centrada en el origen $(0,0,0)$.

\newpage

## Entorno experimental

Raspberry Pi para el desarrollo y validación

IPython/Jupyter para mostrar avances

## Experimentos y discusión. (precisión y speedup) 

## Ciencia reproducible

\begin{figure}[!bp]
\centering
\includegraphics[width=10cm]{img/draft-stamp.jpg}
\end{figure}

# Conclusiones y trabajos futuros

Fortalecer el trabajo multi/interdisciplinar.

**Trabajos Futuros**

Analizar performance del "caminante aleatorio tridimencional" usando distintos lenguajes (Julia, Fortran, C) y estatégias de optimización/paralelización, con el objetivo de mejorar los tiempos de ejecución.

Analizar métodos alternativos al que usa Numpy para generar números random, por ej: The Scalable Parallel Random Number Generators Library (SPRNG)
http://www.sprng.org

\begin{figure}[!bp]
\centering
\includegraphics[width=15cm]{img/draft-stamp.jpg}
\end{figure}

# Anexos

## Integrantes del equipo del Laboratorio de Microscopía Óptica Avanzada

El Laboratorio de Microscopía Óptica Avanzada (LMOA) es dirigido por el Dr. Rodrigo Emiliano Palacios. Integran el equipo y participan del presente trabajo: Lic. Rodrigo Ponsio (doctorando), Franco Bellomo y Lucas Bellomo (estudiantes de Lic. en Física).

## Licencia del documento

\begin{wrapfigure}{r}{0\textwidth}
	\includegraphics[width=3.5cm]{img/by.eps}
\end{wrapfigure}

Este documento esta realizado bajo licencia Creative Commons “Reconocimiento 4.0 Internacional” (CC BY 4.0) \href{http://creativecommons.org/licenses/by/4.0/deed.es}{http://creativecommons.org/licenses/by/4.0/deed.es}

## Licencia del código

 The MIT License (MIT)

Copyright © 2015 Laboratorio de Microscopia Óptica Avanzada UNRC

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

\begin{figure}[!bp]
\centering
\includegraphics[scale=1.6]{img/draft.jpg}
\end{figure}

# Bibliografía
