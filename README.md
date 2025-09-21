# Capítulo V: Product Implementation, Validation & Deployment
## 5.1. Software Configuration Management.
La gestion de la configuración del software es un proceso esencial para garantizar la integridad y coherencia del producto a lo largo de su ciclo de vida. En este capítulo, se detallan las prácticas y herramientas utilizadas para gestionar eficazmente la configuración del software en el proyecto ThermaTrace.

### 5.1.1. Software Development Environment Configuration.

**Project Management**

- Discord:

Se utiliza Discord como plataforma principal de comunicación y coordinación del equipo. Aquí se llevan a cabo reuniones, discusiones y se comparten actualizaciones del proyecto.

- Trello:

Trello se emplea para la gestión de tareas y seguimiento del progreso del proyecto. Se crean tableros, listas y tarjetas para organizar las actividades y asignarlas a los miembros del equipo.

**Requirements Management**
- Miro:
Utilizamos Miro para la gestión y visualización de requisitos. Esta herramienta permite crear diagramas, mapas mentales y flujos de trabajo que facilitan la comprensión y el seguimiento de los requisitos del proyecto.

- UXPressia:

Utilizamos UXPressia para crear mapas de empatía, customer journeys y otros artefactos de experiencia de usuario que ayudan a definir y gestionar los requisitos desde la perspectiva del usuario.

- Structurizr:
Utilizamos Structurizr para modelar y documentar la arquitectura del software, lo que ayuda a gestionar los requisitos técnicos y de diseño del proyecto.

**Product UX/UI Desingn**

- Figma:
Utilizamos Figma para el diseño de la interfaz de usuario y la experiencia de usuario (UX/UI). Esta herramienta permite la colaboración en tiempo real y facilita la creación de prototipos interactivos.

- LucidChart:
LucidChart se utiliza para crear diagramas de flujo, wireframes y otros elementos visuales que apoyan el diseño UX/UI del producto.

**Software Development**
- HTML5:
Usamos HTML5 como el lenguaje de marcado principal para estructurar el contenido de las páginas web del proyecto.

- CSS:
CSS se utiliza para diseñar y estilizar las páginas web, asegurando una apariencia atractiva y coherente con la identidad visual del proyecto.

- Javascript:
Utilizamos JavaScript para agregar interactividad y funcionalidades dinámicas a las páginas web del proyecto.

- WebStorm:
Utilizamos WebStorm como entorno de desarrollo integrado (IDE) para escribir, depurar y probar el código del proyecto.

### 5.1.2. Source Code Management.
El proyecto ThermaTrace, una solución digital orientada a hospitales y farmacias, se desarrolla bajo un enfoque profesional que prioriza la calidad, la seguridad de los datos y la escalabilidad del sistema. La arquitectura se fundamenta en principios de diseño modular y la metodología de Clean Architecture, lo que garantiza una separación clara de responsabilidades, la reutilización de componentes y la facilidad de mantener y evolucionar la plataforma en el tiempo. Este enfoque permite integrar nuevos módulos relacionados con el control de temperatura, gestión de inventario y trazabilidad de medicamentos sin comprometer la estabilidad general del sistema.

Para el desarrollo frontend, el equipo utiliza un entorno moderno optimizado para la creación de interfaces intuitivas y accesibles, que ofrecen a los médicos y farmaceuticos una experiencia ágil y clara. La interfaz está diseñada para priorizar la visualización de datos críticos como reportes de temperatura, estado del inventario y alertas de seguridad, aplicando principios de usabilidad y accesibilidad que garantizan su correcto uso en contextos de alta exigencia como hospitales y cadenas de farmacias. Además, la organización modular de los componentes permite mantener la coherencia visual y facilitar futuras ampliaciones en la experiencia de usuario.

