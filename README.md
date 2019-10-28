*Esta herramienta digital está publicada en la página web de la iniciativa [Código para el Desarrollo](http://code.iadb.org/es/repositorio/45/mapmap)*
# MapMap
### Descripción
---
Aplicación móvil que te permite <i>mapear</i> rutas que recorren los vehículos del Transporte Público de una ciudad, con el objetivo de generar datos en formato <a href="https://developers.google.com/transit/gtfs/" target="_blank">GTFS</a>. 

<strong>MapMap</strong> permite crear trazos georeferenciados sin la necesidad de consumir datos del dispositivo móvil, la información que se recolecta a través de la aplicación es la siguiente:
- Conteo de pasajeros (subida y bajada de usuarios en las paradas).
- Puntos que marcan las paradas por donde se detiene el transporte público.
- Línea de trazo que identifica una ruta.
- Tiempo inicial y final del recorrido.
- Fotografía del transporte público que realiza la ruta.

La aplicación puede ser utilizada para realizar cualquier tipo de trazo/recorrido siempre y cuando se utilicen en dispositivos con sistema operativo Android. El equipo de Codeando Xalapa agradece cualquier comentario, observación o sugerencia con respecto a la información contenida en esta aplicación y sus funcionalidades.


### Problemática
---
En un gran porcentaje de las ciudades latinoamericanas el transporte público se brinda a través de concesiones por medio del sector privado, esto implica un desconocimiento del número de concesiones que transitan por las ciudades, los itinerarios son irregulares así como las rutas por donde circulan los camiones. El no conocer las rutas genera un serio problema para la movilidad de las personas y la administración pública al no lograr gestionar adecuadamente el transporte público de una ciudad.


### Contexto
---
En la ciudad de Xalapa, Veracruz; la organización civil <a href="http://codeandoxalapa.org">Codeando Xalapa</a> llevó a cabo el ejercicio del <a href="https://mapaton.org" target="_blank">Mapatón Ciudadano</a> con la colaboración del Ayuntamiento de la Ciudad de Xalapa, 400 personas participantes y asociaciones como Open Street Map, WRI, Mapillary, entre otras. 

Éste ejercicio consistió en el uso de tecnologías de posicionamiento geográfico (GPS) a través del uso de <strong>MapMap</strong> para la recolección de datos que permitieron crear feeds de las rutas de transporte público liberando esta información en formato abierto (GTFS, JSON, GIS, Shapefiles y GeoJSON) permitiendo ser utilizados por sistemas de navegación y buscando que el uso de los datos liberados permitan mejorar la movilidad de una ciudad.<br><br>
:heavy_exclamation_mark: Importante:
> MapMap está diseñada para el mapeo de rutas de transporte público de la ciudad de Xalapa, pero puede ser ajustada, implementada y reutilizada para el trazado de rutas de transporte o cualquier otro tipo de trazado y en cualquier ciudad.


### Tecnología
---
* Java 1.6 hasta Java 8 - [Descargar](http://www.oracle.com/technetwork/es/java/javase/downloads/index.html)
* Protocol Buffer - [Descargar](https://marketplace.eclipse.org/content/protobuf-dt) 
* Android SDK, versión mínima 2.2 (Api Level 8) - [Descargar](https://developer.android.com/studio/index.html)
* IDE Eclipse for Android Developers - [Descargar](http://www.eclipse.org/downloads/packages/eclipse-android-developers-includes-incubating-components/neon3) 


### Ambiente de desarrollo
---
Si lo que deseas es utilizar el proyecto como desarrollador lo primero que debes hacer el preparar tu ambiente de desarrollo para poder realiar pruebas, detectar posibles errores e incluso proponer mejoras.
```
1. Instalar Java 1.6 en adelante y agregar variables de entorno
  * https://docs.oracle.com/cd/E19182-01/820-7851/inst_cli_jdk_javahome_t/
```
```
2. Instalar Android SDK
  * https://developer.android.com/studio/install.html
```
```
3. Instalar IDE Eclipse (Android Developer)
  * http://www.eclipse.org/downloads/packages/eclipse-android-developers-includes-incubating-components/neon3
```
```
4. Agregar plugin de Android a IDE Eclipse
  * https://stuff.mit.edu/afs/sipb/project/android/docs/sdk/installing/installing-adt.html
  * http://www.theserverside.com/tutorial/Step-by-step-guide-to-Android-development-with-Eclipse
```
```
5. Instalar Protocol Buffer
  * https://github.com/google/protobuf/releases/tag/v2.4.1
  * https://marketplace.eclipse.org/content/protobuf-dt
```
```
6. Crear AVD (Android Virtual Device)
  * https://www.embarcadero.com/starthere/xe5/mobdevsetup/android/en/creating_an_android_emulator.html
  * http://theopentutorials.com/tutorials/android/how-to-create-android-avd-emulator-in-eclipse/ 
```
> **En caso de tener un dispositivo móvil físico no es necesario realizar el paso número 6**


### Instalación
---
Teniendo los archivos descargados y listo el ambiente de desarrollo:<br>
1) En Eclipse, pulse <strong>Archivo</strong> > <strong>Importar</strong>.
2) En la página Seleccionar del recuadro de diálogo Importar, seleccione Android y después <strong>Proyectos Android existentes en el Espacio de trabajo</strong> en el recuadro de lista, pulse <strong>Siguiente</strong>.
3) En la página Importar proyectos del recuadro de diálogo Importar, verifique si la opción <strong>Seleccionar directorio raíz</strong> está seleccionada y, a continuación , pulse el botón <strong>Examinar</strong> de esta opción.
4) En el recuadro de diálogo <strong>Examinar</strong> para buscar carpeta, vaya a la ubicación donde guardo los archivos del proyecto descargados y selecciónelo.
5) Pulse <strong>Finalizar</strong>.
> Importar proyecto Android a IDE Eclipse, tutorial <a href="http://programmerguru.com/android-tutorial/how-to-import-android-project-in-eclipse/">aquí</a>. 
> <strong>MapMap</strong> se encuentra disponible para su descarga en la tienda oficial de aplicaciones para sistema operativo Android:<br> 
<a href="https://play.google.com/store/apps/details?id=codeandoxalapa.org.mapmap" target="_blank"><img src="https://mapaton.org/server/public/images/en_app_rgb_wo_45.png"></a>.

