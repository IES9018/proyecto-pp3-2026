# DIAGRAMAS Y MODELOS DE REFERENCIA EN MERMAID

Este documento contiene los estándares visuales de arquitectura, flujo de trabajo y ciclos de vida obligatorios para el proyecto de PP3.

## 1. Flujo de Trabajo y Git Flow
```mermaid
flowchart LR
    A[Issue en Kanban] --> B[Rama feature/xxx]
    B --> C[Commits Semánticos]
    C --> D[Pull Request a develop]
    D --> E{CI/CD Gate}
    E -- Pass --> F[Code Review Capataz]
    E -- Fail --> C
    F -- Aprobado --> G[Merge a develop]
    G --> H[Release a main]
```

## 2. Estado de Ciclo de Vida de Pull Requests
```mermaid
stateDiagram-v2
    [*] --> Draft: Creación de PR
    Draft --> InReview: Checklists marcadas
    InReview --> ChangesRequested: Hallazgos de Seguridad/Auditoría
    ChangesRequested --> InReview: Commits de Corrección
    InReview --> Approved: Review Docente Aprobada
    Approved --> Merged: Merge a develop
    Merged --> [*]
```
