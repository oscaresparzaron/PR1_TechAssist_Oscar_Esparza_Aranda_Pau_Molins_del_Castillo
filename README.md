PR1 – TechAssist: Diseño de Base de Datos y Modelo E-R

Integrantes: Oscar Esparza Aranda y Pau Molins del Castillo.

Objetivo del diseño: diseñar el modelo Entidad-Relación y el modelo relacional de tablas para TechAssist, empresa de soporte informático, de forma que la información de clientes, técnicos, departamentos, incidencias y servicios quede organizada, sin duplicidades y con relaciones coherentes, como paso previo a una futura implementación en un SGBD.

Descripción breve del modelo: las entidades principales son CLIENTE, TECNICO, DEPARTAMENTO, INCIDENCIA, SERVICIO, SERVICIO_PRESENCIAL y SERVICIO_ONLINE. CLIENTE guarda datos personales y teléfonos en tabla aparte. TECNICO guarda datos personales, dirección compuesta y departamento. DEPARTAMENTO guarda nombre, turno y técnico responsable 1:1. INCIDENCIA guarda título, descripción, fechas, prioridad, estado, cliente y servicio. SERVICIO guarda nombre, precio y jerarquía PRESENCIAL y ONLINE. Las relaciones principales son CLIENTE 1:N INCIDENCIA, DEPARTAMENTO 1:N TECNICO por pertenencia y 1:1 TECNICO por responsable, TECNICO N:M INCIDENCIA resuelta con INTERVENCION, SERVICIO 1:N INCIDENCIA y jerarquía SERVICIO con SERVICIO_PRESENCIAL y SERVICIO_ONLINE.

Archivos incluidos:
-PR1_TechAssist_Oscar_Esparza_Aranda_Pau_Molins_del_Castillo.pdf
-README.md

