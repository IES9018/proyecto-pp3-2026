# 📊 Tutorial: Crear tu Tablero Kanban en GitHub (10 minutos)

> **Sin instalar nada.** El tablero es una función propia de GitHub llamada *Projects*. Si sabés entrar a tu repo, sabés llegar acá.
>
> *(Kanban = tablero visual con columnas Por hacer / En progreso / Hecho; tus tareas son tarjetas que movés según avanzan.)*

---

## Cómo se ve el resultado final

```
┌──────────────────┬──────────────────┬──────────────────┐
│    POR HACER     │   EN PROGRESO    │      HECHO       │
├──────────────────┼──────────────────┼──────────────────┤
│ ┌──────────────┐ │ ┌──────────────┐ │ ┌──────────────┐ │
│ │ RF-03 Registrar│ │ │ SPEC v2      │ │ │ Repo creado  │ │
│ │ animales     │ │ │ (rama tp1)   │ │ │ ✅ merged    │ │
│ └──────────────┘ │ └──────────────┘ │ └──────────────┘ │
│ ┌──────────────┐ │                  │                  │
│ │ ADR-001 stack│ │                  │                  │
│ └──────────────┘ │                  │                  │
└──────────────────┴──────────────────┴──────────────────┘
        ↑ arrastrás las tarjetas entre columnas ↑
```

---

## Paso a paso

### 1️⃣ Entrá a tu repo y abrí la pestaña Projects

```
github.com/IES9018/tu-repo
              ↓ barra superior del repo
[ Code ] [ Issues ] [ Pull requests ] [ Projects ] ← clic acá
```

### 2️⃣ Botón verde: `New project`

- Elegí la plantilla **📋 Board** (es el kanban clásico).
- Nombre sugerido: `Tablero <TuProyecto>` (ej.: `Tablero GanadApp`).
- Clic en **Create project**.

### 3️⃣ Renombrá las columnas

Viene con 3 columnas en inglés. Clic sobre cada nombre → Rename:

| Viene | Renombrala a |
|---|---|
| `Todo` | **Por hacer** |
| `In progress` | **En progreso** |
| `Done` | **Hecho** |

### 4️⃣ Creá tus primeras tarjetas

Dentro de una columna → botón **`+ Add item`** → escribí la tarea y Enter.

Sugerencia para arrancar (copiate estas 5):

```
Por hacer:
  ├── Crear SPEC.md (TP1)
  ├── ADR-001 stack tecnológico (TP1)
  ├── Configurar .opencoderules (TP1)
En progreso:
  └── (lo que estés haciendo hoy)
Hecho:
  └── Repo creado ✅
```

💡 **Truco pro:** si escribís `#` en el buscador del item, GitHub te lista tus Issues y PRs para linkearlos como tarjeta. Así el tablero se conecta solo con tu trabajo real.

### 5️⃣ Usalo: mover = arrastrar

Cuando empezás algo → arrastrala a **En progreso**. Al mergear el PR → a **Hecho**. Nada más.

### 6️⃣ Dejalo linkeado (para que el docente lo vea)

Copiá la URL del tablero (ej.: `github.com/users/tuusuario/projects/1`) y agregala al final de tu `README.md`:

```markdown
## 🗓️ Gestión
Tablero del sprint: [Kanban](link-de-tu-tablero)
```

Ese enlace es la evidencia del ítem *"Proyecto vinculado al tablero"* del CHECKLIST del sprint.

---

## ❓ FAQ

| Pregunta | Respuesta |
|---|---|
| ¿Necesito instalar una app? | No. Es parte de GitHub, funciona en el navegador y en la app móvil de GitHub |
| ¿Puedo usar Trello/Jira en su lugar? | Sí, siempre que el docente tenga acceso de lectura y el tablero cumpla: columnas Por hacer/En progreso/Hecho |
| ¿Un tablero por sprint o uno solo? | Uno solo; al abrir sprint nuevo agregá las tarjetas nuevas (el historial queda arriba) |
| ¿Las tarjetas cuentan para la nota? | El tablero completo alimenta *Gestión del proyecto (15%)*: se ve planificación real, no relleno último día |

---

*Vinculado al [CHECKLIST Sprint 1](../sprints/sprint-1/CHECKLIST.md) · Fase 4*
