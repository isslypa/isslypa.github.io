# Título: Introducción al Control Domótico

Autor: Gonzalez Juan  
Número de estudiante: 20123456  
Asignatura: Programación 2 — Universidad Santo Tomás  
Fecha: 2025-10-28

## Resumen
Este documento presenta la introducción al proyecto ControlDomotico. Se describen los objetivos, la motivación y un breve resumen de las funcionalidades implementadas en la entrega inicial.

## Introducción
El proyecto busca crear una interfaz básica en WinForms que permita registrar y controlar dispositivos (encender/apagar/alternar).

## Alcance
Esta primera entrega cubre: diseño del formulario, clases base para dispositivos, y funcionalidades de agregar/encender/apagar/alternar.

## Metodología
Se utilizó C# con .NET 6/8 y WinForms. Se estructuró el código en carpetas Domain, UI e Infrastructure.

## Desarrollo / Contenido
Se implementó:
- Interfaz IActuable y clases DispositivoBase, Lampara.
- Formulario con controles para agregar y controlar dispositivos.
- Resumen dinámico que muestra totales y estados.

## Resultados
Interfaz funcional que permite agregar dispositivos y controlar su estado. Capturas y demo están incluidas en el repositorio.

## Conclusiones
La entrega cumple los requisitos funcionales básicos. Como mejoras futuras: persistencia en JSON, más tipos de dispositivos y mejor UI.

## Referencias
- Material de la asignatura Programación 2
