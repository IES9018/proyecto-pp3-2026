# Checklist del Estudiante — Sprint 2: Núcleo Funcional y Calidad Local (21 sep – 16 oct)

> 🧭 **¿Te perdiste?** [Volvé al README principal](../../README.md) · 🗓️ Roadmap completo: [CRONOGRAMA-TPs-2026](https://github.com/IES9018/proyecto-adi-2026/blob/main/Planificaciones/CRONOGRAMA-TPs-2026.md)
>
> ⚙️ Flujo de siempre: rama `feature/<tema>` → PR con plantilla → checklists completos → mergeás vos → el docente audita después.

## Fase 0 — Apertura (21 sep)
- [ ] Leé este checklist completo y copiate los objetivos al tablero Kanban
- [ ] Verificá que tu `SPEC.md` v1 y tu arnés `.opencoderules` están mergeados (cierre del Sprint 1)

## Fase 1 — Arquitectura viva (consume el TP2, entrega mar 29 sep)
- [ ] `SPEC.md` actualizado a **v2**: sección "Restricciones arquitectónicas" citando ADRs + changelog
- [ ] Diagramas **C4** (contexto + contenedores) en `docs/arquitectura/` de TU repo — todo elemento trazable a SPEC o ADR

## Fase 2 — Núcleo funcional
- [ ] Features críticos `RF-01…RF-n` del SPEC **operativos en local**
- [ ] Cada feature implementado vía rama + PR propio (historial auditable)

## Fase 3 — Interfaz crítica (consume el TP3, se abre mar 29 sep)
- [ ] Personas y journeys definidos; las **2 pantallas críticas** wireframeadas
- [ ] Pantallas implementadas respetando los criterios de accesibilidad básica

## Fase 4 — Calidad local
- [ ] Suite unitaria con **≥ 10 tests verdes** corriendo localmente
- [ ] Reporte en `docs/pruebas/reporte-sprint2.md`: qué cubre cada test y qué no (Non-Goals de testing)

## Fase 5 — Cierre (hasta jue 15 oct)
- [ ] `docs/auditoria/auditoria-sprint2.md`: errores hallados en código asistido por IA + correcciones con evidencia (links a PRs)
- [ ] PR final del sprint mergeado con todos los checklists completos

## 📦 Entregables formales del sprint

| ID | Entregable | Dónde queda en TU repo |
|---|---|---|
| DEL-S2-01 | Núcleo funcional según SPEC v2 | raíz (`/`) |
| DEL-S2-02 | Diagramas C4 | `docs/arquitectura/` |
| DEL-S2-03 | Suite de pruebas + reporte | `docs/pruebas/reporte-sprint2.md` |
| DEL-S2-04 | Informe auditoría crítica S2 | `docs/auditoria/auditoria-sprint2.md` |

Definición exacta: [sprint-pp3-config.json](../../sprint-pp3-config.json) → `PP3-2026-S2`

> 📊 La rúbrica determinista de este sprint se publica el día de apertura (misma mecánica que la de [Sprint 1](../../docs/auditoria/RUBRICA_AUDITORIA_S1.md)). Los pesos oficiales del espacio (40/20/15/10/15) aplican al cierre integrador.
