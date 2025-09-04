# Parcial_Distribuidos

# Autor
**Diego Alejandro Gil Otálora**  
Código: 202222152  
Universidad Pedagógica y Tecnológica de Colombia  
Ingeniería de Sistemas y Computación - Sistemas Distribuidos  
Tunja, 2025  

---

## Ejercicio 1 — Imagen Personalizada

![alt text](image.png)

![alt text](image-10.png)

- Corriendo el contenedor
![alt text](image-11.png)


## Ejercicio 2 — Persistencia con volumenes

- Crear el volumen 

![alt text](image-1.png)

- Crear el contenedor de postgres

![alt text](image-2.png)

- Creacion de tabla y registros

![alt text](image-3.png)
![alt text](image-4.png)

- Eliminando contenedor y levantando otro con el mismo volumen. (Verificando que los datos siguen ahi)

![alt text](image-5.png)



## Ejercicio 3 — Bind mount y edicion en vivo

- Creacion de un directorio con un archivo (index.html)

![alt text](image-6.png)

- Ejecutando contenedor nginx para servir archivo mediante bind mount de solo lectura

![alt text](image-7.png)

- Acceder al navegador mediante http://localhost:8080
(Para este ejercicio cambie 8080 por 8090 ya que no queria generar algun conflicto con un contenedor ya existente corriendo en ese puerto)

![alt text](image-8.png)

- Modificando el index.htm y mostrando el cambio 

![alt text](image-12.png)


## Ejercicio 4 — Exploracion de contenedores

- Ejecutando en modo interactivo, creando archivos, mostrando ruta de trabajo y listando archivos

![alt text](image-16.png)
se demuestra que existe tanto notas.txt como mensaje.txt

- Saliendo del contenedor, eliminandolo y levantando otro con la misma imagen

![alt text](image-17.png)
Se evidencia que notas.txt ya no existe. Supongo que por falta de persistencia (volumenes o bind mounts)

## Ejercicio 5 — Redis con Dockerfile

- Construyendo la imagen con nombre personalizado (diegoalejandrogil22)

![alt text](image-13.png)

- Levantando el contenedor en segundo plano a travez de la imagen

![alt text](image-14.png)

- Revisando los logs del contenedor

![alt text](image-15.png)

