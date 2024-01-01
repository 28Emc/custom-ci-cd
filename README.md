# custom-ci-cd

Repositorio con archivos necesarios para levantar Jenkins y SonarQube en localhost.

## INSTALACIÓN

Si es la primera vez que utlizas estas imagenes, localizarte en la raíz de este proyecto y ejecutar el siguiente comando

```bash
 docker-compose up
```

De esta forma se descargarán las imágenes necesarias y se levantarán los respectivos contenedores.

![Alt text](images/img_imagenes.png?raw=true "Imagenes")

![Alt text](images/img_contenedores.png?raw=true "Contenedores")

## RESTAURAR VOLUMENES ANTERIORES (BACKUP)

**NOTA: SE RECOMIENDA UTILIZAR "Docker Desktop" Y DESCARGAR LA EXTENSIÓN "Volumes Backup & Share" PARA SIMPLIFICAR LOS PASOS A SEGUIR**

La carpeta "/volumes" contiene los volumenes necesarios para cargar la configuración necesaria para el correcto funcionamiento de los contenedores creados anteriormente; para ello, mediante Docker Desktop, RESTAURAR los volumenes respectivos.

![Alt text](images/img_importar_volumen_desde_lista.png?raw=true "Importar volumenes desde lista")

![Alt text](images/img_seleccionar_local_file.png?raw=true "Importar desde local file")

#### EJM: el volumen "custom-ci-cd_jenkins_home" se restaura para el contenedor "jenkins-1", y así respectivamente

Una vez realizada la importación, levantar los contenedores e iniciar sesión con las siguientes credenciales:

## CREDENCIALES JENKINS

```javascript
Username: emedina
Password: emedina
```

## CREDENCIALES SONARQUBE

```javascript
Username: admin
Password: emedina
```
