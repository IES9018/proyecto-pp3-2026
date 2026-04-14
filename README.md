### 🏫 **Institución:** IES 9-018 "Gobernador Celso Jaque"
### 📚 **Carrera:** Tecnicatura Superior en Desarrollo de Software
### 📖 **Espacio Curricular:** Práctica Profesionalizante III
### 👨‍🏫 **Profesor:** Paulo Alvarez
### 📅 **Año:** 2026 | **Curso:** 3° AÑO | **Formato:** Anual

---

# Práctica Profesionalizante III — 2026

## ¿Qué es este espacio?

La Práctica Profesionalizante III es el espacio donde **ejecutás el proyecto** que diseñaste en Práctica Profesionalizante II. Acá ya no es solo análisis o modelado: es construcción real, con testing, métricas y evaluación de calidad.

Este es el espacio integrador de **todo el tercer año**:

| Materia | Aporte al proyecto |
|---------|--------------------|
| Programación III | Código de mayor complejidad |
| Arquitectura y Diseño de Interfaces | Tecnologías, patrones y UI |
| Auditoría y Calidad de Sistemas | Testing y métricas |
| Seguridad Informática | Protección del sistema |
| Bases de Datos II | BD avanzada |
| Legislación Informática | Marco legal |
| Gestión de Proyectos de Software | Gestión, planificación, cierre |

---

## 🎯 Qué vas a hacer

1. **Ejecutar** el proyecto diseñado en PP2 (análisis + diseño ya entregados)
2. **Programar** con las tecnologías elegidas en ADI
3. **Testear** con criterios de calidad (Auditoría y Calidad)
4. **Asegurar** el sistema (Seguridad Informática)
5. **Gestionar** el proyecto con herramientas ágiles (Gestión de Proyectos)
6. **Documentar** legalmente (Legislación Informática)

---

## 🔄 Flujo de Trabajo

Mismo flujo que en las prácticas anteriores: **GitHub + forks + PRs + issues**

```bash
# Opcion con GitHub CLI (recomendada)
gh repo fork IES9018/proyecto-pp3-2026 --clone=true
cd proyecto-pp3-2026

# Vincular repositorio base (upstream)
git remote add upstream https://github.com/IES9018/proyecto-pp3-2026.git
git fetch upstream

# Crear rama de trabajo
git checkout -b feat/sprint-01

# Guardar cambios y subir rama
git add .
git commit -m "feat: avance sprint 01"
git push -u origin feat/sprint-01

# Crear Pull Request
gh pr create --base main --head feat/sprint-01 --title "Sprint 01" --body "Entrega de avance"
```

```bash
# Opcion manual (sin GitHub CLI)
# 1) Hacer fork desde la web de GitHub
# 2) Clonar tu fork
git clone https://github.com/TU-USUARIO/proyecto-pp3-2026.git
cd proyecto-pp3-2026

# 3) Agregar upstream
git remote add upstream https://github.com/IES9018/proyecto-pp3-2026.git
```

### Entregas mediante Pull Request

- Cada sprint o módulo se entrega con un **Pull Request** al repositorio base
- Las observaciones y correcciones se hacen a través de **issues**
- El historial de commits refleja el progreso real del proyecto

---

## 📚 Estructura de Archivos

| Archivo / Carpeta | Descripción |
|-------------------|-------------|
| `README.md` | Esta guía |
| `LISTA_ESTUDIANTES.md` | Repositorios de todos los estudiantes |
| `INDICE_SEGUIMIENTO.md` | Índice de seguimiento y evaluación |
| `seguimiento-estudiantes.json` | Estado por estudiante |
| `CHANGELOG.md` | Historial de cambios en el material |
| `Planificaciones/` | Cronograma, programa, contrato pedagógico |
| `feedback/` | Feedbacks individuales |

---

## 🔗 Continuidad del Proyecto Integrador

```
PP I (1er año)   → Observación + Programación I + Requerimientos
PP II (2do año)  → Diseño del proyecto + UML + BD + Redes + SO
PP III (3er año) → EJECUCIÓN: código + testing + seguridad + cierre
```

El proyecto que ejecutás en PP3 **es la evolución directa** del diseñado en PP2 durante 2025.

---

## 👥 Equipo

**Profesor:** Paulo Alvarez  
**Institución:** IES 9-018 "Gobernador Celso Jaque" — Mendoza  
**Repositorio base:** [IES9018/proyecto-pp3-2026](https://github.com/IES9018/proyecto-pp3-2026)
