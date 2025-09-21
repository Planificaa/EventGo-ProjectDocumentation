# Capítulo 5: Product Implementation, Validation & Deployment #

## _5.1. Software Configuration Management_ ##

Para asegurar la coherencia, seguimiento y excelencia durante todo el desarrollo de EventGo, el equipo ha establecido una serie de criterios y estándares dirigidos al control de configuraciones. En esta sección se detallan los procedimientos implementados para administrar el código fuente, establecer los ambientes de desarrollo y estructurar el proceso de implementación de la aplicación web.
Dichos lineamientos garantizan la estabilidad de las versiones del software, facilitan la colaboración efectiva entre los miembros del equipo y aseguran que los despliegues sean supervisados y replicables.

### 5.1.1. Software Development Environment Configuration ###

Para garantizar una colaboración efectiva y preservar los estándares de calidad en el desarrollo de EventGo, se ha establecido un ambiente de desarrollo unificado para la totalidad de los integrantes del equipo. A continuación, se presentan las herramientas de software empleadas en las diferentes fases del ciclo de vida del producto digital, especificando su función y su respectivo enlace de referencia o descarga.

**Diseño de Producto UX/UI**
Para el diseño de la experiencia del usuario y la interfaz de la Landing page de EventGo, se implementaron las siguientes herramientas:
* Figma: Se aplicó para el desarrollo de wireframes, maquetas y prototipos de la aplicación web. https://www.figma.com/es-es/
* UXPressia: Implementada para construir User Personas, Mapas de Empatía, Journey Maps e Impact Maps. https://uxpressia.com/
* Miro: Se aplicó para el desarrollo de los mapas de escenarios As-Is y To-Be. https://miro.com/es/

**Desarrollo de Software**
Para el desarrollo del software de la Landing Page, se implementaron los siguientes productos:
* WebStorm (Instalación local): Implementado como ambiente de desarrollo para trabajar con HTML, CSS y JavaScript. https://www.jetbrains.com/es-es/webstorm/
* Git (Instalación local): Aplicado para administrar las modificaciones de código de forma local mediante commits y ramas. https://git-scm.com/
* GitHub: Plataforma de repositorio remoto para el control de versiones del código, aplicando el flujo GitFlow para asegurar un desarrollo estructurado. https://github.com/

**Gestión de Proyectos y Colaboración**
En la administración de proyectos y colaboración del equipo se implementaron:
* Trello: Aplicado para la planificación y monitoreo de actividades, organizadas en listas de "por hacer", "en progreso" y "completado".
* WhatsApp: Canal de comunicación inmediata para coordinar progresos, resolver consultas rápidas y realizar recordatorios. https://web.whatsapp.com/
* Discord: Implementado como plataforma de comunicación por voz y chat, facilitando reuniones ágiles y discusiones técnicas grupales. https://discord.com/
* Zoom: Herramienta implementada para ejecutar reuniones virtuales más estructuradas, presentaciones de progresos y coordinación integral del equipo. https://www.zoom.com/es

**Documentación de Software**
Para la documentación del proyecto se implementaron las siguientes herramientas:
* Vertabelo: Herramienta implementada para el diseño, desarrollo y documentación colaborativa de bases de datos. https://vertabelo.com/
* Lucidchart: Aplicada para el desarrollo de diagramas UML, wireflows y user flows que contribuyen en la planificación y visualización del sistema. https://www.lucidchart.com/pages
* Structurizr: Herramienta aplicada para modelar la arquitectura de software mediante diagramas C4. https://structurizr.com/

**Pruebas de Software**
En cuanto a la verificación del software:
* WebStorm Preview: Se implementó la funcionalidad de vista previa integrada en WebStorm para revisar manualmente archivos .md y otros componentes previo a su integración en el repositorio de GitHub. https://www.jetbrains.com/es-es/webstorm/

### 5.1.2. Source Code Management ###

La administración del código fuente constituye un elemento esencial en el desarrollo colaborativo de software, dado que facilita un control eficaz sobre las modificaciones ejecutadas en el proyecto durante su ciclo de vida completo. En esta sección, se expone el sistema de control de versiones establecido en el proyecto EventGo, empleando GitHub como plataforma central. Asimismo, se especifican las convenciones de trabajo adoptadas por el equipo, tales como el modelo GitFlow, el versionado semántico (Semantic Versioning) y las convenciones de commit mediante Conventional Commits. Dichos lineamientos garantizan un desarrollo estructurado y una integración continua eficiente entre los integrantes del equipo.

**URL de los Repositorios:**
- Organización: [https://github.com/Planificaa](https://github.com/Planificaa)
- Reporte: [https://github.com/Planificaa/EventGo-ProjectDocumentation](https://github.com/Planificaa/EventGo-ProjectDocumentation)
- Landing Page: [https://github.com/Planificaa/EventGo-Landing-Pague](https://github.com/Planificaa/EventGo-Landing-Pague)

**Estructura de Ramas:**
Para preservar un flujo organizado en el desarrollo y optimizar la colaboración, se ha establecido el modelo GitFlow, generando las siguientes ramas:
- Master Branch: Rama principal (main) que contiene las versiones estables del proyecto. El resto de ramas se derivan de esta.
- Develop: Rama secundaria donde se consolidan todas las funcionalidades nuevas previo a su fusión con la rama main.
- Feature Branches: Para esta primera entrega son ramas dedicadas a cada capítulo del informe, permitiendo que cada integrante trabaje de forma independiente sin comprometer el desarrollo principal.
- Release Branch: Rama generada cuando el equipo determina que la rama develop está preparada para convertirse en una nueva versión estable.
- Cover: Rama destinada a los componentes de la portada del informe.
- Student-outcome: Rama dedicada a los resultados de cada uno de los integrantes en relación con el proyecto.
- Bibliography: Rama cuya funcionalidad es desarrollar la bibliografía del informe del proyecto.
- Annexes: Rama destinada a enumerar los anexos de cada entrega del informe.

**Convenciones de commits:**
Para la redacción de commits en el proyecto EventGo, se sigue la convención 'Conventional Commits', la cual cuenta con un formato estándar para facilitar la lectura y comprensión del historial de cambios dentro del proyecto.

```
    <type>[optional scope]: <description>
    
    [optional body]
    
    [optional footer(s)]
```
- Type:
    - feat: Añadir una nueva característica.
    - fix: Correción de errores.
    - docs: Modificaciones en la documentación.
    - style: Cambios que no afectan la lógica del código.
    - refactor: Modificaciones que no añaden características y/o errores.
    - test: Adición/Modificación de pruebas.


- Scope: Brinda información extra acerca del área del codigo afectado.
```
   feat(auth): add register functionality.
```
**Ejemplos básicos de commits:**
```
   feat(login): add organizer authentication module.
```
```
   fix(payment): resolve payment security issue.
```
```
   docs(README): update index instructions.
```

### 5.1.3. Source Code Style Guide & Conventions ###



### 5.1.4. Software Deployment Configuration ###



## _5.2. Landing Page, Services & Applications Implementation_ ##

### 5.2.1. Sprint 1 ###

#### 5.2.1.1. Sprint Planning 1 ####



#### 5.2.1.2. Aspect Leaders and Collaborators ####



#### 5.2.1.3. Sprint Backlog 1 ####



#### 5.2.1.4. Development Evidence for Sprint Review ####



#### 5.2.1.5. Execution Evidence for Sprint Review ####



#### 5.2.1.6. Software Deployment Evidence for Sprint Review ####



#### 5.2.1.7. Software Deployment Evidence for Sprint Review ####

#### 5.2.1.8. Team Collaboration Insights during Sprint ####
