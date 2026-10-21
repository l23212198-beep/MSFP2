[![Open in MATLAB Online](https://www.mathworks.com/images/responsive/global/open-in-matlab-online.svg)](https://matlab.mathworks.com/open/github/v1?repo=l23212198-beep/MSFP2)
# Práctica 2: Modelado del sistema cardiovascular mediante el modelo de Windkessel

## Información de la estudiante

Martin Alonso Gonzalez Holguin [23212198]; l23212198@tectijuana.edu.mx

Modelado de Sistemas Fisiológicos

Ingeniería Biomédica

## Docente

Dr. Paul Antonio Valle Trujillo; paul.valle@tectijuana.edu.mx

Departamento de Ingeniería Eléctrica y Electrónica, Tecnológico Nacional de México/IT Tijuana, Blvd. Alberto Limón Padilla s/n, Tijuana, C.P. 22454, B.C., México.

## Descripción de la asignatura

El modelado de sistemas fisiológicos permite representar procesos del cuerpo humano mediante modelos matemáticos y computacionales para comprender su funcionamiento y analizar cómo responden ante distintas condiciones. En el caso del sistema cardiovascular, se emplean analogías entre las variables hemodinámicas y los elementos de los circuitos eléctricos: la presión sanguínea se relaciona con el voltaje, el flujo sanguíneo con la corriente y la resistencia vascular con la resistencia eléctrica. La capacidad de las arterias para almacenar sangre durante la eyección cardíaca se representa mediante una capacitancia. Estas relaciones permiten estudiar el comportamiento dinámico de la circulación y desarrollar simulaciones útiles en Ingeniería Biomédica.

La asignatura integra conocimientos de fisiología, electrónica, matemáticas y simulación para formular modelos que describan sistemas biológicos. Mediante el estudio del modelo de Windkessel, se busca comprender cómo la resistencia periférica y la distensibilidad arterial influyen en la presión y el flujo sanguíneo, así como reconocer las posibilidades y limitaciones de una representación simplificada del sistema cardiovascular.

## Objetivos

1. Comprender el funcionamiento del sistema cardiovascular a partir del modelo de Windkessel.
2. Identificar las variables fisiológicas del modelo, principalmente la presión arterial, el flujo sanguíneo, la resistencia vascular y la distensibilidad arterial.
3. Establecer la analogía entre el sistema cardiovascular y su circuito eléctrico equivalente.
4. Describir matemáticamente la relación entre los elementos del modelo y la respuesta dinámica de la circulación arterial.
5. Implementar y analizar la simulación del modelo cardiovascular con las herramientas computacionales utilizadas en la práctica.
6. Interpretar la influencia de los parámetros del modelo sobre el comportamiento de la presión y el flujo sanguíneo.

## Descripción detallada del sistema

En esta práctica se estudia el sistema cardiovascular mediante el modelo de Windkessel, una representación simplificada de la circulación arterial que permite analizar la relación entre el flujo sanguíneo impulsado por el corazón y la presión generada en las arterias. Su principio fundamental consiste en representar la elasticidad de los grandes vasos y la oposición al paso de la sangre mediante elementos equivalentes de un circuito eléctrico.

En la analogía eléctrica, la presión arterial corresponde a la diferencia de potencial eléctrico y el flujo sanguíneo a la corriente. La resistencia eléctrica representa la resistencia vascular periférica, mientras que el capacitor representa la capacidad de las arterias para expandirse y almacenar temporalmente parte del volumen sanguíneo durante la sístole. Durante la diástole, la recuperación elástica de las paredes arteriales contribuye a mantener el flujo aun cuando el corazón deja de expulsar sangre momentáneamente.

Para una representación básica de dos elementos, el modelo considera una resistencia periférica (R) y una capacitancia arterial (C). Su comportamiento puede describirse mediante el balance entre el flujo de entrada, el flujo que atraviesa la resistencia y el volumen almacenado por la capacitancia:


$$
Q_{in}(t) = C\frac{dP(t)}{dt} + \frac{P(t)}{R}
$$

En esta expresión, \(Q_{in}(t)\) es el flujo sanguíneo de entrada, \(P(t)\) es la presión arterial respecto a una presión de referencia, \(R\) representa la resistencia vascular periférica y \(C\) la distensibilidad arterial. La constante de tiempo \(\tau = RC\) caracteriza la rapidez con que disminuye la presión en ausencia de flujo de entrada. Esta ecuación se presenta como fundamento general del modelo de dos elementos; su correspondencia exacta con el circuito empleado en la práctica debe verificarse con el material del curso.

La simulación permite observar cómo las variaciones de resistencia y capacitancia modifican la respuesta temporal de la presión arterial. Un incremento de la resistencia tiende a dificultar la salida de sangre hacia la circulación periférica, mientras que los cambios en la capacitancia modifican la capacidad de amortiguar las variaciones de presión. Así, el modelo facilita la interpretación de la función de las arterias como reservorio elástico y muestra la utilidad de las analogías eléctricas para estudiar fenómenos fisiológicos.

**Palabras clave:** Sistema cardiovascular; Modelo de Windkessel; Presión arterial; Flujo sanguíneo; Resistencia vascular; Capacitancia arterial; Simulación.

## Lista de archivos incluidos en el repositorio

1. Cuaderno computacional de MATLAB [.mlx].
2. Modelo de Simulink [.slx].
3. Archivos de Spyder [.py].
4. Imagen con los parámetros del controlador.
5. Imágenes de las simulaciones [.pdf y .png].
6. Análisis matemático: Función de transferencia, modelo de ecuaciones integro-diferenciales, estabilidad y error en estado estacionario.

## Referencias

[1] P. A. Valle, *Syllabus para Modelado de Sistemas Fisiológicos*, Tecnológico Nacional de México / Instituto Tecnológico de Tijuana, Tijuana, B.C., México, 2025. Permalink: https://biomath.xyz/course/

[2] M. C. Khoo, *Physiological Control Systems Analysis Simulation, and Estimation*, 2nd ed. Piscataway, New Jersey, USA: IEEE Press, 2018, Section 4, Page 93.

[3] N. S. Nise, *Control Systems Engineering*, 8th ed. Hoboken, New Jersey, USA: John Wiley & Sons, 2020.
