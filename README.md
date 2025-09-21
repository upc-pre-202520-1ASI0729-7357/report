# Capítulo V: Product Implementation, Validation & Deployment
## 5.1. Software Configuration Management.
### 5.1.1. Software Development Environment Configuration.
### 5.1.2. Source Code Management.
### 5.1.3. Source Code Style Guide & Conventions.
### 5.1.4. Software Deployment Configuration.
## 5.2. Landing Page, Services & Applications Implementation.
## 5.2.1. Sprint 1
### 5.2.1.1. Sprint Planning 1.

El Sprint Planning 1 establece la organización inicial del equipo para desarrollar el MVP de ThermaTrace. Se definen el objetivo del Sprint, las User Stories que serán trabajadas, la capacidad del equipo, y los entregables esperados. Este proceso permite una planificación clara y el alineamiento de todo el equipo hacia un mismo objetivo para la entrega de valor.

| Field | Information |
|:------|:------------|
| **Sprint #** | Sprint 1 |
| **Date** | 2025-09-05 |
| **Time** | 05:00 PM |
| **Location** | Virtual (Discord y Zoom) |
| **Prepared By** | Espinoza Quijandria, Oscar Leonardo |
| **Attendees (to planning meeting)** | Oscar Espinoza, Fabrizio Panta, Axel Ordoñez, Jean Grandez, Frezzia Espinoza |
| **Sprint n – 1 Review Summary** | Not applicable (First Sprint of the Mascota Match project) |
| **Sprint n – 1 Retrospective Summary** | Not applicable (First Sprint of the Mascota Match project). |
| **Sprint n Goal** | Finalize the first version of Therma Trace, including the sections of Home, features, precing , Team and about.<br><br>**Sprint Goal:**<br>Our focus is on launching ThermaTrace MVP.<br>We believe it delivers essential functionality and first user experience.<br>This will be confirmed when users can register, navigate, consult services, choose a plan successfully. |
| **Sprint n Velocity** | 23 Story Points |
| **Sprint Goal & User Stories** | **User Stories:**<br> HU1, HU2, HU3, HU4 , HU5, HU6, HU7 |
| **Sum of Story Points** | **23 Story Points** |

### 5.2.1.2. Aspect Leaders and Collaborators

Para asegurar una ejecución eficiente del Sprint 1, se definieron líderes y colaboradores responsables de las principales áreas del proyecto. Cada miembro del equipo lidera o apoya aspectos específicos como el desarrollo de páginas, integración de funcionalidades, diseño visual y animaciones. Esta matriz garantiza una asignación clara de tareas y fomenta el trabajo colaborativo.

| Team Member      | GitHub Username |  Index | languageSwitcher  | Layout  | Base | Components| 
|------------------|-----------------|---|---|---|---|---|
| Oscar Espinoza   | Carbocnito5443  | L | C | C | C | C | 
| Axel Ordoñez     | noomzzzzz       | C | L | C | C | C | 
| Jean Grandez     | JeanGrandez     | C | C | L | C | C | 
| Fabrizio Panta   | F4brizio24      | C | C | C | L | C | 
| Frezzia Espinoza |                 | C | C | C | C | L | 

### 5.2.1.3. Sprint Backlog 1
El Sprint Backlog 1 consolida todas las funcionalidades principales de ThermaTrace, enfocándose en completar toda la experiencia de usuario inicial: About, Home, Pricing, Team, Features.

| Historia de Usuario | Tarea ID | Descripción de la Tarea | Duración Estimada | Responsable | Estado |
|---------------------|----------|--------------------------|-------------------|-------------|--------|
| HU1 | T01 | Implementar sección **Home** con encabezado, logo y menú de navegación responsive. | 6h | Oscar | Done |
| HU2 | T02 | Desarrollar sección **About** con misión, visión, historia de la startup y valores del equipo. | 4h | Axel | Done |
| HU3 | T03 | Construir sección **Pricing** con tarjetas de planes (Basic, Pro, Enterprise), estilos y botón de registro. | 5h | Jean | Done |
| HU4 | T04 | Diseñar sección **Team** con fotos, nombres, roles y enlaces de contacto de los integrantes. | 5h | Fabrizzio | Done |
| HU5 | T05 | Crear sección **Features** listando los servicios principales con íconos, descripciones y opción “ver más”. | 4h | Frezzia | Done |
| HU6 | T06 | Implementar sección **FAQ** con acordeón desplegable para resolver dudas frecuentes. | 3h | Oscar | Done |
| HU6 | T07 | Añadir funcionalidad de **Internacionalización (i18n)** en la landing page (ES/EN), guardando preferencia de idioma. | 3h | Oscar | Done |


### 5.2.1.4. Development Evidence for Sprint Review.


| Repository   | Branch               | Commit ID | Commit Message                  | Commit Message Body | Committed on Date     |
|--------------|----------------------|-----------|----------------------------------|----------------------|------------------------|
| ThermaTrace  | feature/index             | 298c45a   | feat: add index.html         | -                    | 21 de septiembre de 2025    |
| ThermaTrace  | feature/components             | e856efe   | feat: add components.css                | -                    | 21 de septiembre de 2025    |
| ThermaTrace  | feature/layout             | d08a274   | feat: add layout.css             | -                    | 21 de septiembre de 2025    |
| ThermaTrace  | feature/base             | b8fe11d   | feat: add base.css            | -                    | 21 de septiembre de 2025    |
| ThermaTrace  | feature/LenguageSwitcher             | afe5753   | feat: add LenguageSwitcher.js                | -                    | 21 de septiembre de 2025    |
|

