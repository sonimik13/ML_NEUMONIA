## Clasificación de imágenes de neumonía vírica no COVID-19, neumonía vírica COVID-19 y pulmones sanos

He partido de la base de datos de imágenes de rayos X de COVID-19 de la Sociedad Italiana de Radiología Médica e Intervencionista (SIRM) COVID-19 DATABASE. 

![ ML](img/ML.png)

* Modelos de redes convolucionales (1 canal y 3 canales)
* Modelos transfer learning (VGG-16 y ResNet-50)
* Gráficas con las estadísticas de accuracy y loss para datos de train y validación
* Matriz de confusión
* Predicción de imágenes nuevas

Quería realizar un estudio 100% científico de la evolución del SARS-CoV-2 en España debido al antes y después que hemos experimentado y que estamos experimentando en todo el mundo en mayor o menor medida a causa del SARS-CoV-2.

Los datasets que he usado para tal fin los he obtenido de la página web del Instituto Carlos III y, al hacerlo, ví que no tenía datos de la población, por lo que tuve que recopilarlos de la página del INE.

Me he limitado a analizar la evolución de la pandemia y el grado de afectación al sector de la población por sexo, grupo de edad, sexo-grupo de edad en España desde el 01/01/2020 hasta el 09/03/2021. Quería analizar un poco más en profundidad y he bajado hasta el nivel de CCAA para poder determinar qué CCAA han sufrido más esta pandemia desde el inicio hasta el 09/03/2021 con indicadores propios de enfermedad (índice de letalidad e índice de mortalidad) y propios de esta pandemia (incidencia acumulada a 7 y 14 días).

El proceso realizado ha sido el siguiente:
Recopilación de información de las páginas web indicadas anteriormente
Análisis de datos: La mayoría de los datos de los que disponía eran cuantitativos por lo que he realizado operaciones de agrupación, conteo, sumatorio. Todo el análisis y tratamiento de datos se puede ver en el notebook COVID19
Presentación de los resultados obtenidos en streamlit. El código está en la carpeta streamlit. Para ver la ejecución en streamlit, una vez abiertos los notebooks, hay que poner en la terminal streamlit run main.py
Todo el código está escrito en Python utilizando notebooks de Jupyter y el IDE de PyCharm para streamlit.

Las gráficas generadas, la mayor parte de ellas interactivas, se pueden visualizar en la carpeta img.

## Estudio de la evolución del SARS-CoV-2 en España desde el 01/01/2020 hasta el 09/03/2021 según datos científicos del Instituto Carlos III

Quería realizar un estudio 100% científico de la evolución del SARS-CoV-2 en España debido al antes y después que hemos experimentado y que estamos experimentando en todo el mundo en mayor o menor medida a causa del SARS-CoV-2. 

Los datasets que he usado para tal fin los he obtenido de la página web del [Instituto Carlos III](https://cnecovid.isciii.es/covid19/) y, al hacerlo, ví que no tenía datos de la población, por lo que tuve que recopilarlos de la página del [INE](https://www.ine.es/dyngs/INEbase/es/categoria.htm?c=Estadistica_P&cid=1254734710984).

Me he limitado a analizar la evolución de la pandemia y el grado de afectación al sector de la población por sexo, grupo de edad, sexo-grupo de edad en España desde el 01/01/2020 hasta el 09/03/2021. Quería analizar un poco más en profundidad y he bajado hasta el nivel de CCAA para poder determinar qué CCAA han sufrido más esta pandemia desde el inicio hasta el 09/03/2021 con indicadores propios de enfermedad (índice de letalidad e índice de mortalidad) y propios de esta pandemia (incidencia acumulada a 7 y 14 días).

### El proceso realizado ha sido el siguiente:

* Recopilación de información de las páginas web indicadas anteriormente
* Análisis de datos: La mayoría de los datos de los que disponía eran cuantitativos por lo que he realizado operaciones de `agrupación`, `conteo`, `sumatorio`. Todo el análisis y tratamiento de datos se puede ver en el notebook `COVID19`   
* Presentación de los resultados obtenidos en streamlit. El código está en la carpeta `streamlit`. Para ver la ejecución en streamlit, una vez abiertos los notebooks, hay que poner en la terminal `streamlit run main.py`

Todo el código está escrito en Python utilizando `notebooks` de Jupyter y el IDE de PyCharm para streamlit. 

Las gráficas generadas, la mayor parte de ellas interactivas, se pueden visualizar en la carpeta `img`.

<img src="img/covid.png" width="600">
