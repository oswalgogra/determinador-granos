# Versiones de app según licenciamiento

* Status: accepted
* Deciders: Jorge, Oswaldo
* Date: 2023-11-01

Technical Story: Se manejará distintas licencias para la app, cada una con funcionalidades que van incrementando de licencia en licencia.

## Context and Problem Statement

Se debe poder controlar qué licencia tiene el usuario de la app, de tal forma que al instalarla, tenga acceso a las funcionalidades que corresponden según la licencia o plan que adquirió.

## Considered Options

* Utilizar una sola app, y controlar las opciones de acceso según el plan adquirido.
* Desarrollar varias apps, cada una según el nivel de licencia o plan adquirido

## Decision Outcome

Chosen option: "Desarrollar varias apps, cada una según el nivel de licencia o plan adquirido", because Facilita el control sobre qué plan tienen los clientes y qué pueden hacer sobre el sistema.

### Positive Consequences

* mejorar la optimización de recursos de la app

### Negative Consequences

* Se aumenta la cantidad de apps sobre las cuales hay que hacer vigilancia y mantenimiento.

## Pros and Cons of the Options

### Utilizar una sola app, y controlar las opciones de acceso según el plan adquirido.

Se manja una sola app con todas las funcionalidades, pero solo se habilitan las que el usuario tenga.

* Good, because El mantenimiento sería sobre una sola app.
* Good, because Cualquier usuario puede loguearse en un mismo teléfono.
* Good, because La descarga de la apk sería siempre hacia el mismo destino.
* Bad, because Al ser una sola app, esta debe hacer proceso de sincronización cada vez que el usuario se registre.
* Bad, because La app es más pesada, y tendría funcionalidades que no se utilizarían dependiendo del plan del cliente.
* Bad, because Un usuario con un plan superior puede iniciar sesión en el teléfono de otro usuario y no cerrar sesión, para que el segundo pueda hacer uso de las funcionalidades avanzadas.

### Desarrollar varias apps, cada una según el nivel de licencia o plan adquirido

Se construyen varias apps, y cada una tendrá las funcionalidades pertinentes según el plan que tenga el cliente.

* Good, because El cliente instalaría la versión de la app que le corresponde según el plan.
* Good, because Se puede controlar a qué funcionalidades tiene acceso el cliente según el plan adquirido.
* Good, because Se optimizan los recursos al tener en una app las funcionalidades suficientes.
* Bad, because Se debe hacer mantenimiento sobre varias apps.
* Bad, because El proceso de actualización de un plan a otro debe ser guiado para que el cliente instale la app correcta sin perder los datos.
