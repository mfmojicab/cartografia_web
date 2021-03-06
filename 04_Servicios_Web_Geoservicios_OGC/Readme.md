# Servicios web, geoservicios y OGC

- [Servicios web, geoservicios y OGC](#servicios-web-geoservicios-y-ogc)
  - [Presentación](#presentaci%C3%B3n)
  - [Ejercicio 1: Consumiendo servicios WMS con clientes de escritorio](#ejercicio-1-consumiendo-servicios-wms-con-clientes-de-escritorio)
  - [Ejercicio 2: Consumiendo servicios WMS con clientes ligeros](#ejercicio-2-consumiendo-servicios-wms-con-clientes-ligeros)
  - [Ejercicio 3: Servicios OGC y Python](#ejercicio-3-servicios-ogc-y-python)
    - [Otros recursos sobre python](#otros-recursos-sobre-python)
    - [Ejemplos Python / Arcpy](#ejemplos-python--arcpy)

## Presentación

Enlace https://github.com/dersteppenwolf/cartografia_web/blob/master/04_Servicios_Web_Geoservicios_OGC/04_Servicios_web_geoservicios_OGC.pdf


## Ejercicio 1: Consumiendo servicios WMS con clientes de escritorio

A través de clientes SIG de escritorio como QGIS o Arcgis Desktop / pro puede consumir servicios OGC WMS y WFS

Realizar lo siguiente: 

- Ubique un servicio WMS de una entidad colombiana.  Ejemplos:
  - IGAC
    - https://geoportal.igac.gov.co/contenido/geoservicios 
    - https://geoportal.igac.gov.co/contenido/datos-abiertos-cartografia-y-geografia
  - Datos Abiertos Bogotá https://datosabiertos.bogota.gov.co/dataset?res_format=WMS
- Visualice el servicio wms que seleccionó a través de QGIS.  ( __Qgis Working with WMS Data__ http://www.qgistutorials.com/en/docs/working_with_wms.html  ).  
- Explore el mapa utilizando las herramientas de "zoom" y "pan". Ubique una zona de interés, preferiblemente no tan grande. 
- Ubique un servicio WFS de una entidad colombiana.  Ejemplos:
  - IGAC
    - https://geoportal.igac.gov.co/contenido/geoservicios 
    - https://geoportal.igac.gov.co/contenido/datos-abiertos-cartografia-y-geografia
  - Datos Abiertos Bogotá https://datosabiertos.bogota.gov.co/dataset?res_format=WFS
- Adicione la capa WFS de interés a QGIS (__WFS and WFS-T Client__  https://docs.qgis.org/3.10/en/docs/user_manual/working_with_ogc/ogc_client_support.html#wfs-and-wfs-t-client ) y asígnele una simbología.
- Genere un pdf de una zona de interés donde se puedan visualizar tanto los datos provenientes del WMS como los del WFS.
- Repita el ejercicio utilizando Arcgis Desktop o Arcgis Pro  
  - __Arcgis Desktop Adding WMS services__ http://desktop.arcgis.com/en/arcmap/latest/map/web-maps-and-services/adding-wms-services.htm 
  - __Adding a WFS service to ArcMap__ https://desktop.arcgis.com/en/arcmap/latest/map/web-maps-and-services/adding-a-wfs-service-to-arcmap.htm
  - __Arcgis Pro: Agregar servicios WFS__ https://pro.arcgis.com/es/pro-app/help/data/services/add-wfs-services.htm
- Suba los dos pdfs generados a su repositorio de Github. Comparta los urls de los geoservicios utilizados y los pdfs generados a través del chat de la clase.
  


## Ejercicio 2: Consumiendo servicios WMS con clientes ligeros

A través de clientes ligeros javascript es posible  consumir servicios OGC WMS y WFS

Ejemplo 1 leaflet y wms: 
- Vista web:  https://dersteppenwolf.github.io/cartografia_web/04_Servicios_Web_Geoservicios_OGC/html/leaflet_wms.html
- Código:  https://github.com/dersteppenwolf/cartografia_web/blob/master/04_Servicios_Web_Geoservicios_OGC/html/leaflet_wms.html

Ejemplo 2 leaflet y wms: 
- Vista web:  https://dersteppenwolf.github.io/cartografia_web/04_Servicios_Web_Geoservicios_OGC/html/leaflet_wms_2.html
- Código: https://github.com/dersteppenwolf/cartografia_web/blob/master/04_Servicios_Web_Geoservicios_OGC/html/leaflet_wms_2.html


Realizar lo siguiente: 
- A partir de los ejemplos mostrados en clase, modificar el código html / js  para cargar diferentes wms de servicios de entidades colombianas.
- Publique el html generado en github (Carpeta: ogc, Archivo: wms.html ). 
- Comparta el url del html generado (vista github pages y código en github)  a través del chat de la clase.

Ejemplos de visualización de WMS con otras herramientas basadas en javascript: 

- Visor WMS Esri Js https://developers.arcgis.com/javascript/3/samples/layers_wms/
- Mapbox Gl https://www.mapbox.com/mapbox-gl-js/example/wms/
- Carto https://carto.com/learn/guides/styling/inserting-external-basemaps/

## Ejercicio 3: Servicios OGC y Python

**OWSLib** 
http://geopython.github.io/OWSLib/ 
Librería de python para el desarrollo de clientes para servicios web basados en Open Geospatial Consortium (OGC) 

![img](img/OWSLib.png "img")

**Google Colaboratory**

**Colaboratory** es un entorno gratuito de Jupyter Notebook que no requiere configuración y que se ejecuta completamente en la nube.

Realizar lo siguiente: 
- Crear cuenta en Google Colaboratory https://colab.research.google.com/ (Requiere cuenta de gmail)
- Sigua el siguiente  ejemplo de OWSLib / python ejecutado a través de  Google Colaboratory  
- Consumiendo servicios WFS [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/dersteppenwolf/cartografia_web/blob/master/04_Servicios_Web_Geoservicios_OGC/ejemplo_python_wfs.ipynb)
-  Consumiendo servicios WMS [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/dersteppenwolf/cartografia_web/blob/master/04_Servicios_Web_Geoservicios_OGC/ejemplo_wms.ipynb)

![img](img/colab.png "img")

### Otros recursos sobre python 

- Python for beginners https://data-flair.training/blogs/start-learning-python-with-infographic/ https://d2h0cx97tjks2p.cloudfront.net/blogs/wp-content/uploads/sites/2/2019/02/Python-Infographic-for-beginners-to-learn-Python-Quickly.jpg
- Python Hello world https://www.learnpython.org/en/Hello,_World!
- Primeros pasos con Jupyter Notebook https://www.adictosaltrabajo.com/2018/01/18/primeros-pasos-con-jupyter-notebook/
- Google Colab: Python y Machine Learning en la nube https://www.adictosaltrabajo.com/2019/06/04/google-colab-python-y-machine-learning-en-la-nube/
- Utilizando python para GIS   https://twitter.com/ramiroaznar/status/1241297375903318017
- Course Files for Complete Python 3 Bootcamp Course on Udemy https://github.com/Pierian-Data/Complete-Python-3-Bootcamp
- Introducing kepler.gl for Jupyter https://medium.com/vis-gl/introducing-kepler-gl-for-jupyter-f72d41659fbf
- Python for geo-people - Fall 2016 https://github.com/Python-for-geo-people/Course-information
- Automating GIS processes course
  - 2016 https://automating-gis-processes.github.io/2016/index.html
  - 2018 https://automating-gis-processes.github.io/site/2018/
  - github https://github.com/Automating-GIS-processes/Course-information

### Ejemplos Python / Arcpy

- Python variables y operaciones: https://gist.github.com/dersteppenwolf/fca39c1971fd0fd7c3ce
- Describir feature https://gist.github.com/dersteppenwolf/6dc546ef359ffbb85947
- Buffer https://gist.github.com/dersteppenwolf/82d65df9544933289bab
- Clip https://gist.github.com/dersteppenwolf/6dae5bfd9521db50e567
