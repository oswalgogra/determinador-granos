# Gestor de estados de la móvil

* Status: proposed
* Deciders: Oswaldo, Javier Campuzano, Jorge Luis
* Date: 2023-09-11

## Context and Problem Statement

Se requiere identificar cambios en la móvil, para poder renderizar lo que se presenta en la visual de la App. Por ejemplo, estado de la conexión con el hardware del determinador, saber si el bluetooth está encendido.

## Considered Options

* Provider
* Stateful widget
* Bloc
* RiverPot

## Decision Outcome

Chosen option: "Provider", because Esta librería consume poco recursos y ahorra el proceso de hacer pooling a los cambios de estado. Es la más fácil de implementar, el equipo de desarrollo ya la conoce.
