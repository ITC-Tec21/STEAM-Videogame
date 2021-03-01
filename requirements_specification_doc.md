# Agustín Pumarejo Ontañón, Sebastián Juncos Leunig, Adriana Abella Kuri

# Connecting Maze / Peeprol Maze
Juego de puzzle en el que se completa un circuito con compuertas lógicas para emitir una señal.

# Table of content

- [Introduction](#introduction)
    - [Purpose](#purpose)
    - [Scope](#scope)
    - [Definitions and Acronyms](#definitions-and-acronyms)
- [Overall Description](#overall-description)
    - [User classes](#user-classes)
    - [Assumptions and Dependencies](#assumptions-and-dependencies)
- [System Features and Requirements](#system-features-and-requirements)
    - [Functional Requirements](#functional-requirements)
    - [External Interface Requirements](#external-interface-requirements)
    - [Non-functional Requirements](#non-functional-requirements)
- [Screens](#screens)
    - [Wireframes](#wireframes)

_Table of content generated using VSCode plugin [Markdown TOC](https://marketplace.visualstudio.com/items?itemName=AlanWalk.markdown-toc)_

# Introduction

## Purpose
Promover que alumnos de preparatoria o más jovenes escojan carreras STEAM al exponerlos a conceptos de lógica computacional a través de un videojuego atractivo. Se hará una captura de los resultados y mejoras de los jugadores para analizar la efectividad del juego.

## Scope
Alumnos mexicanos entre 9 y 18 años, especialmente miembros de grupos que no tienen suficiente representación en la industria de la tecnología, como las mujeres u otras minorías. 

## Definitions and Acronyms
STEAM: ciencias, tecnologías, ingeniería, artes y matemáticas (por sus siglas en inglés).
Puzzle: género de videojuegos que consiste en resolver un problema utilizando lógica y agilidad mental.

# Overall Description
Un nuevo videojuego original de circuitos donde el jugador debe escoger una combinación de compuertas lógicas para completar el nivel.

## User classes
Jugadores: Alumno que utilizará el juego
Analista de STEAM: Miembro de la OSF que verá el progreso de los jugadores en el juego

## Assumptions and Dependencies
Suposiciones: 
Desarrollar una habilidad relacionada con un área de conocimiento genera un interés en esa área.
El jugador tiene un entendimiento básico del funcionamiento de un circuito.
Practicar al resolver varios niveles ayudará a desarrollar la habilidad en el jugador.

Dependencias:
El jugador debe tener una conexión a internet y un navegador con los requerimientos mínimos para correr el juego.
El tamaño de la muestra (número de jugadores) debe ser suficientemente grande para un buen análisis de datos.
Dependeremos de una base de datos activa para la recopilación de los resultados y hospedar la página web y el videojuego.

# System Features and Requirements
This is where you detail the specific requirements for building your product.

## Functional Requirements
The functional requirements describe the services and functions of a system. Functional requirements must be precise and unambiguous.

El jugador debe poder interactuar con el videojuego.
El jugador debe poder seleccionar un nivel.
El jugador debe poder pausar el juego.
El jugador podrá consultar la información relevante sobre cada compuerta desde el menú de pausa.
El jugador debe poder salir del juego cuando este lo desee.
El juego debe calcular el puntaje de los usuarios, utilizando el número de movimientos como parámetro.
El jugador debe poder visualizar la expresión lógica correspondiente a cada nivel.
El juego debe ser capaz de recopilar la información de los resultados de los jugadores.
Se requerirá crear un usuario para comenzar el juego, este podrá retomar el juego despues de hacer login.
El jugador podrá consultar información acerca de la empresa STEAM y sobre los conceptos manejados en el juego en una página del sitio web.
El analista de STEAM podrá consultar los datos a través de una interfaz de usuario.
El usuario podrá ajustar el volumen de los efectos y la música.

## External Interface Requirements
External interface requirements are types of functional requirements. They outline how your product will interface with other components or systems.

There are several types of interfaces you may have requirements for, including:
- User
- Hardware
- Software
- Communications

## Non-functional Requirements
Non-functional requirements are restrictions on the system or the development process. Non-functional requirements can be more critical than functional ones. If they are not met, the system is useless!
El sistema debe ser responsivo ante el input, el retraso debe ser menor a 400 milisegundos.

El juego debe poder correr en los navegadores mas populares (Google chrome, Mozilla Firefox, Safari y Microsoft Edge).

Los niveles se irán desbloqueando conforme el jugador progrese en el juego.

El jugador podrá escoger cualquier nivel que ya haya superado.

El jugador podrá entender las reglas del juego de manera fácil e intuitiva en menos de 5 minutos.

# Screens
  especificar user classes que tienen acceso a las pantallas
Identifying the individual screens (for an app), or pages (for a website) are where a product’s shape starts to become clear. They are a distillation of the user stories into a set of distinct sections that satisfy the needs and behaviors identified so far. The process of outlining an application’s screens may also highlight any requirements or considerations that have been overlooked up to this point.

###Juego:

Menú de pausa

Selección de nivel

Pantalla con el nivel actual

Ajustes

###Página:

Login/Register

Videojuego.

Acerca de STEAM.

Resultados recabados.

Reglas explicación e información del juego.

###Acceso a pantallas por clases de usuario:

Jugador: Menú de pausa, selección de nivel, pantalla con el nivel actual, ajustes, login/register, videojuego, acerca de STEAM, reglas e información del juego.
Analista de STEAM: Pantallas del jugador más acceso a los resultados recabados.

This has the dual purpose of both contributing to a more accurate vision of the product early on, and serving as a jumping-off point for the time when designers do get involved.

## Wireframes
Wireframes are simple page layouts that outline the size and placement of elements, and features on a page. They are generally devoid of color, font styles, logos or any design elements.

Wireframing is probably the most time-consuming step of this process and for some simple projects, it may be overkill. For complex projects where serious design thinking needs to happen, wireframes are an indispensable tool.

Here are some popular tools for wireframing:
- https://marvelapp.com/  
- https://balsamiq.com/ 
- https://jetstrap.com/ 
- https://www.fluidui.com/ 
- https://ninjamock.com/ 
- https://www.justinmind.com/ 
- https://moqups.com/
