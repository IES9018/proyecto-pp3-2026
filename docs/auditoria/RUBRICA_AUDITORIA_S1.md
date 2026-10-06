# RUBRICA DETERMINISTA DE EVALUACION - SPRINT 1

> **Alcance:** estos pesos son el instrumento especifico del Sprint 1 y NO reemplazan los pesos oficiales del espacio (Implementacion 40% - Testing 20% - Seguridad 15% - Documentacion 10% - Gestion 15%), que se aplican sobre el conjunto del cuatrimestre en el cierre integrador.

| Criterio | Peso | Indicador de Cumplimiento (Score 0-100) | Evidencia verificada por el docente |
| :--- | :--- | :--- | :--- |
| **Git Flow y Trazabilidad** | 25% | Respeto del flujo por ramas (`feature/*`), PRs con plantilla completa mergeados por el alumno, commits convencionales trazables a issues. | Historial `git log` y PRs del repo del alumno |
| **Auditoria Critica de Codigo** | 35% | Documentacion explicita en `auditoria-sprint1.md` de errores hallados en codigo asistido por IA y sus correcciones, con evidencia enlazada. | Parseo de Markdown en `docs/auditoria/` |
| **Calidad Automatizada Local** | 20% | Linter/formatter configurado y ejecutado localmente; plantilla de PR con checklists completos en cada entrega. | Contenido del PR y configs de lint en el repo |
| **Seguridad Base** | 20% | Cero leaks de secrets, `.gitignore` funcional, entradas sanitizadas en componentes criticos. | Revision estatica del repo (scanner del docente) |