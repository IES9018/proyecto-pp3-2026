# PP3 — Alineación documental 2026

**Fecha:** 2026-10-05 · **Alcance:** higiene documental + cierre del Cuadernillo 03
**Rama:** `feature/docs-cuadernillo-alignment` · **Sin push directo a main/develop.**

## Fuentes canónicas (SSOT)

| Qué | Fuente única |
|---|---|
| Fechas, entregables, reglas de sprint/Git Flow, cierre | `sprint-pp3-config.json` |
| Detalle operativo por sprint | `sprints/sprint-N/sprint-config.json` |
| Tareas tildables del estudiante | `sprints/sprint-N/CHECKLIST.md` |
| Marco académico | `Planificaciones/Programa-…` y `Contrato-Pedagogico-…` |
| Navegación | `README.md` |
| Infraestructura (histórico) | `course-state.json` (snapshot 26-ago-2026, **no** es SSOT) |

Fechas vigentes intencionales (2.º semestre): S1 24-ago–18-sep · S2 21-sep–16-oct · S3 19-oct–13-nov · cierre técnico **17-nov** · defensa integradora **19-nov** (CRONOGRAMA-TPs: "Integrador Final - defensa del repo | jue 19 nov").

## Contradicciones encontradas

1. Planificación de raíz duplicaba `Planificaciones/` y mencionaba **forks** (L38) — incompatible con el modelo *sin forks* vigente.
2. README con estado estático ("EMPEZÁ ACÁ Sprint 1… SPRINT VIGENTE") mezclaba cronograma con estado vivo.
3. Git Flow se explicaba con un solo flujo (`feature→develop→main`) sin distinguir el bootstrap S1 (PR hacia `main`, checklist S1) del flujo completo.
4. `DIAGRAMAS_REFERENCIA.md` mostraba el flujo sin declarar a qué escenario aplica.
5. `course-state.json` (26-ago, S1 "VIGENTE") podía leerse como SSOT de fechas.

## Cambios aplicados

| Archivo | Cambio |
|---|---|
| `Planificacion-…-2026.md` (raíz) | Reemplazado por nota-redirigido a los canónicos (versión previa en historial de Git) |
| `INDICE_SEGUIMIENTO.md` | Referencia actualizada al puntero |
| `README.md` | "Empezá acá" durable (SSOT → checklist), tabla de SSOT, mapa de sprints sin estado envejecido, `course-state.json` reclasificado como snapshot |
| `docs/auditoria/GIT_FLOW_SETUP.md` | + Matriz de Git Flow por escenario (6 filas, con fuente por fila) |
| `docs/arquitectura/DIAGRAMAS_REFERENCIA.md` | Notas de escenario en los 2 diagramas (flujo completo con develop; ciclo de vida de PR) |

## Cambios NO aplicados y por qué

- **Fechas y cronograma:** intactos (intencionales; SSOT no los contradice).
- **`course-state.json`:** sin reescritura — es snapshot histórico; reclasificado por documentación, no reescrito.
- **`docs/TUTORIAL-kanban.md`:** el "enlace roto" `link-de-tu-tablero` es un placeholder pedagógico intencional dentro de un ejemplo.
- **`.opencoderules` / `INSTRUCTIONS.md`:** sin cambios; coherentes con Programa (Anexo I) y README (no endurecer ni flexibilizar sin respaldo).

## Cuadernillo (fuera del repo)

Correcciones A1-A7 aplicadas en `cuadernillos/pp3-coordinacion/` (workspace): Git Flow bootstrap/completo, plantilla de PR real (Trazabilidad de Issue + Quality & Security Gate + Git Flow & Convenciones), rúbrica determinista con pesos/score/evidencias, aserciones sin atribuir al bot, cierre técnico 17-nov separado de defensa 19-nov (CHANGELOG e informe incluidos), checkpoint mobile TP5, paginación verificada (p.21: previa 101% → se mantiene, checkpoint íntegro). Detalle: `FINAL_BOOKLET_QA.md`. PDF final: 42 págs. A4, QA PASS.

## Repo

Inventario: `sprint-pp3-config.json` **CANONICAL** · `sprints/sprint-N/*` **OPERATIONAL** · `CHECKLIST.md` **OPERATIONAL (interfaz pedagógica)** · Programa/Contrato **CANONICAL (marco)** · README **DERIVED (navegación)** · `course-state.json` **HISTORICAL (snapshot)** · planificación raíz → **redirigida** · `GIT_FLOW_SETUP` **OPERATIONAL (infra)** · `DIAGRAMAS_REFERENCIA` **CANONICAL (visual)** · `INSTRUCTIONS.md`/`.opencoderules`/`INSTRUCCIONES_ORGANIZACION.md` **OPERATIONAL (arnés)** · PR template **CANONICAL**.

## QA

- Enlaces internos clave: 26 OK · 1 roto real (puntero→informe, resuelto con este documento) · 1 placeholder intencional (tutorial).
- Sin "forks" activos en documentos vigentes (queda solo en historial y en este informe como registro).
- `grep` de contradicciones: "SPRINT VIGENTE" eliminado del README; "17 nov/19 nov" reconciliados con config + CRONOGRAMA.
- Cuadernillo: qa-preflight PASS · qa_contenido PASS · regresión 18/18 PASS · 42 páginas A4.

## Commit(s)

1. `docs: redirige la planificacion raiz a los documentos canonicos`
2. `docs: hace durable la navegacion de sprints y explicita el SSOT`
3. `docs: documenta la matriz de Git Flow por escenario`
4. `docs: anota el escenario en los diagramas de referencia`
5. `docs: registra la alineacion documental 2026`

## PR

`feature/docs-cuadernillo-alignment` → `develop` (flujo del repo de coordinación), con la plantilla oficial. Sin autoaprobación ni automerge.

## Pendientes humanos

- Revisión docente del PR (1 aprobación requerida por protección).
- Confirmar que no existan consumidores externos de la planificación raíz fuera de `INDICE_SEGUIMIENTO.md` (único consumidor detectado en el repo).
