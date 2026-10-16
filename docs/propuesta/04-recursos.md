# Fase 4 · Recursos · <estudio>
## Introducción

Este documento define la estructura de recursos, herramientas técnicas y metodologías de gestión necesarias para llevar a cabo el desarrollo del proyecto. Su propósito es garantizar una distribución clara de responsabilidades en el equipo, asegurar la viabilidad del desarrollo y coordinar el flujo de trabajo colaborativo.

El contenido se articula en torno a tres pilares organizativos:

* **Gestión del talento y roles (Las personas):** Asignación de liderazgos técnicos individuales (Frontend, Backend, Base de datos y QA/Despliegue) y organización modular de tareas en parejas (responsable y apoyo) para cubrir la autenticación, los registros de glucosa/comidas, la calculadora de bolus y las alertas. Se establecen canales de comunicación centralizados a través de Discord y acuerdos de equipo mediante contrato.
* **Infraestructura y herramientas (La tecnología):** Referencia al *stack* técnico detallado en la fase de viabilidad (React, Node.js, Express y MongoDB Atlas) y selección de herramientas estándar para control de versiones (Git/GitHub), prototipado (Figma), desarrollo (VS Code) y pruebas de API (Postman).
* **Flujo de trabajo y repositorio (La gestión):** Metodología ágil apoyada en GitHub Projects (tablero Kanban *To Do / In Progress / Done*), estrategia de ramificación basada en `main`, `develop` y ramas por *issue*, junto con la estructura física de carpetas para el control de la documentación, cliente frontend y servidor backend.
## 1. Las personas
### Roles técnicos
  | Persona | Rol | De qué responde |
### Responsables por módulo
  | Módulo | Requisitos (RF) | Responsable | Apoyo |
### Comunicación     (enlace al contrato)
## 2. La tecnología
### Stack, servicios y APIs   (enlace a la fase 2)
[Enlace a fase 2](https://github.com/Sromerop0610/ProyectoOptativa/blob/develop/docs/propuesta/02-viabilidad-tecnica.md#requisitos-t%C3%A9cnicos)
### Herramientas de desarrollo
| Para qué | Herramienta |
| :--- | :--- |
| **Control de versiones** | Git / GitHub |
| **Diseño UI/UX y prototipado** | Figma |
| **Entorno de desarrollo (IDE)** | Visual Studio Code |
| **Pruebas de APIs y endpoints** | Postman |
| **Gestión de base de datos** | MongoDB Atlas |
| **Comunicación del equipo** | Discord |
## 3. La gestión
### Tablero
La organización del proyecto se gestionará mediante una metodología ágil utilizando **GitHub Projects**.

El trabajo se estructurará en las siguientes columnas principales:
* **To Do:** Tareas planificadas para el sprint o hito actual.
* **In Progress:** Tareas en desarrollo activo.
* **Done:** Tareas completadas, probadas e integradas en la rama principal.

### Ramas

La rama main contiene el codigo principal de la aplicacion, despues tenemos una rama develop en la cual vamos implementando los diferentes cambios para que cuando esten revisados sean integrados en main, para trabajar creamos ramas para cada issue que salen de develop y una vez terminadas se integran en esta.

### Estructura de carpetas

La estructura actual del proyecto es la siguiente

```text
proyecto-diabetes/
├── .github/ISSUE_TEMPLATE
│   └── tarea.md                
├── client/                     
│   └── README.md
├── docs/
│   ├── docs/
│       ├── 00-brainstorming.md              
│       ├── 01-problema.md         
│       ├── 02-viabilidad-tecnica.md             
│       ├── 03-objetivos-y-alcance.md              
│       └── 04-recursos.md
│   └── CONTRATO.md              
├── server/                      
│   └── README.md
├── .gitignore                   
└── README.md                    
