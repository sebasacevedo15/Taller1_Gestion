#######################
TALLER 1 GESTION DE DATOS
Daniela Rocio Rubio
Israel Steven Orozco
Juan Sebastian Acevedo

Link Video: https://youtu.be/eGY8IYMxsn0

Para el taller se seleccionan datasets 
	Secuestro
	Homicidios
	Hurto
	Terrorismo

1.Al realizar un análisis de la calidad de los datos en los diferentes datasets se encuentran diferentes formatos en la representación del código del DANE, por lo cual es necesario establecer un formato unico para los datasets, se analiza de igual manera datos homónimos, donde se encuentran algunas columnas con datos como "NO REPORTA" y "NO REPORTADO". Se decide dejar uno de los dos.
De igual manera se analizan datos nulos pero no se encuentran en el Dataset
Se estandariza el nombre de dptos y municipios segun estandar de DANE


2. Responda las siguientes preguntas
2.1. ¿Cuáles han sido los departamentos (TOP 3) más afectados en términos de cantidad de delitos cometidos en los últimos 5 años?
HOMICIDIOS
ANTIOQUIA	4393
VALLE DEL CAUCA	3855
BOGOTA D.C.	2582

TERRORISMO
ANTIOQUIA	241
ARAUCA	173
NORTE DE SANTANDER	172

HURTO
CUNDINAMARCA	2628
CESAR	1552
META	1326

SECUESTRO
ANTIOQUIA          4558
CESAR              2093
VALLE DEL CAUCA    1861

2.2. Para los casos en los que aplique, ¿cuál ha sido el arma o medio más común para cometer el delito?
HOMICIDIOS
VEHICULO               34319

TERRORISMO
ARTEFACTO EXPLOSIVO/CARGA DINAMITA    1638

HURTO
SIN EMPLEO DE ARMAS            12748

SECUESTRO
No Aplica

2.3. Para los casos en los que aplique, ¿cómo ha sido la proporción de géneros y grupos etarios que han estado involucrados en este tipo de delito? ¿Han variado con el paso de los años?
HOMICIDIOS GENERO
GENERO
FEMENINO        12319
MASCULINO       47431
NO REPORTADO       60

GRUPO ETARIO
ADOLESCENTES     2924
ADULTOS         54671
MENORES          2170
NO REPORTADO       45

TERRORISMO
No Aplica

HURTO
GENERO
FEMENINO         5951
MASCULINO       26649
NO REPORTADO     3541

GRUPO ETARIO
ADOLESCENTES       12
ADULTOS         32482
MENORES            18
NO REPORTADO     3399
Valiendome de una tabla resumen en la que esta por año la cantidad e hurtos cometidos por cada genero y grupo etario, se concluye que en su gran mayoría son cometidos por adultos masculinos con un aparticipacion de mas del 70% porcentaje que no varia muhco año tras año, seguido por las mujeres adultas.

SECUESTRO
No Aplica

2.4. ¿Se evidencia alguna tendencia para cometer dicho delito en algún mes particular del año?
HOMICIDIOS
Enero     2918
En enero se cometen más delitos que en los demás meses

TERRORISMO
Febrero     191

HURTO
Enero     1914

SECUESTRO
Mayo     2546

2.5. Para los casos en los que se disponga del detalle del delito o de una descripción, como por ejemplo en delitos sexuales y secuestro, ¿cuáles son las descripciones o modalidades más comunes?
HOMICIDIOS
ARTÍCULO 109. HOMICIDIO CULPOSO ( EN ACCIDENTE DE TRÁNSITO)        59800
ARTÍCULO 110. HOMICIDIO CULPOSO ( CIRCUNSTANCIAS DE AGRAVACIÓN)       10

TERRORISMO
No Aplica 

HURTO
No Aplica

SECUESTRO
SECUESTRO EXTORSIVO    11816
SECUESTRO SIMPLE        6826


3.Se realizan agrupaciones para el df de homicidios y se normaliza por cantidad de habitantes, donde se encuentra que debido a la gran población de bogotá la cantidad de homicidios per capita es muy pequeña a comparación de los demás municipios

2017  ANTIOQUIA          0.015800
      BOGOTA D.C.        0.000065
      VALLE DEL CAUCA    0.009058
2018  ANTIOQUIA          0.016072
      BOGOTA D.C.        0.000069
      VALLE DEL CAUCA    0.010566
2019  ANTIOQUIA          0.016322
      BOGOTA D.C.        0.000069
      VALLE DEL CAUCA    0.010827
2020  ANTIOQUIA          0.014847
      BOGOTA D.C.        0.000054
      VALLE DEL CAUCA    0.005980
2021  ANTIOQUIA          0.025748
      BOGOTA D.C.        0.000067
      VALLE DEL CAUCA    0.009420
2022  ANTIOQUIA          0.007383
      BOGOTA D.C.        0.000024
      VALLE DEL CAUCA    0.002463

4. Se realiza un merge por municipio de más de un millon de habitantes para los diferentes dataset, se tiene genera un dataset llamado mergefinal en el cual se observa que los datos para los diferentes tipos de delito se encuentran muy cercanos. Se realiza análisis gráfico en python.
