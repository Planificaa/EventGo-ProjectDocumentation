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

![settings-page.png](../img/Chapter%20V/settings-page.png)

##### 3. Selección de GitHub Pages

Dentro de la sección **Settings**, en el menú lateral, busque la opción denominada **Pages**. Esta opción permite configurar el despliegue de la página desde una rama específica del repositorio.

![pages.png](../img/Chapter%20V/pages.png)

##### 4. Configuración de GitHub Actions

En la opción **Pages**, seleccione la opción "Github Actions" y luego en la opción de "Configure" en el recuadro de 'Static HTML'
Se aperturará un nuevo archivo de configuración en el cual se debe cambiar la rama por "main" y la carpeta por "./public". Finalmente, haga clic en el botón verde de "Start commit" para guardar los cambios.

![static-yml.png](../img/Chapter%20V/static-yml.png)

<br> 


##### 5. Confirmación del deploy

Una vez que GitHub complete el proceso de deploy, en la parte superior de la sección **Pages** se mostrará un mensaje de confirmación junto con el enlace generado para acceder a la **landing page** del proyecto.

<br>

![deploy-static-1.png](../img/Chapter%20V/deploy-static-1.png) 
<br>

![deploy.png](../img/Chapter%20V/deploy.png)

De esta manera, cuando se realice un nuevo commit desdelaramamain, GitHub automáticamente actualizará la **landing page** con los cambios realizados.

##### 6. Acceso a la página

Finalmente, podrá acceder a la **landing page** desde el enlace que se generó al finalizar el deploy. Aquí está un ejemplo de enlace:  
`https://planificaa.github.io/EventGo-Landing-Pague/`

![despliegue-landing.png](../img/Chapter%20V/despliegue-landing.png)


## _5.2. Landing Page, Services & Applications Implementation_ ##

### 5.2.1. Sprint 1 ###

En el Sprint 1, se enfocó el trabajo en diseñar y desarrollar la Landing Page de EventGo, con el objetivo de presentar de forma clara y atractiva los beneficios de la plataforma para organizadores y anfitriones de eventos. Durante este sprint, se trabajó en una estructura de navegación intuitiva y una disposición visual que permitiera destacar las características principales del servicio. Se organizó el equipo para distribuir las tareas y lograr un diseño completamente responsivo, asegurando que la página se visualice correctamente en distintos tamaños de pantalla.

#### 5.2.1.1. Sprint Planning 1 ####

|             Sprint #             |                                                                                                                                                                                                                                                                                                                                                                                                                                                          Sprint 1                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
|:--------------------------------:|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------:|
|  **Sprint Planning Background**  |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
|               Date               |                                                                                                                                                                                                                                                                                                                                                                                                                                                          12/08/25                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
|               Time               |                                                                                                                                                                                                                                                                                                                                                                                                                                                        20:30 horas                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
|             Location             |                                                                                                                                                                                                                                                                                                                                                                                                                                               Reunión virtual - Zoom/Discord                                                                                                                                                                                                                                                                                                                                                                                                                                               |
|           Prepared By            |                                                                                                                                                                                                                                                                                                                                                                                                                                                      Deybbi Crisanto                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
|            Attendees             |                                                                                                                                                                                                                                                                                                                                                                                                           - July Paico <br> - Deybbi Crisanto  <br> - Didier Meza  <br> - Bryan Hermoza  <br> - Fernando Paucar                                                                                                                                                                                                                                                                                                                                                                                                            |
|    Sprint n-1 Review Summary     |                                                                                                                                                                                                                                                                                                                                                                                                                                 Este constituye el primer sprint a ejecutar por el equipo                                                                                                                                                                                                                                                                                                                                                                                                                                  |
| Sprint n-1 Retrospective Summary |                                                                                                                                                                                                                                                                                                                                       Durante este sprint se acordó establecer reuniones periódicas para realizar un seguimiento del progreso y cumplir las metas establecidas. Además se destacó el compromiso de los integrantes del equipo por alcanzar los objetivos definidos.                                                                                                                                                                                                                                                                                                                                        |
|  **Sprint Goal & User Stories**  |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
|          Sprint 1 Goal           | El enfoque de este sprint se centró en desarrollar la Landing Page de EventGo, proporcionando a los nuevos usuarios una interfaz visualmente atractiva y de fácil navegación que les permitiera conocer a profundidad la propuesta. Se enfocó en construir secciones clave como Inicio, Beneficios, Funcionalidades, Planes, Quiénes Somos y About the Product, con el objetivo de comunicar de forma clara el valor que EventGo aporta a organizadores y anfitriones de eventos. <br/>Se considera que esto facilita a los usuarios la comprensión rápida del funcionamiento de la plataforma, generando una experiencia inicial positiva y confiable. <br/>Se validará este trabajo cuando la Landing Page esté completamente operativa, con una navegación fluida, contenido informativo en cada sección y una experiencia responsiva que permita a los usuarios interactuar correctamente desde cualquier dispositivo. |
|        Sprint 1 Velocity         |                                                                                                                                                                                                                                                                                                                                                                                                                                              Velocidad de 18 - Primer Sprint                                                                                                                                                                                                                                                                                                                                                                                                                                               |
|       Sum of Story Points        |                                                                                                                                                                                                                                                                                                                                                                                                                                                 Sprint 1 - 18 Story Points                                                                                                                                                                                                                                                                                                                                                                                                                                                 |