En cuanto a la estructura técnica, se adoptan buenas prácticas de colaboración en equipo, control de versiones y automatización de flujos de trabajo, lo cual asegura uniformidad y calidad en el código. Se incorporan metodologías ágiles para iterar en el diseño y validación de prototipos con usuarios reales, verificando que los flujos de interacción respondan a las necesidades específicas de las instituciones de salud. Con ello, ThermaTrace no solo se consolida como una herramienta tecnológica robusta, sino también como una plataforma confiable que fortalece la seguridad en la gestión de medicamentos y optimiza los procesos internos en hospitales y farmacias.

Finalmente, se mantiene un repositorio denominado upc-pre-202520-1ASI0729-7357 (https://github.com/upc-pre-202520-1ASI0729-7357), donde se concentran versiones exploratorias y entornos de prueba orientados a hospitales y farmacias. Este repositorio funciona como espacio experimental para validar nuevas funcionalidades relacionadas con la gestión de temperatura, trazabilidad de medicamentos y optimización de inventarios, antes de su incorporación al sistema central de producción. Además, permite realizar pruebas funcionales y demostraciones internas con usuarios clave, asegurando que las mejoras propuestas respondan a las necesidades reales del sector salud.

![Repositorios de ThermaTrace](https://scontent.flim15-1.fna.fbcdn.net/v/t1.15752-9/551311708_1323660692748451_3932849482348297948_n.png?_nc_cat=103&ccb=1-7&_nc_sid=0024fc&_nc_ohc=dJu0MelnnfEQ7kNvwGjEPuJ&_nc_oc=AdkwQjuJrYOZrD6Cdh0tSjsHqFvTlv_qG7yvHDI127Xs5b21ei5PSNgqIxWtj3nLOdTAG9NQQsGrlwbl8zTocC29&_nc_ad=z-m&_nc_cid=0&_nc_zt=23&_nc_ht=scontent.flim15-1.fna&oh=03_Q7cD3QHdjnqPex30s0KJaw66HYPHW3BnFRk4unhWH4G6i13FPw&oe=68F75E84)
<br>

### 5.1.3. Source Code Style Guide & Conventions.

El mantenimiento de un estilo de código estandarizado y una arquitectura bien definida es fundamental para garantizar la escalabilidad, mantenibilidad y colaboración efectiva en el desarrollo de ThermaTrace. En este proyecto se han adoptado convenciones de codificación y lineamientos de arquitectura que aseguran calidad técnica, legibilidad y consistencia en todos los módulos, alineándose con prácticas recomendadas de la industria y metodologías modernas de ingeniería de software.

**Arquitectura y organización del sistema**

Desde el punto de vista arquitectónico, se emplea el modelo C4 de Simon Brown, que permite describir el sistema en distintos niveles: contexto, contenedor, componente y código. Este enfoque facilita la comunicación entre perfiles técnicos y no técnicos, permitiendo que tanto desarrolladores como stakeholders de hospitales y farmacias comprendan la lógica del sistema. La organización sigue principios de Domain-Driven Design (DDD) y Clean Architecture, lo que asegura una clara separación entre presentación, aplicación, dominio e infraestructura. Gracias a esta estructura, se logra un bajo acoplamiento, pruebas más efectivas y flexibilidad para incorporar nuevas funcionalidades como módulos de trazabilidad, control de temperatura en tiempo real o gestión de inventarios críticos.

**Frontend: Angular**

En el frontend, se utiliza Angular como framework principal, con una arquitectura basada en módulos y componentes reutilizables. La estructura generada por el Angular CLI facilita la estandarización entre miembros del equipo. La nomenclatura sigue convenciones claras: clases en PascalCase y archivos en kebab-case. Además, se aplican prácticas recomendadas como:

- Detección de cambios con OnPush.
- Separación entre lógica y presentación.
- Inyección de dependencias vía constructor.
- Internacionalización con @angular/localize, gestionando archivos JSON de idioma.

**Alineación con guías de estilo estándar**

Aunque el detalle completo de las guías externas (como la Google HTML/CSS Style Guide o la Angular Style Guide) no se incluye de manera exhaustiva en el reporte, la organización y convenciones observadas en el código de ThermaTrace demuestran una alineación con estas prácticas. El uso del inglés en nombres de variables, funciones y componentes asegura coherencia internacional, mientras que la aplicación de linting automatizado refuerza la mantenibilidad y la calidad del sistema.

### 5.1.4. Software Deployment Configuration.
Para gestionar el desarrollo de ThermaTrace de manera colaborativa, el equipo empleó la funcionalidad de forks en GitHub. Cada integrante creó un fork del repositorio principal alojado en la cuenta oficial, asignando un nombre identificador. Esta práctica permitió a los miembros del grupo disponer de un entorno propio donde experimentar, probar nuevas funciones o realizar ajustes sin comprometer directamente la estabilidad del código base.

Una vez creado, el fork quedaba disponible en el perfil de cada colaborador como una copia independiente del repositorio original, lista para ser modificada y sincronizada según el avance del proyecto. Este flujo de trabajo garantizó la seguridad e integridad del repositorio upstream, mientras fomentaba la autonomía individual y la organización del equipo, asegurando que todas las mejoras o correcciones pasaran por un proceso de validación antes de incorporarse oficialmente al sistema central de ThermaTrace.

![imagen deploy 1](https://scontent.flim15-1.fna.fbcdn.net/v/t1.15752-9/552223944_1701654900496595_1803262069206559475_n.png?_nc_cat=103&ccb=1-7&_nc_sid=0024fc&_nc_ohc=fCsE5_KsgoEQ7kNvwG3rLII&_nc_oc=AdkTGB493FgiNCQwgtFHSbbDtqDD-3G3A38irKxA2bgLWz45Wc-a79x1LZbYpHy-yy6X1lctu_XC575-Y6ZchPoC&_nc_ad=z-m&_nc_cid=0&_nc_zt=23&_nc_ht=scontent.flim15-1.fna&oh=03_Q7cD3QESHZ8HZuobdmmHm2wGfDPxEcUZcBjzCoIaSSin0C8LPA&oe=68F78028)
![imagen deploy 2](https://scontent.flim15-1.fna.fbcdn.net/v/t1.15752-9/551712165_1139658748260941_9019660909457222181_n.png?_nc_cat=109&ccb=1-7&_nc_sid=0024fc&_nc_ohc=9f936UuILAsQ7kNvwGkWLRJ&_nc_oc=Adl7KuWGcCZtRvliQR2jK9AWnmo_CqdFhZtnDooMd6-6m4ArdzvEVnJcBLUY1K2BvbVW0NQTjhj1_o_wtYGrFERK&_nc_ad=z-m&_nc_cid=0&_nc_zt=23&_nc_ht=scontent.flim15-1.fna&oh=03_Q7cD3QFcwaRaLPiQPuPdrY42PbauW2ERYxF-nqRfq0Cj90g5XQ&oe=68F75F26)
![imagen deploy 3](https://scontent.flim15-1.fna.fbcdn.net/v/t1.15752-9/550981287_1424460261979165_2063420566730392179_n.png?_nc_cat=110&ccb=1-7&_nc_sid=0024fc&_nc_ohc=brCVl0LZ7P4Q7kNvwFkbnQp&_nc_oc=AdnmbXIJnTETzsU-fgCuwDbi_RWwxixHy7udFtXOmVT1KNqHVFdwYeN_CEO7xsQSjtqiOPUZSlqZhMesgk8TWoxB&_nc_ad=z-m&_nc_cid=0&_nc_zt=23&_nc_ht=scontent.flim15-1.fna&oh=03_Q7cD3QERic9QDaBvpA0yPQ-W72p0mX5IKYIW9et7u43p9EAaiQ&oe=68F77C84)

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

-Enlace al Landing Page desplegado: <https://upc-pre-202520-1asi0729-7357.github.io/LANDING-PAGE-/>

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
