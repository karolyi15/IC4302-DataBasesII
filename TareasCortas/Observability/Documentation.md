**Instituto Tecnologico de Costa Rica**
**Escuela de Ing. Computacion**
**IC4302 - Bases de Datos 2**
**Gunther Karolyi**
**2017238873**
**Grupo 01**

# Guia de Instación

A continuacion, se presentan los pasos a seguir para ejecutar correctamente el proyecto Observability.
Esta guia de pasos supone que el usuario tiene instalado el programa Docker Desktop y utiliza el sistema operativo windows.

1. Instacion del Comando Scoop
   Para instalar el command scoop en windows, es necesario utilizar el power-shell y ejecutar los siguientes comandos.

   * **Set-ExecutionPolicy RemoteSigned -scope CurrentUser**
   * **iwr -useb get.scoop.sh | iex**

2. Habilitar Kubernetes en Docker
   Es necesario iniciar Docker Desktop e ingresar a la seccion de ajustes. Seguidamente seleccionar la opcion de kubernet desde el menu lateral izquierdo y finalmente seleccionar la opcion de habilitar kubernetes.

3. Instacion de Kubectl
   Para iniciar con la instación, es necesario abrir el power-shell de windows e ingresar el siguiente comando.

   * **scoop install kubectl**

4. Instacion de Helm
   Nuevamente en el power-shell introducimos el comando:

     * **scoop install helm**
    
    Esto nos va a permitir iniciar con la creacion de los helm charts.

# Creacion de Helm Charts

Inicialmente, es necesario la creacion de un directorio en donde se desarrollara el proyecto. Mediante la utilizacion del commando **helm create** se procede a crear el chart de databases y el chart de monitoring.
Una vez creados, es necesario añadir los repositorios requeridos para la utilizacion de las dependecnias necesarias. Mediante el commando **helm search** se puede encontrar las versiones de los charts.
Una vez se tenga esto configurado, se procede con la edicion de los archivos chart.yml y values.yml, en donde se estableceran las configuraciones deseadas.

# Conclusiones

Debido a la falta de datos de prueba, las conclusiones se enforan principalmente en los beneficios y optimizacion que se genera en la desarrollo de software mediante la utilizacion de las tecnologias utilizadas en el proyecto.
Una de las principales ventajas comprobadas es la facilidad y la eficiencia con la que se puede automatizar procesos de desarrollo. Tambien, se destaca la gran eficiencia en la utilizacion de recursos, ya que desde el mismo chart se pueden asignar los recursos a utilizar, limitando las aplicacion de alto consumo. Esta claro que esto es un benefico consecuente debido al aislamiento que se logra mediante el uso de contenedores.
Finalmente, se evidencio que mediante la utilizacion de estas tecnologias se logran aspectos tales como el bussiness continuity, debido que permite la utilizacion de replicas de las bases de datos con gran facilidad y mantener el sistema corriendo la mayor parte del tiempo.

# Repositorio

Favor revisar el repositorio para encontrar la ultima version existente de la documentacion.

**https://github.com/karolyi15/IC4302-DataBasesII.git**
