# PP3 — Coordinación del Proyecto Integrador 🚀

**Práctica Profesionalizante III · IES 9-018 · Ciclo 2026**
Tecnicatura Superior en Desarrollo de Software · 3° Año · Prof. Paulo Alvarez

> Este es el **repo de coordinación de la cátedra**: acá está el checklist del sprint vigente, las reglas de Git Flow y la rúbrica de auditoría. Tu código vive en **tu repositorio individual** dentro de la organización `IES9018`.
>
> Teoría de arquitectura: [`ADI-teoria-y-recursos`](https://github.com/IES9018/ADI-teoria-y-recursos) · Consignas y plantillas ADI: [`proyecto-adi-2026`](https://github.com/IES9018/proyecto-adi-2026)

---

## 🚦 EMPEZÁ ACÁ (Sprint 1 — 24 ago al 18 sep)

| Paso | Qué hacer | Evidencia esperada |
|---|---|---|
| 1 | Leé el **CHECKLIST del sprint** completo | [sprints/sprint-1/CHECKLIST.md](./sprints/sprint-1/CHECKLIST.md) |
| 2 | Creá tu repo individual `<nombre_alumno>-<nombre_proyecto>` | ej.: `raul-crm` — público, en `IES9018`, **sin forks** |
| 3 | Subí tu `SPEC.md` inicial (proyecto traído de PP2) | raíz de tu repo |
| 4 | Configurá tu arnés `.opencoderules` (+ `INSTRUCTIONS.md`) | raíz de tu repo |
| 5 | Vinculá tu repo al tablero Kanban de la materia | captura/enlace en el tablero | *(tablero visual de tareas)* → [tutorial](docs/TUTORIAL-kanban.md)
| 6 | Al cerrar: completá el informe de auditoría crítica | `docs/auditoria/auditoria-sprint1.md` en TU repo |

> 🗓️ Roadmap de TPs ADI + sprints: [CRONOGRAMA-TPs-2026](https://github.com/IES9018/proyecto-adi-2026/blob/main/Planificaciones/CRONOGRAMA-TPs-2026.md)

Checklist detallado: [sprints/sprint-1/CHECKLIST.md](./sprints/sprint-1/CHECKLIST.md)

---

## 🎯 ¿Dónde está la tarea de hoy?

Siempre en la carpeta del sprint activo:

```
sprints/
├
───
 sprint-1/            
 ← 
SPRINT VIGENTE (24 ago - 18 sep)
│
   
├
───
 CHECKLIST.md     
 ← 
tus objetivos tildables
│
   
└
───
 sprint-config.json
├
───
 sprint-2/            
 ← 
PROXIMO (21 sep - 16 oct): nucleo funcional + calidad local
├
───
 sprint-3/            
 ← 
PLANIFICADO (19 oct - 13 nov): seguridad + despliegue
└
───
 cierre               
 ← 
17 nov: pipeline CI + release v0.1.0 + informe final
``````

Entregables formales del Sprint 1 (definición exacta): [sprint-pp3-config.json](./sprint-pp3-config.json)

---

## 🔀 Git Flow obligatorio (aplicado por plataforma)

```
feature/<tema>  →  PR a develop (1 revisión)  →  PR develop → main (1 revisión)
```

* Push directo a `main` o `develop`: **BLOQUEADO** (ni siquiera el docente puede).
* Commits convencionales: `feat:` `fix:` `docs:` `ci:` `chore:`.
* Todo PR usa la plantilla oficial con checklists de calidad, seguridad y trazabilidad.

> **Regla dual:** En tu repo IES9018/<alumno>-<proyecto> hacés el merge vos tras completar los checklists (historial reversible). En este repo de coordinación el esquema es PR + 1 revisión docente (rama protegida).

Plantilla automática: [.github/PULL_REQUEST_TEMPLATE.md](./.github/PULL_REQUEST_TEMPLATE.md)
Referencia visual: [docs/arquitectura/DIAGRAMAS_REFERENCIA.md](./docs/arquitectura/DIAGRAMAS_REFERENCIA.md)

---

## 📊 Evaluación

### Criterios oficiales del espacio (contrato pedagógico)

| Área | % |
|---|---|
| Implementación (funcionalidad y calidad de código) | 40% |
| Testing y calidad | 20% |
| Seguridad | 15% |
| Documentación técnica y legal | 10% |
| Gestión del proyecto (commits, PRs, issues) | 15% |

### Instrumento del Sprint 1

Rúbrica determinista de auditoría: [docs/auditoria/RUBRICA_AUDITORIA_S1.md](./docs/auditoria/RUBRICA_AUDITORIA_S1.md)
Tu informe: `auditoria-sprint1.md` documentando errores hallados en código asistido por IA y sus correcciones.

Marco completo: [Programa PP3](./Planificaciones/Programa-Practica-Profesionalizante-III-2026.md) · [Contrato pedagógico](./Planificaciones/Contrato-Pedagogico-Practica-Profesionalizante-III-2026.md)

---

## 📂 Mapa de este repo

| Ruta | Qué hay |
|---|---|
| `sprints/sprint-*/` | Checklists y configuración de cada sprint |
| `sprint-pp3-config.json` | SSOT: reglas de Git Flow y entregables por entregable-ID |
| `course-state.json` | Estado de infraestructura e hitos de ambas cátedras |
| `Planificaciones/` | Programa oficial + Contrato pedagógico firmados |
| `docs/auditoria/` | Rúbricas deterministas y actas de auditoría |
| `docs/TUTORIAL-kanban.md` | Tutorial visual del tablero Kanban (GitHub Projects) |
| `.github/PULL_REQUEST_TEMPLATE.md` | Plantilla que se autocompleta en cada PR |
| `INSTRUCCIONES_ORGANIZACION.md` / `INSTRUCTIONS.md` | Reglas + arnés local OpenCode |
| `INDICE_SEGUIMIENTO.md` · `LISTA_ESTUDIANTES.md` · `seguimiento-estudiantes.json` | Seguimiento docente |

---

## ❓ FAQ rápida

| Pregunta | Respuesta corta |
|---|---|
| ¿Hago fork? | **NO.** Creás tu repo propio en `IES9018`. |
| ¿Puedo pushear directo a main/develop de MI repo? | **En tu repo individual** (IES9018/<alumno>-<proyecto>): trabajá por ramas y abrí PRs; mergeá vos mismo cuando los checklists estén completos. Queda trazado en el historial y es reversible (revert merge si falla). **En este repo de coordinación**: PR con al menos 1 aprobación (rama protegida), como indica el diagrama de Git Flow de abajo. |
| ¿Dónde está el proyecto que diseñé en PP2? | Lo ejecutás vos; el modelo de referencia está en [proyecto-adi-2026](https://github.com/IES9018/proyecto-adi-2026). |
| ¿Cómo declaro un Non-Goal? | Sección 3 de tu `SPEC.md`. Ver [SPEC-template ADI](https://github.com/IES9018/proyecto-adi-2026/blob/main/templates/SPEC-template.md). |
