# AD-3.-Diagramas-UML
El ejercicio plantea el diseño y estructura de un programa para la gestión de torneos e-Sports basándose en un diagrama de casos de uso y uno de clases.

Actores identificados  
**Administrador del torneo:** Aquel usuario responsable de crear y organizar el torneo, premios, partidas y emparejamientos.

**Administrador de equipos:** Usuario responsable de crear el equipo y gestionar sus jugadores.

### Funcionalidades del sistema

#### Gestión de equipos y jugadores

* Registrar equipo.  
* Añadir jugadores a un equipo.  
* Consultar lista de equipos y jugadores.

#### Gestión de torneos

* Crear un torneo.  
* Inscribir equipo en un torneo.  
* Generar emparejamientos de partidas.

#### Gestión de partidas y resultados

* Registrar resultado de una partida.  
* Actualizar clasificación del torneo.

#### Gestión de premios

* Asignar premios a los ganadores.

[Esquema de casos de uso](https://github.com/Victorsuero7/AD-3.-Diagramas-UML/blob/main/Diagrams/casos-uso.png)

### 

### Entidades y relaciones

**Torneo:** representa la entidad en torno a la que gira la aplicación   
**Jugador:** Aunque no es un actor principal del sistema forma parte de la información del programa y está presente en las relaciones y agregaciones  
**Equipo:** representa una agrupación de jugadores que compiten en nombre de una entidad  
**Partida:** cada uno de los emparejamientos del torneo  
**Premio**

Un torneo está compuesto por varios equipos y varias partidas.  
Un equipo está compuesto por al menos un jugador.  
Un jugador solo puede formar parte de un equipo.  
Un torneo tiene un premio.

### Clases principales

Clases de entidad  
	Representan las unidades de información claves del programa

* Equipo  
* Jugador  
* Torneo  
* Partida  
* Premio

Interfaces de control  
Manejan la lógica y la gestión

* GestorEquipos  
* GestorTorneos  
* GestorResultados  
* GestorPremios

Interfaces de vistas  
	manejan la lógica de la representación de la informacion

* Consultar información

Clases de interfaz (Vista)  
	Permiten la visualización de información

* VistaEquipos  
* VistaTorneos  
* VistaPartidas  
* VistaPremio

[Esquema de clases](https://github.com/Victorsuero7/AD-3.-Diagramas-UML/blob/main/Diagrams/clases.png)
