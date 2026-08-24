# GIT FLOW - SETUP DE INFRAESTRUCTURA (SPRINT 1)

## Cambio aplicado
Creacion formal de la rama `develop` y activacion de Branch Protection sobre `main` y `develop` via GitHub API.

## Detalle tecnico
| Item | Valor |
| :--- | :--- |
| Fecha de aplicacion | 2026-08-24 |
| Rama base | `main` @ `6c8f802` |
| Rama creada | `develop` (GitHub API -> HTTP 201 Created) |
| Proteccion `main` | HTTP 200 OK |
| Proteccion `develop` | HTTP 200 OK |

## Politica vigente (ambas ramas)
* Pull Request obligatorio con **1 aprobacion** minima.
* `dismiss_stale_reviews`: **true** (los cambios nuevos invalidan aprobaciones viejas).
* `enforce_admins`: **true** (push directo prohibido incluso para administradores/docentes).
* `allow_force_pushes`: **false** / `allow_deletions`: **false**.

## Flujo de trabajo resultante
`feature/<tema>` -> PR hacia `develop` (1 review) -> PR de integracion hacia `main` (1 review).

## Evidencia del flujo
Este documento ingreso mediante el propio flujo gobernado: rama `feature/git-flow-s1` -> PR -> aprobacion docente -> merge a `develop`. El intento previo de escritura directa sobre `main` fue rechazado por la API con HTTP 409, demostrando que la proteccion esta activa.

Contrato declarado en `sprint-pp3-config.json` (seccion `rules`) queda ahora **aplicado por la plataforma**, no solo documentado.
