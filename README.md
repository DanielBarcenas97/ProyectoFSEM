### UNIVERSIDAD NACIONAL AUTÓNOMA DE MÉXICO
### FACULTAD DE INGENIERÍA
### Fundamentos de Sistemas Embebidos

## Proyecto final: "Centro Multimedia con conexion a servicios de streming populares"
    Usa Python 3.73 y la libreria PyQt5

### Semestre 2022-1
### Integrantes:
    Barcenas Martinez Edgar Daniel
    Garcia Reyes Saúl Michel
    Hernández Rodríguez Alejandro
    
## Objetivo.
Desarrollar a través de código Python compartible con el sistema operativo Raspbian un centro de entretenimiento para la reproducción de películas, videos, música, y fotografías.
    
## Configuración de la tarjeta Raspberry e instalación del software.
### 1. Recomendaciones para la instalación de Raspbian en VirtualBox.

    A) Raspberry PI Modelo 2 o un software de virtualización.
    B) Imagen ISO de Raspbian.
    C) Tarjeta flash de al menos 5 GB o mayor a este tamaño.
    D) Memoria RAM de al menos 512 MB y memoria gráfica de 64 MB.
    
### 2. Descarga de ISO de Raspbian. 

Ir a la página https://www.raspberrypi.org/ y en la sección de descargas, descargar la ISO del sistema operativo último que se tenga.

<p align="center">
  <img src="https://user-images.githubusercontent.com/95458811/146435752-813b51d0-8ec1-4861-ae21-66d157a4486a.PNG" width="500" alt="Sublime's custom image"/>
</p>

### 3. Instalación en VirtualBox.

A) Creación de la máquina virtual (nombre, carpeta, tipo, versión (se recomienda 64 bits), tamaño de memoria y disco duro).
    
<p align="center">
  <img src="https://user-images.githubusercontent.com/95458811/146436483-518bb3cb-83b2-401e-b131-e962452a2007.PNG" width="400" alt="Sublime's custom image"/>
</p>

B) Creación del disco duro virtual (ubicación de archivo, tamaño de archivo, tipo de archivo de disco duro, almacenamiento en unidad de disco duro).

<p align="center">
  <img src="https://user-images.githubusercontent.com/95458811/146436757-beca1b22-6e55-41e3-b736-260995cc3812.PNG" width="400" alt="Sublime's custom image"/>
</p>

C) Configuración de la máquina virtual.

-> Asociación de imagen ISO descargada (buscar y seleccionar la ISO que se descargó en el paso 2).

<p align="center">
  <img src="https://user-images.githubusercontent.com/95458811/146438152-82b3c11c-f76b-4ada-bd05-598862e9e592.PNG" width="450" alt="Sublime's custom image"/>
</p>

-- Ejemplo de seleccion de ISO descargada:

<p align="center">
  <img src="https://user-images.githubusercontent.com/95458811/146438821-12b5e275-149f-47af-8064-dd5a0a2a44ce.PNG" width="450" alt="Sublime's custom image"/>
</p>


<p align="center">
  <img src="https://user-images.githubusercontent.com/95458811/146439479-5ad0ef9a-f647-495a-bf61-049b62878fb5.PNG" width="400" alt="Sublime's custom image"/>
</p>

D) Encendido máquina virtual.

-> Inicio de máquina virtual.

<p align="center">
  <img src="https://user-images.githubusercontent.com/95458811/146440449-f74749a9-13a8-49a1-979e-a97b9591c9d9.PNG" width="300" alt="Sublime's custom image"/>
</p>

-> Inicio en modo gráfico.

<p align="center">
  <img src="https://user-images.githubusercontent.com/95458811/146440508-50d6140e-a0d0-4678-9001-ca02e29c636d.PNG" width="400" alt="Sublime's custom image"/>
</p>

-> Después de configurar el particionado de la máquina virtual, se inicia el entorno gráfico.

