# MapMap
### Descripción
---
Aplicacíon móvil que te permite mapear rutas que recorren los vehiculos del Transporte Público de una ciudad, con el objetivo de generar datos en formato <a href="https://developers.google.com/transit/gtfs/" target="_blank">GTFS</a>. 

<strong>MapMap</strong> permite crear trazos georeferenciados sin la necesidad de consumir datos del dispositivo móvil, la información que se recolecta a través de la aplicación es la siguiente:
- Conteo de pasajeros (subida y bajada de usuarios en las paradas).
- Puntos que marcan las paradas por donde se detiene el transporte público.
- Línea de trazo que identifica una ruta.
- Tiempo inicial y final del recorrido.
- Fotografía del transporte público que realiza la ruta.

La aplicación puede ser utilizada para realizar cualquier tipo de trazo/recorrido siempre y cuando se utilicen en dispositivos con sistema operativo Android. El equipo de Codeando Xalapa agradece cualquier comentario, observación o sugerencia con respecto a la información contenida en esta aplicación y sus funcionalidades. <strong>MapMap</strong> se encuentra disponible para su descarga en la tienda oficial de aplicaciones para sistema operativo Android siguiendo esté <a href="https://play.google.com/store/apps/details?id=org.codeandoxalapa.mapmap&hl=es" target="_blank">enlace</a>.


### Problemática
---
En un gran porcentaje de las ciudades latinoamericanas el transporte público se brinda a través de concesiones por medio del sector privado, esto implica un desconocimiento del número de concesiones que transitan por las ciudades, los itinerarios son irregulares así como las rutas por donde circulan los camiones. El no conocer las rutas genera un serio problema para la movilidad de las personas y la administración pública al no lograr gestionar adecuadamente el transporte público de una ciudad.


### Contexto
---
En la ciudad de Xalapa llevamos a cabo el ejercicio del <a href="https://mapaton.org" target="_blank">Mapatón Ciudadano</a> con la colaboración de la sociedad civil (Codeando Xalapa), 400 personas participantes, gobierno municipal y asociaciones como Open Street Map, WRI, entre otras. 

Este ejercicio consistió en el uso de tecnologías de posicionamiento geográfico (GPS) a través del uso de <strong>MapMap</strong> para la recolección de datos que permitieron crear feeds de las rutas de transporte público liberando esta información en formato abierto (GTFS, JSON, GIS, Shapefiles y GeoJSON) permitiendo ser utilizados por sistemas de navegación y buscando que el uso de los datos liberados permitan mejorar la movilidad de una ciudad. 
> MapMap está diseñada para el mapeo de rutas de transporte público de la ciudad de Xalapa, pero puede ser ajustada, implementada y reutilizada para el trazado de cualquier tipo y en otras ciudades.


### ¿Cómo se utiliza?
---
El equipo de Codeando Xalapaa creó un manual de usuario que explica paso a paso cómo utilizar MapMap para realizar el mapeo de una ruta de Transporte Público, puedes descargar el manual en formato PDF
[https://mapaton.org/docs/Manual_de_Usuario_MapMap.pdf](https://mapaton.org/docs/Manual_de_Usuario_MapMap.pdf) 


### Tecnología
---
* Java 1.6 en adelante - [Descargar](http://www.oracle.com/technetwork/es/java/javase/downloads/index.html)
* Protocol Buffer Java 2.4.1 - [Descargar](https://github.com/google/protobuf/releases/tag/v2.4.1) 
* Android SDK, versión mínima 2.2 (Api Level 8) - [Descargar](https://developer.android.com/studio/index.html)
* IDE Eclipse for Android Developers - [Descargar](http://www.eclipse.org/downloads/packages/eclipse-android-developers-includes-incubating-components/neon3) 


### Ambiente de desarrollo
---
Si lo que deseas es utilizar el proyecto como desarrollador lo primero que debes hacer el preparar tu ambiente de desarrollo para poder realiar pruebas, detectar posibles errores e incluso proponer mejoras.

1. Instalar Java 1.6 en adelante y agregar variables de entorno
  * https://docs.oracle.com/cd/E19182-01/820-7851/inst_cli_jdk_javahome_t/
2. Instalar Android SDK
  * http://www.androidcentral.com/installing-android-sdk-windows-mac-and-linux-tutorial
3. Instar IDE Eclipse (Android Developer)
  * http://www.eclipse.org/downloads/packages/eclipse-android-developers-includes-incubating-components/neon3
4. Agregar plugin de Android a IDE Eclipse
  * https://stuff.mit.edu/afs/sipb/project/android/docs/sdk/installing/installing-adt.html
  * http://www.theserverside.com/tutorial/Step-by-step-guide-to-Android-development-with-Eclipse
5. Importar proyecto Android a IDE Eclipse
  * http://programmerguru.com/android-tutorial/how-to-import-android-project-in-eclipse/
6. Crear AVD (Android Virtual Device)
  * https://www.embarcadero.com/starthere/xe5/mobdevsetup/android/en/creating_an_android_emulator.html
  * http://theopentutorials.com/tutorials/android/how-to-create-android-avd-emulator-in-eclipse/

_**En caso de tener un dispositivo móvil físico no es necesario realizar el paso no.6**_


### Contribuyentes:
---
[![](https://mapaton.org/images/small-logo-codeandoxalapa-readme.png)](https://github.com/codeandoxalapa) Codeando Xalapa
* Rolando Drouaillet Pumarino
* Juan Manuel Becerril del Toro
* Elizabeth Montenegro Ñeco
* Elías Martín Sánchez Jímenez


### Agradecimiento:
---
Agradecemos a todos los miembros que pertenecen a la comunidad de Codeando Xalapa por contribuir en este proyecto. También agradecemos al proyecto [TransitWand](https://github.com/conveyal/transit-wand) por haber creado la aplicación móvil que sirvió como base para construir MapMap.


### Licencia
---
The MIT License (MIT)
Copyright (c) 2017 Codeando Xalapa


#### <i>Happy Coding!</i>