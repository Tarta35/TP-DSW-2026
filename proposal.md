# Propuesta TP DSW

## Grupo
### Integrantes
* 53136 - Caballero, Luciano
* 53269 - Leone, Lucca
* 52925 - Vella, Luca
* 53137 - Diogo Utrera

### Repositorios
* [frontend app](http://hyperlinkToGihubOrGitlab)
* [backend app](http://hyperlinkToGihubOrGitlab)


## Tema
El sistema es un gestor y administrador de articulos de una casa de subastas. En el se puede crear y registrarse en subastas online.
Tambien se puede gestionar el estado de cada articulo, a su vez su ingreso y egreso de la casa de subasta.


### Modelo
<img width="2682" height="1059" alt="Modelo de Dominio Gestion de nueva propuesta drawio (2)" src="https://github.com/user-attachments/assets/25177682-6ae6-4e6b-aa77-d9ec466eaa2e" />




Link al drive, contiene la imagen y el modelo realizado en draw.io: https://drive.google.com/drive/folders/1elOoolKdCF_jXy4o09QsKXLZrdcb7qfM?usp=sharing

## Alcance Funcional 

### Alcance Mínimo

Regularidad:
|Req|Detalle|
|:-|:-|
|CRUD simple|1. CRUD Usuario<br>2. CRUD Tag<br>3. CRUD Categoria_Articulo<br>4. CRUD <br>5. CRUD |
|CRUD dependiente|1. CRUD Subasta {depende de} CRUD Gerente<br>2. CRUD ValorTag {depende de} CRUD Tag<br>3. CRUD Subasta {depende de} CRUD Articulo<br>4. CRUD Articulo {depende de} CRUD Categoria_Articulo<br>5. CRUD Articulo {depende de} CRUD Usuario|
|Listado<br>+<br>detalle| 1. Listado de Articulo filtrado por modelo, categoria, autor, muestra nombre, descripcion => detalle muestra datos completos del articulo<br> 2. Listado de Subasta filtrado por categoria, fecha, nombre, disponibilidad => detalle muestra datos completos de la subasta|
|CUU/Epic|1. Participar de una subasta<br>2. Registro y Verificación de Perfil|


Adicionales para Aprobación
|Req|Detalle|
|:-|:-|
|CRUD |1. CRUD Usuario<br>2. CRUD Subasta<br>3. CRUD Categoria_Subasta<br>4. CRUD Articulo<br>5. CRUD Modelo<br>6. CRUD Categoria_Articulo<br>7. CRUD Autor|
|CUU/Epic|1. Participar de una subasta<br>2. Definir los detalles para aceptar y recibir el articulo<br>3. Visualizar subastas en las que se registro y administrarlas<br>4. Registro y Verificación de Perfil<br>|


### Alcance Adicional Voluntario

*Nota*: El Alcance Adicional Voluntario es opcional, pero ayuda a que la funcionalidad del sistema esté completa y será considerado en la nota en función de su complejidad y esfuerzo.

|Req|Detalle|
|:-|:-|
|Listados |1. Estadía del día filtrado por fecha muestra, cliente, habitaciones y estado <br>2. Reservas filtradas por cliente muestra datos del cliente y de cada reserve fechas, estado cantidad de habitaciones y huespedes|
|CUU/Epic|1. Consumir servicios<br>2. Cancelación de reserva|
|Otros|1. Envío de recordatorio de reserva por email|