#### 5.2.1.2. Aspect Leaders and Collaborators ####

|            Team Member            | GitHub Username |    Header    | Footer | Inicio | Beneficios | Funcionalidades | Planes | About Us | About the product |
|:---------------------------------:|:---------------:|:------------:|:------:|:------:|:----------:|:---------------:|:------:|:--------:|:-----------------:|
|   Hermoza Paredes, Bryan Norberto |     WasNeo      |      C       |   C    |   C    |     C      |        C        |   L    |    L     |         C         |
|  Meza Solórzano, Didier Sebastian |   DidierMeza    |      L       |   C    |   C    |     C      |        C        |   C    |    C     |         C         |
|  Crisanto Calle, Deybbi Anderson  |     Dacc03      |      C       |   L    |   C    |     C      |        C        |   C    |    C     |         C         |
| Paucar Zenteno, Jesús Fernando    |  devFernando22  |      C       |   C    |   L    |     C      |        C        |   C    |    C     |         L         |
|   Paico Calderon, July Zelmira    |   u20211d760    |      C       |   C    |   C    |     L      |        L        |   C    |    C     |         C         |

#### 5.2.1.3. Sprint Backlog 1 ####

Para el sprint 1 usamos la herramienta trello para organizar las tareas del equipo.

Enlance: https://trello.com/invite/b/68cf9fb9c584710a5768a36f/ATTIfe3ba144603fbac432bba489eb041af805EA0880/eventgo-sprint-1 

![trello-board.png](../img/Chapter%20V/trello-board.png)

En el tablero se pueden visualizar las user stories que se abarcaron en este sprint, así como el estado de las mismas (To-Do, In-Progress, Review, To-Fix, Done) y se les asignó story points con fechas de entrega.

|    Sprint #    |                                                 | | Sprint 1 | | |                                  |                                               |
|:--------------:|:-----------------------------------------------:|:--------:|:--------:|:--------:|:--------:|:--------------------------------:|:---------------------------------------------:|
| **User Story** |                                                 | **Work-Item/Task** | | | |                                  |                                               |
|    **ID**      |                    **Title**                    | **ID** | **Title** | **Description** | **Estimation (Hours)** |         **Assigned To**          | **Status (To-Do/ In-Process/To-Review/Done)** |
|       ID       |            US01 Navegación sencilla             | TA01 | Menu con hipervinculacion | Cada hipervinculo debe de redirigir a una sección específica de la landing page | 2 | Meza Solórzano, Didier Sebastian |                     Done                      |
|       ID       |          US02 Propuesta de valor clara          | TA01 | Hero | Se debe desarrollar un banner con una frase que represente a la aplicación web | 2 |  Paucar Zenteno, Jesús Fernando  |                     Done                      |
|       ID       |            US05 Llamada a la acción             | TA01 | Call to action | Se debe desarrollar un botón call to action que redirija a la aplicación web | 1 | Hermoza Paredes, Bryan Norberto  |                     Done                      |
|       ID       |           US03 Información segmentada           | TA01 | Benefits | crear la sección de beneficios de la plataforma web, que muestre los atractivos de la propuesta | 2 |   Paico Calderon, July Zelmira   |                     Done                      |
|       ID       |      US04 Funcionalidades de la aplicación      | TA01 | Funcionalidades | Se debe desarrollar una sección que liste las funcionalidades que ofrece la plataforma web | 2 |   Paico Calderon, July Zelmira   |                     Done                      |
|       ID       | US06 Visualización de tutorial de la aplicación | TA01 | About the product | Se desarrolla sección donde figura un video que explica el funcionamiento de la plataforma web. | 1 |   Paico Calderon, July Zelmira   |                     Done                      |
|       ID       |           US07 Confianza y seguridad.           | TA01 | About us | Debe presentar una sección con información del equipo de trabajo | 2 | Crisanto Calle, Deybbi Anderson  |                     Done                      |
|       ID       |             US08 Velocidad de carga             | TA01 | Loading | Se debe implementar funciones que permitan fácil loading a carga de información | 2 |  Paucar Zenteno, Jesús Fernando  |                     Done                      |
|       ID       |         US09 Visualización de precios.          | TA01 | Suscripciones | Debe presentar la información de los precios de cada plan de suscripción | 2 | Hermoza Paredes, Bryan Norberto  |                     Done                      |
|       ID       |             US10 Diseño responsive              | TA01 | Responsive | Se desarrolla implementar las configuraciones de quejas que diferentes tamaños de pantallas | 2 | Crisanto Calle, Deybbi Anderson  |                     Done                      | 