Una vez importado el proyecto podrá correr la aplicación desde un dispositivo virtual ó bien desde un dispositivo móvil con sistema Android.


### ¿Cómo se utiliza?
---
El equipo de Codeando Xalapa creó un manual de usuario que explica paso a paso cómo utilizar MapMap para realizar el mapeo de una ruta de Transporte Público, puedes descargar el manual en formato PDF
[https://mapaton.org/docs/Manual_de_Usuario_MapMap.pdf](https://mapaton.org/docs/Manual_de_Usuario_MapMap.pdf) 


### Metodología
---
<strong>MapMap</strong> fue utilizada en el ejercicio del <a href="https://mapaton.org" target="_blank">Mapatón Ciudadano</a>, esté mapeo colaborativo realizado en el ciudad de Xalapa dió como resultado una propuesta metodológica para realizar el trazado de rutas de transporte público en <strong>cualquier ciudad que quiera implementarlo</strong>, se divide en 3 apartados:<br><br>
1. <strong>Previo al Trazado</strong><br>
 <code>1.1.</code> Tener identificado brigadistas (personas que harán el trazado).<br>
 <code>1.2.</code> Tener un primer acercamiento con checadores y choferes, desde los puntos más importantes que concentran rutas.<br>
 <code>1.3.</code> Identificar los puntos de inicio y fin.<br>
 <code>1.4.</code> Mapear las rutas en papel (fieldpapers.org), en la medida de lo posible.<br>
 <code>1.5.</code> Verificar si en los periodos de tiempo en lo que se quiere realizar el trazado se van a presentar eventos extraordinarios.<br>
 <code>1.6.</code> Identificar las zonas geográficas.<br>
 <code>1.7.</code> Organizar brigadas de voluntarios por zonas y rutas.<br>
 <code>1.8.</code> Asignar líderes a la brigadas de voluntarios.<br>
 <code>1.9.</code> Probar MapMap en una ruta seleccionada antes de iniciar el proceso.<br>
 <code>1.10.</code> Capacitar a las brigadas de voluntarios (ver manual de usuario).<br>
 <code>1.11.</code> dentificar horarios y días en los que hay disponibilidad el servicio de transporte público.<br><br>
2. <strong>Durante el Trazado</strong><br>
 <code>2.1.</code> Organizar las brigadas de voluntarios por parejas.<br>
 <code>2.2.</code> Cubrir todas las rutas.<br>
 <code>2.3.</code> Realizar y repetir el trazado de ruta.<br>
 <code>2.4.</code> Los líderes de brigadas deben estar en contacto con sus brigadas de voluntarios.<br>
 <code>2.5.</code> Reportar el progreso del trazado por parte de los brigadistas voluntarios a los líderes de brigada.<br><br>
3. <strong>Posterior al Trazado</strong><br>
 <code>3.1.</code> Recopilar la información resultado del trazado en el repositorio.<br>
 <code>3.2.</code> Las brigadas de voluntarios deben informar a sus líderes que concluyeron el proceso de trazado.<br>
 <code>3.3.</code> Los líderes deben llevar un registro de la zonas y rutas a su cargo que han sido trazadas por completo.<br>
 <code>3.4.</code> La información deben ser verificada y contrastada con la cartografía de la zona geográfica que fue trazada.<br><br>
> Existe una versión extendida de la metodología la cual se puede ver en: <a href="https://mapaton.org">mapaton.org</a>.


### Manejo de datos
---
Una vez que utilizaste MapMap para realizar el mapeo de una ruta de transporte público la información de la(s) ruta(s) se encuentra(n) dentro de la aplicación MapMap y por tal motivo no es posible utilizar esos datos en un formato estandarizado e interpretable por sistemas de geo referencia como QGIS, Open StreetMap, Google Maps, entre otros. Para poder disponer y manejar los datos es necesario contar con la infraestructura de almacenamiento así como de conversión de datos y realizar un proceso de limpieza a los datos almacenados.
<br><br>
Escoger servidor de almacenamiento:<br>

1) Servidor Público dentro de la web del Mapatón Ciudadano (https://mapaton.org/mapmap):  Esté servidor permite almacenar y concentrar las rutas mapeadas para visualizarlas sobre un tile de Open Street Map (OSM) y conversión en formato Shapefile (.shp) y comma-separated values (.csv).

<img src="https://mapaton.org/libs/images/principal.png" with="100%" align="middle" title="Route" />

2) Instalar tu propio servidor: Utilizando el código abierto de TransitWand puedes controlar y modificar el proceso de almacenamiento, visualización y conversión de datos sin depender de un servicio que a pesar de ser público y gratuito podría dejar de funcionar en cualquier momento. Ver como instalar tu propio servidor desde esté <a href="https://github.com/codeandoxalapa/mapmap/tree/master/server">enlace</a>.


