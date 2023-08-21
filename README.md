# AREP-Taller-1
En este taller se tuvo como objetivo realizar una aplicación para consultar películas de cine, en la cual se establece una conexión a una API externa que contiene toda la información que se requiere mostrar.

## Para ejecutar el programa

Se puede hacer uso del comando git clone y usar la URL del repositorio:
```
https://github.com/JuanPabloDaza/AREP-Taller-1
```

## Prerequisitos

Es necesario tener instalado maven para compilar y probar los test del programa, si no se tiene maven puede instalar [aqui](https://maven.apache.org/install.html).

## Instalacion 

Una vez clonado, se debe hacer uso del comando:

```
mvn package
```

Este comando compilara el programa y tambien ejecutara las pruebas. 

## Ejecutar pruebas

Si se quiere ejecutar solamente las pruebas se puede hacer uso del comando:

```
mvn test
```
Las pruebas verifican el funcionamiento del cache y de la conexion del programa a la API externa.

## Despliegue del programa:

Para ejecutar el programa se usa el comando:

```
mvn exec:java -D "exec.mainClass"="edu.escuelaing.arep.ASE.app.HttpServer"
```
Una vez ejecutado se debe acceder a traves de un buscador y con la direccion:
```
127.0.0.1:35000
```

## Construido con:

* [Maven](https://maven.apache.org/) - Manejo de dependecias.
* [OMDb API](https://www.omdbapi.com/) - API Externa

## Autor

* Juan Pablo Daza Pinzon

## Reconocimientos

* Ayuda en la construccion de la tabla para la informacion suministrada - [Juan Sebastian Rodriguez Peña](https://github.com/JSebastianRod)
* [Implementacion del Cache LRU](https://www.youtube.com/watch?v=efiWbPSinD8)