## Detalles
Cada feature fue desarrollado en una branch diferente siguiendo buenas prácticas de control de versiones y trabajo en equipo. Se utilizaron mensajes de commit descriptivos y cada cambio fue verificado.

### 5.2.1.5. Execution Evidence for Sprint Review.

Durante el Sprint 1, el equipo ejecutó las tareas de desarrollo de la Landing Page de MascotaMatch siguiendo el plan establecido. Se completó el objetivo de crear, implementar y desplegar la página con una estructura HTML básica, diseño UX/UI optimizado y estilos responsivos, todo dentro del plazo asignado.

<img width="1899" height="942" alt="image" src="https://github.com/user-attachments/assets/ea59668f-a472-414b-b16e-253a875d035b" />

<img width="1905" height="944" alt="image" src="https://github.com/user-attachments/assets/45f4e51f-0027-4ce4-8c04-173e7b5f3fb9" />

<img width="1896" height="946" alt="image" src="https://github.com/user-attachments/assets/0cb431a1-293a-48bf-9b91-7a5fe8e5899c" />

<img width="1899" height="939" alt="image" src="https://github.com/user-attachments/assets/94af8220-cb60-433f-af4f-ec5a98ca6ef9" />

<img width="1894" height="943" alt="image" src="https://github.com/user-attachments/assets/5ba7db68-cccb-4e6f-9a8c-8d60f2f2aa9a" />

<img width="1896" height="935" alt="image" src="https://github.com/user-attachments/assets/7a38cdb1-ba98-4f6c-ac4a-132197f48900" />

<img width="1900" height="978" alt="image" src="https://github.com/user-attachments/assets/853de6a2-e10b-41c0-89e0-607652ed05a5" />

-Enlace al Landing Page desplegado:

### 5.2.1.6. Services Documentation Evidence for Sprint Review.

Durante el Sprint 1, el equipo de ThermaTrace se enfocó en el desarrollo de la Landing Page del proyecto, por lo que no se implementaron ni consumieron servicios (APIs) en esta etapa. La documentación de servicios se realizará en futuros sprints, conforme se avance en el desarrollo del backend y las funcionalidades dinámicas de la aplicación.

### 5.2.1.7. Software Deployment Evidence for Sprint Review.

En el Sprint 1 se realizó el lanzamiento de la primera versión del Landing Page, la cual fue publicada mediante GitHub Pages. A continuación, se muestran las evidencias correspondientes al despliegue.

Cómo acceder a la landing page:

<img width="1899" height="942" alt="image" src="https://github.com/user-attachments/assets/ea59668f-a472-414b-b16e-253a875d035b" />

<img width="1905" height="944" alt="image" src="https://github.com/user-attachments/assets/45f4e51f-0027-4ce4-8c04-173e7b5f3fb9" />

<img width="1896" height="946" alt="image" src="https://github.com/user-attachments/assets/0cb431a1-293a-48bf-9b91-7a5fe8e5899c" />

<img width="1899" height="939" alt="image" src="https://github.com/user-attachments/assets/94af8220-cb60-433f-af4f-ec5a98ca6ef9" />

<img width="1894" height="943" alt="image" src="https://github.com/user-attachments/assets/5ba7db68-cccb-4e6f-9a8c-8d60f2f2aa9a" />

<img width="1896" height="935" alt="image" src="https://github.com/user-attachments/assets/7a38cdb1-ba98-4f6c-ac4a-132197f48900" />

<img width="1900" height="978" alt="image" src="https://github.com/user-attachments/assets/853de6a2-e10b-41c0-89e0-607652ed05a5" />

### 5.2.1.8. Team Collaboration Insights during Sprint.

En el Sprint 1, el equipo se centró en el desarrollo, implementación y despliegue de la Landing Page de MascotaMatch. El trabajo se distribuyó de manera colaborativa, con cada miembro asumiendo responsabilidades en áreas clave como el desarrollo de la estructura HTML, el diseño de la interfaz y la experiencia de usuario, y la creación de estilos responsivos. Además, algunos miembros se encargaron del control de versiones y del despliegue en GitHub Pages.

La comunicación fue constante a través de plataforma usada: Discord, WhatsApp, Slack; y utilizamos herramientas como Trello, GitHub Projects para gestionar tareas y hacer seguimiento de los avances. La colaboración fue eficiente y fluida, pero se identificó la necesidad de mejorar la planificación temporal para optimizar la entrega de futuros sprints.

| Repository     | Branch     | Commit ID      | Commit Message                     | Commit Message Body                                        | Committed on Date     |
|----------------|------------|----------------|-------------------------------------|-------------------------------------------------------------|------------------------|
| ThermaTrace   | feature/index      | a1c3f4e     | feat: add landing page view                | Implementación de la vista de bienvenida personalizada       | 21 de septiembre de 2025    |
| ThermaTrace   | feature/components    | b7d8e2c     | feat: add Styles css            | Creación del módulo de edición de perfil con campos dinámicos| 21 de septiembre de 2025    |
| ThermaTrace   | feature/layout    | c2e9a8d     | feat: Styles css                 | Diseño e implementación de la sección de servicios           | 21 de septiembre de 2025    |
| ThermaTrace   | feature/base        | d4b7f3a     | feat: Styles css                | Incorporación de los tres planes de suscripción con botones  | 21 de septiembre de 2025    |
| ThermaTrace  | feature/LenguageSwitcher         | e5f6b0d     | feat: Cambio de idioma                     | Desarrollo de la sección FAQ con preguntas frecuentes        | 21 de septiembre de 2025    |
| ThermaTrace   | deploy | f9c2a1b     | chore: deploy to GitHub Pages      | Despliegue de la landing actualizada en entorno de producción| 21 de septiembre de 2025    |