### Limpieza de datos
---
Una vez que los datos se encuentran concentrados en la infraestructura de almacenamiento es posible descargarlos en dos formatos (.shp, .csv) para su uso.


#### Descargar datos
Lo único que se requiere es ingresar el código de seis dígitos que la aplicación proporciona para identificar el dispositivo que fue utilizado para realizar el mapeo y darle click al botón ENVIAR. Una vez enviado los datos, las rutas se pueden consultar desde la plataforma (https://mapaton.org/mapmap).<br><br>
<img src="https://mapaton.org/libs/images/home.jpg" with="300px" align="middle" title="Route" />
<br><br>
Una vez que ingresaste tu código es posible descargar los datos, seleccionando la ruta que deseas descargar en el formato que tú indiques.<br><br>
<img src="https://mapaton.org/libs/images/interna.png" with="100%" align="middle" title="Route" />


#### Convertir ShapeFiles a GEOJSON
Al contar con la información descargada en formato Shapefile (.shp) es posible realizar un proceso de conversión a otros formatos como por ejemplo Geojson (http://geojson.org/) que nos permite utilizar y manipular los datos con lenguajes de programación como Javascript y realizar interfaces de consulta para visualizar las rutas. <br><br>
Para realizar ese proceso adicional de conversión que se encuentra fuera de Transitwand se puede hacer uso de otras herramientas Open Source (https://ogre.adc4gis.com/), el resultado de aplicar estás herramientasse puede observar en el siguiente enlace en donde se encuentra una ruta en formato Geojson (https://github.com/codeandoxalapa/mapmap/blob/master/data/001/route/route.geojson).
Ejemplo de un geojson obtenido de <strong>MapMap</strong>:<br><br>
<img src="https://mapaton.org/libs/images/example_geojson.png" with="100%" align="middle" title="Route" />


#### Publicación en datos abiertos
Una vez que se dispone de los datos en formato estandarizado y abierto se puede realizar una publicación de la información recolectada. En el caso de Mapatón Ciudadano las rutas de transporte público se publicaron en dos plataformas mexicanas para la publicación de datos abiertos, estas son:
  * http://datamx.io/dataset/rutas-de-transporte-publico-en-xalapa
  * https://datos.gob.mx/busca/dataset/rutas-tranporte-publico

Es importante mencionar:<br>
```
En ambas plataformas los datos pueden ser descargados y utilizados de manera libre y gratuita.
```
```
El Ayuntamiento de la Ciudad de Xalapa realizó la publicación en https://datos.gob.mx.
```
De esa forma la información puede ser utilizada y compartida para futuros proyectos, investigaciones académicas, análisis y planeación de movilidad urbana, entre otros.
> Existe una versión extendida del proceso de limpieza de datos la cual se puede ver en: <a href="https://mapaton.org">mapaton.org</a>. Actualmente no está publicada porque se encuentra en un proceso de rediseño, se espera tenerla pública próximamente.


### Análisis de calidad
---
De acuerdo al sistema de evaluación de software definido en la guía de ciclo de vida de desarrollo de software, el análisis de esta herramienta ha generado la siguiente evaluación:

Blocker issues: 4 (> 0) <strong>Low</strong> <br>
Duplicated lines: 9.5% (< 15%) <strong>Hard</strong> <br>
Critical issues: 49 (> 20) <strong>Standard</strong> <br>
Technical debt: 5d (< 10d) <strong>Hard</strong> <br>
Test coverage: 0% (< 10%) <strong>Low</strong> <br>

<img src="https://mapaton.org/libs/images/sonar_result1.png" with="100%" align="right" title="Route" /><br>
Más información en este <a href="https://el-bid.github.io/software-life-cycle-guide/delivery/evaluation-matrix/">enlace</a>.


### Autores:
---
[![](https://mapaton.org/libs/images/small-logo-codeandoxalapa-readme.png)](https://github.com/codeandoxalapa)
* Rolando Drouaillet Pumarino
* Juan Manuel Becerril del Toro
* Elizabeth Montenegro Ñeco
* Elías Martín Sánchez Jímenez


### Información adicional
---
Un ejemplo de los trazos y archivos que pueden ser realizados con <strong>MapMap</strong> son:<br><br>
* Visor de rutas - https://mapaton.org/rutas/
* Servidor para administrar rutas y generar archivos Shapefiles|CSV - http://mapaton.org/mapmap
* Geojson - https://github.com/codeandoxalapa/mapmap/tree/master/data
* Datos en <a href="https://www.mapillary.com/app/user/xalapa?lat=19.533702607228946&lng=-96.84397948833018&z=11.389325293212847&username%5B%5D=xalapa">Mapillary</a>
<br><br>
o bien, un resultado visual (ejemplo de una ruta): 
<img src="https://mapaton.org/libs/images/ejemplo_route.png" with="100%" title="Route" />


### Licencia
---
Licencia MIT [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)


### Agradecimiento:
---
Agradecemos a todos los miembros que pertenecen a la comunidad de <a href="http://codeandoxalapa.org/">Codeando Xalapa</a> por contribuir en este proyecto. También agradecemos al proyecto [TransitWand](https://github.com/conveyal/transit-wand) por haber creado la aplicación móvil que sirvió como base para construir <strong>MapMap</strong>.

#### <i> Happy Coding!</i>
<img src="https://mapaton.org/libs/images/back.png" with="100%" title="Route" />
