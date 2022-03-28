# Challenge reactor-core - solucion en tests


<p align="center">
<img src="https://www.sofka.com.co/wp-content/uploads/2021/02/sofkau-logo-horizontal.png">
</p>
<p align="center">
  <img src="https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=java&logoColor=white">
</p>
<p align="center">
  <img src="https://img.shields.io/github/v/release/JoseNSoler/PracticaMVC?style=flat-square"
</p> 


# Descripcion general

Dentro del código se encuentra un ejemplo para aplicar reactividad con Spring Boot, se cuenta con una herramienta utilitaria para leer archivos CSV, lo que se buscar es aplicar los operadores reactivas para leer este archivo, y se reta para hacer este procedimiento en mongodb.


Se implementan los requerimientos especificados por medio de unitTest:
- A partir de una lista de datos de jugadores se debe realizar consultas y/o operaciones que permita filtrar y ordenar los jugadores, se debe consultas los jugadores mayores a 34 años, jugadores filtrados por un club especifico.
- Consular las nacionalidades de los jugadores, crear una lista de las nacionalidades y un rancking de los jugadores por cada pais que se tengan en la lista.


Leer las pruebas unitarias.


# Step by Step

- Transformar un CSV una lista de Stream de Java (Usar operadores basicos)
- En vez de usar Java Stream aplicamos reactividad (Reactor Core) con trasnformaciones (Usar operadores basicos)
- Optimizar las consultas y aplicar un servicio web para hacer estos filtros
- Hacer un proceso de migración en donde tomemos los datos del archivo y lo llevemos a una base datos (MangoDB)
- Trabajo directamente los desde una base de datos reactiva y objserva la rendimiento
- Prueba de concurencia con JMeter, donde vamos a colocar 100 hilos de ejeucución para observar los comportamientos de cada servicio
