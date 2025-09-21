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

La definición de una guía de estilo y convenciones de codificación constituye un aspecto fundamental para asegurar que el código sea comprensible, sostenible y consistente durante todo el ciclo de vida del proyecto. En esta sección, se exponen las convenciones establecidas por el equipo para la programación en los lenguajes implementados en el proyecto EventGo, que comprenden HTML, CSS, JavaScript y C#.

Dichas convenciones abarcan aspectos como la denominación de variables, funciones, clases y archivos, así como las mejores prácticas para la redacción de código, siguiendo guías de estilo reconocidas y estándares de la industria. Al aplicar estas convenciones, se busca garantizar la calidad del código y optimizar la colaboración entre los integrantes del equipo, evitando inconsistencias y errores frecuentes.

**Nomenclatura General:**

Para asegurar una correcta coherencia en todo el código, se aplicarán las siguientes directrices:

- Los nombres de variables, funciones y métodos deben implementar **camelCase**.
- Los nombres de clases y componentes seguirán la convención **PascalCase**.
- Para los archivos y carpetas, se empleará la convención **kebab-case**.

Se optará por utilizar Inglés para todas las denominaciones con el objetivo de garantizar la comprensión entre los integrantes del equipo y facilitar la colaboración internacional.

Ejemplos:

- Variables: ```organizerName```, ```hostName```
- Clases: ```ListEvents```, ```Organizer```
- Archivos: ```host-message.service.js```,```organizer.controller.js```

**Espacios y Sangría**

La sangría del código en EventGo seguirá las siguientes directrices para garantizar claridad y orden:

- Se implementarán 2 espacios para la sangría en archivos HTML, CSS y JavaScript.
- En archivos C#, se aplicarán 4 espacios para la sangría.

Esta directriz permite preservar consistencia en todos los lenguajes empleados para este proyecto, facilitando la colaboración entre todos los integrantes del grupo.

**Ejemplo de HTML con sangría:**
```html
<!DOCTYPE html>
<html>
  <head>
    <title>EventGo</title>
  </head>
  <body>
    <h1>¡Encuentra a tu organizador de eventos!</h1>
    <p>No esperes más...</p>
  </body>
</html>
```

**Convenciones por Lenguaje:**

- Framework:
    - Implementaremos Vue como Framework para el desarrollo del Front-End.
- Tecnologías:
    - HTML5, CSS3 para aspectos estáticos y presentación.
    - JavaScript para incorporar interactividad y lógica.
- Diseño:
    - Tanto para el Landing Page como para la aplicación web implementaremos Material Design, con el objetivo de garantizar una correcta, moderna y optimizada experiencia de usuario.
- Biblioteca de componentes de UI:
    - Se opta por utilizar PrimeVue como biblioteca principal para componentes de la interfaz de usuario, lo cual facilita la creación de interfaces interactivas y atractivas.
- Estilo y Estructura:
    - HTML/CSS: Seguiremos la [Guía de Estilo HTML y CSS](https://google.github.io/styleguide/htmlcssguide.html) proporcionada por Google, con la finalidad de mantener consistencia y legibilidad en los archivos.
    - JavaScript: Para el código JavaScript, se aplicará la [Guía de Estilo de JavaScript de Airbnb](https://github.com/airbnb/javascript), para asegurar un código limpio, legible y sobre todo bien estructurado.
- Arquitectura del proyecto:
    - Mediante Vue, la arquitectura del proyecto será por componentes, donde cada funcionalidad, sección de la aplicación se encapsula en un archivo independiente que gestiona su propio estado y comportamiento.

**Ejemplo de Convención para un Componente en Vue:**

```vue
<template>
  <div>
    <Button label="example" @click="generateExample"/>
  </div>
</template>

<script>
  export default {
    name: 'Example',
    data() {
      return {
        numberOfExamples: 9
      };
    },
    methods: {
      generateExample() {
        if (this.numberOfExamples > 0) {
          this.numberOfExamples--;
        }
      }
    }
  };
</script>

<style scoped>
  /* Aplicando Material Design a través de PrimeVue */
  button {
    background-color: #3cc7a8;
    color: white;
  }
</style>
```

**Gherkin:**
- Para redactar las pruebas automatizadas, seguimos la convención de [Gherkin Syntax](https://cucumber.io/docs/gherkin/). Esto permite una descripción clara y precisa de los escenarios de prueba en los archivos .feature.
- Implementamos Given-When-Then para describir el comportamiento esperado en cada escenario.

**Espaciado:**
- Consideramos siempre colocar un espaciado entre operadores y parámetros en las funciones.

Ejemplo:
```vue
<script>
export default {
  data() {
    return {
      example1: 23,
      example2: 5,
      example3: 1
    };
  },
  mounted() {
    this.availableExamples = this.example1 - this.example3 - this.example2;
  }
};
</script>
```

**Comillas:**
- En JavaScript dentro de Vue, implementaremos comillas simples('') para las cadenas.

**Límite de Longitud de Línea:**
- No debe exceder las 80 columnas por línea. Si ese fuera el caso, deberemos de dividir la línea del código para una mejor claridad y limpieza.


### 5.1.4. Software Deployment Configuration ###

En esta sección se especifica la configuración necesaria para el despliegue de la solución EventGo, incluyendo los pasos clave para lograr la publicación satisfactoria de la **landing page** utilizando GitHub Pages para visualizar cada commit de la **landing page**.

A continuación, se describen los pasos para realizar el despliegue de la **landing page** del proyecto **EventGo**:

##### 1. Actualización de ramas

Asegúrese de que todas las ramas del repositorio estén actualizadas. Posteriormente, ingrese a GitHub y diríjase al repositorio del proyecto **EventGo**.

![repositorio-del-proyecto](../img/Chapter%20V/repo.png)

##### 2. Acceso a las configuraciones

Una vez dentro del repositorio, haga clic en la pestaña **Settings** en la parte superior del repositorio.

![settings.png](../img/Chapter%20V/settings.png)

##### 3. Selección de GitHub Pages

Dentro de la sección **Settings**, en el menú lateral, busque la opción denominada **Pages**. Esta opción permite configurar el despliegue de la página desde una rama específica del repositorio.

![pages.png](../img/Chapter%20V/pages.png)

##### 4. Configuración de la rama principal

En la opción **Pages**, seleccione la rama principal (generalmente denominada **main** o **master**). Posteriormente, haga clic en el botón **Save** para iniciar el proceso de deploy de la página.

<br>

##### 5. Confirmación del deploy

Una vez que GitHub complete el proceso de deploy, en la parte superior de la sección **Pages** se mostrará un mensaje de confirmación junto con el enlace generado para acceder a la **landing page** del proyecto.

<br>

##### 6. Acceso a la página

Finalmente, podrá acceder a la **landing page** desde el enlace que se generó al finalizar el deploy. Aquí está un ejemplo de enlace:  
`https://`


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
