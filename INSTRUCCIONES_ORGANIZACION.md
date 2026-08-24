# INSTRUCCIONES_ORGANIZACION.md

## Reglas Obligatorias de Operatoria y Repositorios — Organización IES9018

### 1. Creación de Repositorios de Estudiantes
* **Prohibición absoluta de Forks:** Ningún estudiante debe forkear repositorios base. Todo proyecto se crea directamente dentro de la organización `IES9018`.
* **Nomenclatura obligatoria:** `<nombre_alumno>-<nombre_proyecto>` (ej.: `raul-crm`, `analia-portal`).

### 2. Rol Docente (Capataz / Arquitecto de Obra)
* El docente no escribe código del alumno: audita de forma determinista mediante CLI, deja **Issues** y realiza **Code Reviews** en los Pull Requests.
* Toda especificación (`SPEC.md`) requiere aprobación docente previa a la fusión de código.

### 3. Arnés Exclusivo OpenCode
* El único arnés válido es la combinación `.opencoderules` + `INSTRUCTIONS.md` en la raíz del repositorio.
* Cualquier otro archivo de configuración de agentes queda **fuera del estándar organizacional** y será observado en auditoría.
* El motor local es OpenCode; su comportamiento queda limitado por dichos archivos sin excepciones.
