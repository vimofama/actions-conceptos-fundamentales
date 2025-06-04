# Conceptos Fundamentales

## GitHub Actions
GitHub actions es una herramienta de GitHub que nos ayuda automatizar tareas relacionadas a nuestro repositorio.

- CI (Continuous Integration)
- CD (Continuous Deployment)

## ¿Cómo funciona?
GitHub Actions nos permite crear Workflows que serán ejecutados en eventos específicos
- Push
- Merge
- PR

## Casos de uso:
Automatización.
- Build
- Testing
- Notificaciones (Slack, Correos, Notion, Asana...)
- Escaneo de seguridad

## Conceptos claves
### Workflows
- Conjunto de procesos automatizados definidos en un archivo YAML dentro de .github/workflows

### Triggers
- Eventos que hacen que el workflow se ejecute.
- Se definen utilizando on.

### Jobs
- Unidades independientes de trabajo dentro de un workflow
- Se ejecutan en paralelo por defecto
- Cada Job corre en un runner
- Se definen utilizando jobs

### Steps
- Pasos individuales dentro de un Job
- Un Job puede poseer multiples pasos
- Se ejecutan secuencialmente en el mismo runner
- Tiene la capacidad de usar variables de entorno
- Se definen utilizando steps
    - Utilizan name, uses / run

### Runners
- Entorno (Máquinas virtuales) donde se ejecutan los jobs
- Github posee imagenes actualizadas de S.O como Ubuntu, Windows, MacOs
- Se definien utilizando runs-on
