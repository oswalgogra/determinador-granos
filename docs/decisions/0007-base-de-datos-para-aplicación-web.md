# Base de datos para aplicación web

* Status: accepted
* Deciders: Oswaldo G., Jhoinner S., José Luis P., Jorge Luis H, Carmen G.
* Date: 2023-10-24

Technical Story: Base de datos para la aplicación web

## Context and Problem Statement

Se requiere definir un motor de base de datos a utilizar para almacenar los datos del modelo necesarios para la gestión del sistema de información.

## Considered Options

* Oracle
* Mysql
* PostgreSQL

## Decision Outcome

Chosen option: "PostgreSQL", because El equipo ya tiene experiencia en el uso de este motor de base de datos, no implica costos de licenciamiento. Es un motor al que se puede integrar Django sin problemas. El volúmen de información a manejar por el momento se puede gestionar a través de este motor.
