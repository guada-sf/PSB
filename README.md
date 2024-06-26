# PSB
Trabajo Práctico Final de Procesamiento de Señales Biomédicas

Consigna:

Tema 1 - CLASIFICADOR DE ESTADOS DEL SUEÑO

En base a los datos de polisomnografía MIT/BIH generar un clasificador de estados del sueño
a partir de los datos de ECG correspondientes a cada paciente. Los datos corresponden a 18
registros. Los sujetos son varones de entre 32 y 56 años; y sus pesos varían entre 89 y 152
kg (peso promedio 119 kg). Los registros slp01a y slp01b son segmentos del mismo paciente,
pero slp02a y slp02b son de sujetos distintos. Los demás corresponden todos a distintos
pacientes. En todos los registros van a encontrar con una señal de ECG, una de presión
arterial invasiva, una de EEG y una señal de respiración. En algunos registros también se
incluye otras señales como la señal de esfuerzo respiratorio, el electrooculograma (EOG),
una señal de volumen sistólico y una señal de oxímetro del lóbulo de la oreja. Todas las
señales fisiológicas fueron muestreadas a una frecuencia de 250 Hz.

A partir de las señales de ECG deberán hallar los intervalos RR. Tengan en cuenta aquí que
si la serie temporal del intervalo RR contiene ruido, afectará negativamente a los resultados.
Por lo tanto, para eliminarlo, deberán realizar un prepocesado acorde de las señales y los
datos RR. Luego deberán extraer las características en el domino del tiempo y de frecuencia a tener en
cuenta para la clasificación.

Características en el dominio del tiempo:

Analizar la variación de los intervalos RR utilizando métodos estadísticos para caracterizar la
VFC. Extraer tres características en el dominio del tiempo: la media, la desviación estándar
(SD) y la RMSSD (la raíz cuadrada media de las diferencias sucesivas entre ciclos normales
adyacentes) de los intervalos RR.

Características en el dominio de las frecuencias:

Aquí deberán comparar los tres algoritmos vistos en clase para estimar la densidad espectral
de potencia de los intervalos RR: el algoritmo de transformada rápida de Fourier (FFT), el
método autorregresivo (AR) y el periodograma de Lomb (LS) para el análisis de la Variabilidad
de la Frecuencia Cardiaca (VFC). Se propone que extraigan las siguientes características a partir de cada método
mensionados: la relación LF-HF representada como LF/HF y LFn y HFn.

Finalmente, a partir de estos seis atributos deberán obtener un algoritmo que les permita
clasificar las etapas del sueño a partir de los datos de ECG y compara la eficiencia de los
métodos utilizados para el análisis espectral de la VFC.
