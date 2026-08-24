# RÚBRICA DETERMINISTA DE EVALUACIÓN - SPRINT 1

| Criterio | Peso | Indicador de Cumplimiento (Score 0-100) | Entrada de Control CLI Go |
| :--- | :--- | :--- | :--- |
| **Git Flow & Trazabilidad** | 25% | Respeto estricto de ramas (`feature/*` -> `develop` -> `main`), PRs trazables a Issues y commits semánticos. | Inspección de `git log` y GitHub GraphQL API |
| **Auditoría Crítica de Código** | 35% | Documentación explícita en `auditoria-sprint1.md` de errores hallados en código asistido por IA y sus correcciones. | Parseo de AST/Markdown en `docs/auditoria/` |
| **CI/CD & Automatización** | 20% | Correcta ejecución de linter, validación de sintaxis y pasaje de checks automatizados en PR. | Status Check API de GitHub Actions |
| **Seguridad Base** | 20% | Zero leaks de secrets, configuración limpia de `.gitignore` y sanitización de componentes críticos. | Scanner estático Go (`gosec` / `trufflehog`) |