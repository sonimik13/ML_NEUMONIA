## Clasificación de imágenes de neumonía vírica no COVID-19, neumonía vírica COVID-19 y pulmones sanos

Uno de los problemas de los que hemos sido testigos en este tiempo ha sido la falta de alternativas eficaces - excepto el test médico - para la detección
de COVID-19. 

En cada una de las olas sufridas se han visto incrementados los casos de COVID-19 positivos y aquellos casos que presentaban incertidumbre (no confirmados) por lo que los
centros de salud y hospitales se han visto desbordados.

Esta situación es la que me ha empujado a realizar este estudio con imágenes de rayos X de COVID-19 de la Sociedad Italiana de Radiología Médica e Intervencionista (SIRM) COVID-19 DATABASE recopilados de la página web de [kaggle](https://www.kaggle.com/tawsifurrahman/covid19-radiography-database), cuyo objetivo final a perseguir era realizar la clasificación de pacientes con neumonía vírica no COVID-19, pacientes con neumonía vírica COVID-19 y pacientes con pulmones sanos.

### El proceso realizado ha sido el siguiente:

* Recopilación de imágenes de la página indicada anteriormente
* Análisis de datos: Tenía imágenes que se correspondían a 4 causístiscas pero he descartado las imágenes de opacidad pulmonar porque no me iban a servir para discriminar la neumonía correctamente ya que las personas con ese episodio podían tener su origen en una neumonía u otra enfermedad. También he tenido que balancear los datos, ya que tenía una cantidad mayor de muestras de pacientes con pulmones sanos por lo que el modelo no iba a generalizar bien si cogía todas las muestras de las que disponía. 

Todo el código está escrito en Python utilizando Google colab.

