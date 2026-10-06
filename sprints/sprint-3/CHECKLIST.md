# Checklist del Estudiante — Sprint 3: Seguridad, Despliegue y Evidencia Medible (19 oct – 13 nov)

> 🧭 **¿Te perdiste?** [Volvé al README principal](../../README.md) · 🗓️ Roadmap completo: [CRONOGRAMA-TPs-2026](https://github.com/IES9018/proyecto-adi-2026/blob/main/Planificaciones/CRONOGRAMA-TPs-2026.md)
>
> ⚙️ Flujo de siempre: rama `feature/<tema>` → PR con plantilla → checklists completos → mergeás vos → el docente audita después.

## Fase 0 — Apertura (19 oct)
- [ ] Leé este checklist completo y actualizá el tablero Kanban → [Tutorial paso a paso](../../docs/TUTORIAL-kanban.md)
- [ ] Verificá que el núcleo del Sprint 2 está mergeado y los tests siguen verdes

## Fase 1 — Contratos antes que código (consume el TP4, entrega mar 27 oct)
- [ ] `api-contracts.yaml` (OpenAPI 3.x) con tus **5 endpoints críticos**, linter sin errores
- [ ] API implementada respetando el contrato — todo cambio de endpoint empieza en el YAML

## Fase 2 — Seguridad aplicada
- [ ] Threat model lite completado: ≥ 5 amenazas STRIDE sobre TUS endpoints reales
- [ ] Cada amenaza tiene mitigación **aplicada en el código** y documentada en `docs/seguridad/`
- [ ] Arnés actualizado con las reglas de seguridad (sin secrets, validación de entradas, contrato primero)

## Fase 3 — Mobile medible (consume el TP5, entrega lun 10 nov)
- [ ] ADR-006: estrategia mobile decidida con matriz de decisión
- [ ] Pantallas críticas adaptadas a breakpoint móvil (targets táctiles ≥ 48px)
- [ ] Presupuestos de rendimiento (LCP / INP / peso JS) definidos con herramienta de medición asignada

## Fase 4 — Despliegue funcional
- [ ] Sistema accesible: URL pública **o** artefacto reproducible documentado paso a paso
- [ ] Guía de despliegue en `docs/deploy/deploy.md` (qué hiciste, cómo se reproduce, qué harías distinto)

## Fase 5 — Cierre (hasta jue 12 nov)
- [ ] Presupuestos **medidos** con evidencia registrada (capturas o salidas de herramienta)
- [ ] `docs/auditoria/auditoria-sprint3.md`: incidentes IA + correcciones + estado de seguridad
- [ ] PR final del sprint mergeado

## 📦 Entregables formales del sprint

| ID | Entregable | Dónde queda en TU repo |
|---|---|---|
| DEL-S3-01 | API según contratos OpenAPI (linter limpio) | `docs/arquitectura/api-contracts.yaml` |
| DEL-S3-02 | Threat model con mitigaciones aplicadas | `docs/seguridad/` |
| DEL-S3-03 | Presupuestos de rendimiento medidos | `docs/arquitectura/presupuestos-rendimiento.md` |
| DEL-S3-04 | Despliegue funcional accesible | `docs/deploy/deploy.md` |
| DEL-S3-05 | Informe auditoría crítica S3 | `docs/auditoria/auditoria-sprint3.md` |

Definición exacta: [sprint-pp3-config.json](../../sprint-pp3-config.json) → `PP3-2026-S3`

> 📊 La rúbrica determinista de este sprint se publica el día de apertura. Después viene el **Cierre (mar 17 nov)**: pipeline CI + release v0.1.0 + informe final — la base de tu defensa integradora.
