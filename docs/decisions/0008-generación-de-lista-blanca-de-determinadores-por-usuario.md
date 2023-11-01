# Generación de lista blanca de determinadores por usuario

* Status: proposed
* Deciders: Jose Luis, Oswaldo
* Date: 2023-11-01

## Context and Problem Statement

Asegurar que cuando un usuario se registre, se sincronicen los datos de los dispositivos que adquirió. Porque cuando se vaya a capturar mediciones, solo se deben recibir de dispositivos que sean propiedad del usuario que está logueado.

## Considered Options

* Que el usuario digite cada serial de cada dispositivo, y se registren en una tabla local (devices).
* Que cuando el usuario se registre, el sistema valide contra la base de datos central qué dispositivos compró, y los sincronice en la tabla (devices) correspondiente.
* Luego de que el usuario se registre, la app le permita seleccionar una opción para que haga la sincronización de los datos de los dispositivos en la tabla (devices) correspondiente.

## Decision Outcome

Chosen option: "Que cuando el usuario se registre, el sistema valide contra la base de datos central qué dispositivos compró, y los sincronice en la tabla (devices) correspondiente.", because Se controla por parte nuestra que al aplicación del cliente tenga almacenados los datos de los dispositivos que la persona compró, sin que haya intervención de ella o alguna inteacción manual. Ya que este proceso sería automático y bajo nuestro control.