<p align="center">
  <img src="https://user-images.githubusercontent.com/95458811/146441116-11079e1a-43b5-4894-b739-4c017d57ec35.PNG" width="300" alt="Sublime's custom image"/>
</p>

E) Configuración para el uso de la máquina.

-> Seleccion de idioma.

<p align="center">
  <img src="https://user-images.githubusercontent.com/95458811/146442022-4ba0e66d-9c9a-4dff-a7f9-0aa836e28f22.jpeg" width="400" alt="Sublime's custom image"/>
</p>

-> Creación de contraseña para la cuenta.

<p align="center">
  <img src="https://user-images.githubusercontent.com/95458811/146442236-459040e8-21cb-4ad8-8c4c-25f18aeccd78.jpeg" width="400" alt="Sublime's custom image"/>
</p>


### 4. Comandos para configuración de la Raspberry para la ejecución correcta del proyecto.

A) Encender la Raspberry seleccionando el icono de terminal.

<p align="center">
  <img src="https://user-images.githubusercontent.com/95458811/146441696-fc7ac8af-466f-44f4-9fa1-0fc5323003dd.PNG" width="450" alt="Sublime's custom image"/>
</p>

B) Instalación de Git, comprobación de versión.

<p align="center">
  <img src="https://user-images.githubusercontent.com/95458811/146443161-9b8efdc4-03f1-4f71-b9b6-5fa741249b74.PNG" width="400" alt="Sublime's custom image"/>
</p>


<p align="center">
  <img src="https://user-images.githubusercontent.com/95458811/146443673-f02bd134-1ec3-487f-b6e6-fd759b10e271.PNG" width="350" alt="Sublime's custom image"/>
</p>

C) Configuración de Git (información personal : nombre de confirmación y dirección de correo electrónico).

-> Ejemplo para nombre de confirmación y dirección de correo electrónico.

<p align="center">
  <img src="https://user-images.githubusercontent.com/95458811/146444118-69761f03-ea63-4188-963c-725e7b7120b0.jpeg" width="450" alt="Sublime's custom image"/>
</p>

D) Descarga del repostorio del proyecto.

-> Ingresó a la carpeta o ubicación donde se exportara el repostorio (para este ejemplo la carpeta de nombre "FSEM") y descarga del mismo con el comando "git clone" seguido de la dirección https del proyecto.

<p align="center">
  <img src="https://user-images.githubusercontent.com/95458811/146445338-f6f37af6-371d-40d9-9726-6664731e79e7.jpeg" width="400" alt="Sublime's custom image"/>
</p>


<p align="center">
  <img src="https://user-images.githubusercontent.com/95458811/146445066-71ebb10e-7b1b-4a0d-b3b8-dd4c6b3c97f5.PNG" width="500" alt="Sublime's custom image"/>
</p>

### 5. Configuración del proyecto.

A) Instalación de paquetes a través de la actualización de librerías del sistema con los comandos:

    sudo apt-get update
    sudo apt-get upgrade
    
B) Instalación de paquetes (Pyqt5) para ejecutar el proyecto.

    sudo apt-get install python3-pyqt5
    sudo apt-get install qt5-default pyqt5-dev pyqt5-dev-tools
    sudo apt-get install -y python3-pyqt5.qtwebengine
    sudo apt-get install libqt5multimedia5-plugins
    sudo apt-get install python3-pyqt5.qtmultimedia
   
C) Instalación de librería para video.

    pip3 install python-vlc 

## Ejecución del Centro Multimedia y su entorno gráfico.

A) Para ejecutar el proyecto se escribe el comando:

    python3 MultimediaCenter.py
    
B) Entorno gráfico del centro multimedia.

<p align="center">
  <img src="https://user-images.githubusercontent.com/95458811/146449744-806748da-0274-45ef-845a-fb2772a6b30f.jpeg" width="500" alt="Sublime's custom image"/>
</p>

