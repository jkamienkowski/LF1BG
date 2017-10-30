# Archivos para análisis de datos de Laboratorio 1 de Física de Biólogos y Geólogos.
Estos códigos usan principalmente: 

* [Numpy][https://docs.scipy.org/doc/numpy-dev/dev/]
* [Pandas][https://pandas.pydata.org/pandas-docs/stable/index.html]
* [Scipy][https://docs.scipy.org/doc/scipy/reference/]

### Consideraciones generales
Todo está armado en Jupyter Notebook. Este entorno es muy bueno para explorar datos y compartir código comentado, pero deben tener cuidado de correr las celdas en orden. Si no lo hacen, pueden estar corriendo el código sobre datos que no corresponden... Como es el caso de algunos que obtenían valores de R^2 mayores a 1.

Originalmente estos archivos estaban armados en función de las prácticas, presentando sólo lo nuevo en cada una de ellas, pero pensados como bloques que después los alumnos debían ensamblar según lo requiera cada práctica. A continuación los desarmamos todavía más, en función de los análisis.

### Levantar los datos
La función que vamos a utilizar en primer lee archivos .csv (comma separated values), que son archivos en los que se representa una matriz de datos usando la coma (,) como separador de columnas y el punto (.) como separador de decimales. La función además acepta algunas líneas de encabezado, es decir que puede hacer la excepción de no mirar las primeras N líneas que tienen otro formato.

OJO: Guardar un archivo como .csv no convierte automáticamente el formato del archivo, es posible guardar cualquier cosa como .csv que después no va a leer.

Primer chequeo, abrir el archivo con Notepad, Wordpad, gedit, ... y fijarse en que formato está. 

* Si sólo tienen un archivo y no quieren complicar en nada el programa pueden cambiar el formato "a mano": Borrar el encabezado, Buscar&Reemplazar comas (,) por puntos (.), y Buscar&Reemplazar tabulaciones (\t ó     ) por comas (,). 

* Si no, se puede arreglar todo en Python...

### Histogramas.

### Estadísticos y Errores.
Algunos ejemplos para calcular estimadores de tendencia central y de dispersión (media, mediana, desvio estandar, etc). Y ejemplos de desarrollo para propagar errores. 

### Transformaciones y Gráficos XY con error.
Armada originalmente para la práctica de hojas. Otras transformación puede verse en el de amortiguado.

### Ajuste lineal por Cuadrados Mínimos.
Se presenta el código para estimar cuadrados mínimos y cuadrados mínimos ponderados o pesados. Este código incluye el calculo de R^2.

### Detección de flancos (para la señal del Photogate).
Se presenta estimar la velocidad a partir de la señal del Photogate. También se agrega un código para generarse unos datos sintéticos, los mismos son interesante para comprender el efecto del cambio de frecuencia de adquisición.

### Detección de máximos (para una señal oscilatoria).
Detección de picos y cáculo de la frecuencia angular para un movimiento oscilatorio simple y amortiguado. También se agregan códigos para generarse unos datos sintéticos, los mismos son interesante para comprender el efecto del cambio de frecuencia de adquisición y del ruido en la detección de máximos.
En función de la experiencia en clase, se incluye un algoritmo más complejo para los casos en los que el primero no funciona.

## Otros programas / Más info.
### Programa de análisis de datos de video: [Tracker][https://physlets.org/tracker/]
### [Página de la materia][http://materias.df.uba.ar/f1bygaa2017c2/]