#### 5.2.1.4. Development Evidence for Sprint Review ####

![commits-landing.png](../img/Chapter%20V/commits-landing.png)

#### 5.2.1.5. Execution Evidence for Sprint Review ####

**Landing Page**
URL: https://planificaa.github.io/EventGo-Landing-Pague/ 

Despues de finalizar el sprint 1, hemos logrado implementar todas las funcionalidades de nuestra landing page, con excepción de la sección about the product, que todavía no contiene un video que muestre el funcionamiento de nuestra plataforma web, puesto que la plataforma web aún no existe en este sprint. A continuación, te invitamos a explorar nuestros avances a través de imágenes que muestran el resultado obtenido.

***header:*** La barra de navegación que nos ayudará a redirigirnos por las diferentes secciones de la landing page.

![header-v1.png](../img/Chapter%20V/header-v1.png) 

***Hero:*** Banner que contiene un botón que te llevará a registrarte a nuestra apliación web.

![hero-v1.png](../img/Chapter%20V/hero-v1.png) 

***Functionality:*** Seccion donde los visitantes de la lading page podrán ver como es que funciona nuestra aplicacion y que les ofrece

![functionalities-v1.png](../img/Chapter%20V/functionalities-v1.png)

***Benefits:*** Sección donde los visitantes de la landing page podrán ver los beneficios principales que les ofrece nuestra aplicación.

![benefits.png](../img/Chapter%20V/benefits.png) 

***Plans:*** Sección donde los visitantes de la landing page podrán ver los diferentes planes de suscripción que ofrecemos.

![plans.png](../img/Chapter%20V/plans.png) 

***About Us:*** Sección donde los visitantes de la landing page podrán ver información sobre nuestro equipo de trabajo.

![about-us-v1.png](../img/Chapter%20V/about-us-v1.png) 

***Footer:*** Pie de página que contiene información de contacto y redes sociales.

![footer-v1.png](../img/Chapter%20V/footer-v1.png)

#### 5.2.1.6. Services Documentation Evidence for Sprint Review. ####


#### 5.2.1.7. Software Deployment Evidence for Sprint Review ####

Para el despliegue de nuestra Landing Page hemos utilizado GitHub Pages. Para hacer esto, hemos trabajado en un repositorio de GitHub donde divimos el trabajo en ramas. En la sección de configuración y Pages, seleccionamos la rama main para desplegar nuestra web.

**Link de la landing page desplegada:** https://planificaa.github.io/EventGo-Landing-Pague

![evidence-github-actions-deploy-landing.png](../img/Chapter%20V/evidence-github-actions-deploy-landing.png)

#### 5.2.1.8. Team Collaboration Insights during Sprint ####

La meta de este sprint fue la implementación de la Landing Page. Para llevar a cabo este objetivo, hicimos uso de diversas herramientas como GitHub, WebStorm, HTML, CSS y JavaScript. Como evidencias del trabajo realizado tenemos los diagramas de flujo que representan los commits realizados por cada miembro del equipo AngelDevs.

![commits-landing.png](../img/Chapter%20V/commits-landing.png)
La imagen muestra un gráfico de barras donde se refleja la cantidad de commits hechos por cada miembro del equipo en la Landing Page.

![contributors-landing.png](../img/Chapter%20V/contributors-landing.png)
En esta imagen se refleja la el nivel de modificaciones realizadas por los commits de cada integrante en el repositorio de la Landing Page.

![network-part1-landing.png](../img/Chapter%20V/network-part1-landing.png)
![network-part2-landing.png](../img/Chapter%20V/network-part2-landing.png)
En la imagen se puede apreciar las ramas feature creadas para el repositorio y las fechas en que se unieron, así como se aplicó gitflow para su desarrollo.