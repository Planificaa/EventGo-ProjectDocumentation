# Capítulo 5: Product Implementation, Validation & Deployment #

#
# _5.1
. Software Con
figuration Management_ ##

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

## 5.2.2. Sprint 2
### 5.2.2.1. Sprint Planning 2.

A continuación, se detalla, en la tabla siguiente, información sobre el planeamiento del segundo sprint. Además, para este sprint se definieron dos objetivos para cubrir los aspectos de sitio web estático y aplicación front-end. El primer objetivo se centra en desarrollar una mejora visual para el sitio web estático y añadir secciones para Call-To-Action para los visitantes del sitio web. Por otro lado, el segundo objetivo se centra en el desarrollo y despliegue de la primera versión de la aplicación front-end de Planifica.

| Sprint #                                     | Sprint 2                                               |
|----------------------------------------------|--------------------------------------------------------|
| <b> Sprint planning Background </b>          | --                                                     |
| Date                                         | 2025/10/06                                             |
| Time                                         | 11:00 AM                                               |
| Location                                     | Reunión por Discord |
| Prepared By                                  | Deybbi Anderson Crisanto Calle                       |
| Attendees                                    | Crisanto Calle  Deybbi Anderson / Paico Calderon July Zelmira / Paucar Zenteno Jesus Fernando / Meza Solòrzano Didier Sebastiàn   |
| Sprint 1 Review Summary                      | En el sprint anterior, el equipo completó una primera vista de la Landing Page implementando las secciones y estilos básicos que necesitará, como Beneficios, Planes e Información sobre la Startup. |
| Sprint 1 Retrospective Summary               | El principal aspecto que el equipo debe mejorar es la mayor comunicación entre los miembros para que se mantengan al tanto del progreso de cada uno. Ahora, el plan para el próximo sprint es trabajar de forma más organizada para que cada miembro sepa qué hacer.  |
| <b> Sprint Goal & User Stories </b>          | --                                                     |
| Sprint 2 Goals                               | <b> Nuestro objetivo en este sprint es desarrollar la primera versión funcional del Frontend de EventGo utilizando Vue, priorizando la creación de componentes reutilizables, un diseño responsive y una navegación fluida. Nos enfocaremos en implementar las secciones ya definidas con un código limpio, modular y mantenible, apoyándonos en librerías de UI modernas para lograr una experiencia visual coherente. La meta es entregar una versión navegable y adaptable a distintos dispositivos, que permita realizar pruebas tempranas de usabilidad y verificar que la interfaz cumpla con los objetivos de claridad, atractivo visual y facilidad de uso. Esta entrega será validada mediante una demo funcional, desplegada de forma local o en un hosting temporal (como Netlify o Vercel), para obtener feedback interno antes de avanzar hacia las etapas de integración con el backend o funcionalidades más complejas. | 
| Sprint 2 Velocity                            | 26                                                    |
| Sum of Story Points                          | 32                                                     |

### 5.2.2.2. Aspect Leaders and Collaborators.

En esta sección, se incluye la matriz de liderazgo y colaboración desarrollada para este segundo sprint. Los principales aspectos que se toman en cuenta en este sprint se centran en cada las principales secciones que presenta el Front-End Web Application. Para esto, hemos definido las siguientes secciones: TaskManagement, ProfileManagement ,QuotesManagement, Event Management y Direc-comunication)

| Team Member                        | GitHub Username | TaskManagement | ProfileManagement | QuotesManagement | Event Management | Direc-comunication| 
|------------------------------------|-----------------|---------------------|-----------|-------------------|---------------------------------------------------|---------|
| Crisanto Calle Deybbi Anderson     | Dacc03    |         |         |     L     |            |   L     |         
| Paico Calderon July Zelmira   | JulyP      |         |          |         |      L      |       |     
| Paucar Zaenteno Jesus Fernando       | devFernando22      |    L     |          |          |           |        | 
| Meza Solòrzano Didier Sebastiàn    | Didier04x       |       |   L       |          |            |        |

#### 5.2.2.3.Sprint Backlog 2.

Para el sprint 2 usamos la herramienta trello para organizar las tareas del equipo.

Link de enlace del Trello: https://trello.com/invite/b/68e9c721f4d00cbac602db94/ATTI8f88418c7ca80434b0aeff65f24d3d4fEF5EC824/eventgo-sprint-2 

![trello-sprint-2.png](../img/Chapter%20V/trello-sprint-2.png)

En el tablero se pueden visualizar las user stories que se abarcaron en este sprint, así como el estado de las mismas (To-Do, In-Progress, Review, To-Fix, Done) y se les asignó story points con fechas de entrega.


<table>
  <tr>
    <td> <strong>Sprint #</strong></td>
    <td align="center" colspan="7"> <strong>Sprint 2</strong> </td>
  </tr>
   <tr>
    <td align="center" colspan="2"> <strong>User Story</strong></td>
    <td align="center" colspan="6"> <strong>Work-item/Task</strong></td>
  </tr>
  <tr>
    <td align="center"> <strong>ID</strong> </td>
    <td align="center"> <strong>Title</strong></td>
    <td align="center"> <strong>ID</strong> </td>
    <td align="center"> <strong>Title</strong></td>
    <td align="center"> <strong>Description</strong></td>
    <td align="center"> <strong>Estimation (Hours)</strong></td>
    <td align="center"> <strong>Assigned To</strong></td>
    <td align="center"> <strong> Status (To-do/In-Process/To-Review/Done)  </strong></td>
  </tr>
  <!---------------------------------------------------------------------- -->
  <tr>
    <td rowspan="3" align="center"> US24 </td>
    <td rowspan="3" align="center"> Solicitar cotización a un organizador</td>
    <td align="center"> TA01 </td>
     <td align="center"> Create a quote management</td>
    <td align="center">Crear un formulario para generar una cotización </td>
    <td align="center"> 3</td>
    <td align="center"> Crisanto Calle, Deybbi Anderson</td>
    <td align="center">Done</td>
  </tr>
  <tr>
    <td align="center"> TA02 </td>
     <td align="center"> Add component to create and edit services into a quote</td>
    <td align="center"> Crea componentes para crear y editar cotizaciones en una tabla</td>
    <td align="center"> 3</td>
    <td align="center"> Crisanto Calle, Deybbi Anderson</td>
    <td align="center">Done</td>
  </tr>
  <tr>
    <td align="center"> TA03 </td>
     <td align="center">Add external service for CRUD operations of quotes</td>
    <td align="center"> Crea un servicio para acceder al fake api y hacer operaciones de CRUD</td>
    <td align="center"> 2</td>
    <td align="center"> Crisanto Calle, Deybbi Anderson</td>
    <td align="center">Done</td>
  </tr>
<!----------------------------------------------->
  <tr>
    <td rowspan="1" align="center"> US21 </td>
    <td rowspan="1" align="center"> gestion de mensajes</td>
    <td align="center"> TA01 </td>
    <td align="center"> Create a message component to view messages </td>
    <td align="center"> Se llama a un servicio de mensajes para el organizador.</td>
    <td align="center"> 2</td>
    <td align="center"> Deybbi Anderson, Crisanto Calle</td>
    <td align="center">Done</td>
  </tr>
  <!----------------------------------------------->
  <tr>
    <td rowspan="1" align="center"> US19 </td>
    <td rowspan="1" align="center"> Gestión de presupuesto del evento</td>
    <td align="center"> TA01 </td>
    <td align="center"> Add external service for CRUD operations of services into a quote</td>
    <td align="center"> Se crea un servicio para acceder al apifake y hacer operaciones de crud.</td>
    <td align="center"> 2</td>
    <td align="center"> Crisanto Calle, Deybbi Anderson</td>
    <td align="center">Done</td>
  </tr>
<!-------------------------------------------------->
  <tr>
    <td rowspan="3" align="center"> US18 </td>
    <td rowspan="3" align="center"> Lista de tareas del evento</td>
    <td align="center"> TA01 </td>
    <td align="center"> Create a task management board</td>
    <td align="center"> crea un board de gestión de tareas.</td>
    <td align="center"> 2</td>
    <td align="center"> Paucar Zaenteno Jesus Fernando </td>
    <td align="center"> Done</td>
  </tr>
  <tr>
    <td align="center"> TA02 </td>
     <td align="center">Add a component to create and edit tasks</td>
    <td align="center"> Crea componentes para crear y editar tareas en el task board</td>
    <td align="center"> 3</td>
    <td align="center"> Paucar Zaenteno Jesus Fernando</td>
    <td align="center">Done</td>
  </tr>
   <tr>
    <td align="center"> TA03 </td>
     <td align="center">Add external service for CRUD operations of tasks</td>
    <td align="center"> Crea un servicio para acceder al fake api y obtener, editar o elimnar datos de las tareas.</td>
    <td align="center"> 2</td>
    <td align="center"> Paucar Zaenteno Jesus Fernando</td>
    <td align="center">Done</td>
  </tr>
  <!----------------------------------------------->
  <tr>
    <td rowspan="1" align="center"> US22 </td>
    <td rowspan="1" align="center"> Visualización de resumen del evento</td>
    <td align="center"> TA01 </td>
    <td align="center"> Create event summary</td>
    <td align="center"> Se debe desarrollar un card que muestre el resumen del evento</td>
    <td align="center"> 2</td>
    <td align="center"> Paico Calderon, July Zelmira </td>
    <td align="center">Done</td>
  </tr>
  <!------------------------------------------------>
   <tr>
    <td rowspan="2" align="center"> US23 </td>
    <td rowspan="2" align="center"> Visualizar perfiles de organizadores	</td>
    <td align="center"> TA01 </td>
    <td align="center"> Organizer profile</td>
    <td align="center"> Se desarrolla secion de perfil del organizador.</td>
    <td align="center"> 3</td>
    <td align="center"> Meza Solórzano Didier Sebastián </td>
    <td align="center"> Done</td>
  </tr>
  <tr>
    <td align="center"> TA02 </td>
     <td align="center">Add Reviews and rating</td>
    <td align="center"> Crea una vista con las reseñas y calificaciones que tiene el organizador.</td>
    <td align="center"> 2</td>
    <td align="center">Meza Solórzano Didier Sebastián</td>
    <td align="center">Done</td>
  </tr>
  <!------------------------------------------------>
   <tr>
    <td rowspan="1" align="center"> US17 </td>
    <td rowspan="1" align="center"> Registro de nuevo evento.</td>
    <td align="center"> TA01 </td>
    <td align="center"> Create a new event</td>
    <td align="center"> Crea un componente que genere un evento cuando se apruebe la cotización.</td>
    <td align="center"> 2 </td>
    <td align="center"> Paico Calderon, July Zelmira </td>
    <td align="center"> Done</td>
  </tr>
</table>

#### 5.2.2.4.Development Evidence for Sprint Review.

<table>
  <tr>
    <td align ="center" > <strong>Repository</strong></td>
    <td  align ="center" > <strong>Branch</strong></td>
    <td  align ="center" > <strong>Commit ID</strong></td>
    <td  align ="center" > <strong>Commit message</strong></td>
    <td  align ="center" > <strong>Commit Message body</strong></td>
    <td  align ="center" > <strong>Commit on (date)</strong></td>
  </tr>

  <tr>
    <td rowspan="6" align="center"> https://github.com/Planificaa/eventgo-frontend.git </td>
    <td align="center"> feature/event-manager</td>
    <td align="center"> e9962e8</td>
    <td align="center"> feat(event-manager): improve filtering, sorting and pagination using primevue.</td>
    <td align="center"> ---</td>
    <td align="center"> 2 hours ago</td>
  </tr>

  <tr>
    <td align="center">feature/task-management</td>
    <td align="center"> 4deb6d6</td>
    <td align="center"> fix(task-management): update task link in app header to correct route.</td>
    <td align="center"> ---</td>
    <td align="center"> 3 hours ago</td>
  </tr>

  <tr>
    <td align="center"> feature/task-management</td>
    <td align="center">1d8bba</td>
    <td align="center"> fix: update task link in AppHeader to correct route.</td>
    <td align="center"> ---</td>
    <td align="center"> 3 hours ago</td>
  </tr>

  <tr>
    <td align="center"> feature/quote-management</td>
    <td align="center"> e5cf384</td>
    <td align="center"> feat(quote-management): update API base URL to production server.</td>
    <td align="center"> ---</td>
    <td align="center">3 hours ago</td>
  </tr>

  <tr>
    <td align="center"> feature/Profile-managment</td>
    <td align="center"> e643aae</td>
    <td align="center"> feat(Profile-managment): add all about profile-management</td>
    <td align="center"> ---</td>
    <td align="center">3 hours ago</td>
  </tr>

  <tr>
    <td align="center"> feature/task-management</td>
    <td align="center"> 7d8cb57</td>
    <td align="center"> Update TaskEditPage.vue</td>
    <td align="center"> ---</td>
    <td align="center">4 hours ago</td>
  </tr>

  <tr>
    <td align="center"> https://github.com/Planificaa/eventgo-frontend.git </td>
    <td align="center"> feature/task-management</td>
    <td align="center"> 3b33b74</td>
    <td align="center"> Update TaskCreatePage.vue</td>
    <td align="center"> ---</td>
    <td align="center"> 4 hours ago</td>
  </tr>

</table>

#### 5.2.2.5.Execution Evidence for Sprint Review.

**Bounded Context Quote Management**

**Quote Management**

Esta es la página donde se gestionan todas las cotizaciones. Se puede crear cotizaciones nuevas, asi como actualizar los datos de cotizaciones anteriormente registradas, si en caso el organizador necesite definir cambios de último momento.

![quote-management.png](../img/Chapter%20V/quote-management.png)

**Quote Order Form Component**

Este es el formulario donde se define información relevante respecto al posible evento que se vaya a realizar. El organizador podrá definir el tipo de evento que se planeará, la cantidad de invitados, asi como la fecha que se celebraria. Además se podrá agregar los servicios que incluirá en la planeación.

![quote-order-create-and-edit.png](../img/Chapter%20V/quote-order-create-and-edit.png)

Una vez definido la información de la cotización, se registrará en el Fake API y se mostrará en la página **Quote Management**
![quote-order-created.png](../img/Chapter%20V/quote-order-created.png)

![quote-list.png](../img/Chapter%20V/quote-list.png)


**Service Item Form Component**

Este es un formulario donde se define la información del servicio a incluir en la cotización, se redacta una breve descripción del servicio, se define la cantidad, el precio unitario y se calcula el precio total. Posteriormente, al crear el servicio, se registra en la tabla de Servicios Incluidos del formulario de cotizaciones
![service-item-create-and-edit.png](../img/Chapter%20V/service-item-create-and-edit.png)

Una vez definido el servicio, se registrará en el Fake API y se mostrará en el formulario de Quote Order
![service-added-quote-order.png](../img/Chapter%20V/service-added-quote-order.png)


**Bounded Context Task Management**

**Task Management**

Esta es la página donde se visualiza el estado actual de la organizacion de las tareas del evento. Se puede crear tareas nuevas y asignarlas a un estado especifico, dependiendo del enfoque del organizador.
Con el objetivo de mantener al anfitrion de eventos siempre al tanto de las tareas que se están realizando, las que faltan por hacer, por revisar y completadas.

![task-management.png](../img/Chapter%20V/task-management.png)

**Edit Task Component**

Este es un componente donde se podra editar una tarea, se podra cambiar el titulo, descripcion y columna a la que pertenece.

![edit-task-management.png](../img/Chapter%20V/edit-task-management.png)

**Event Management**

Este es un componente que permitirá al organizador ver sus eventos creados, así como ver un resumen del evento.

![event-management.png](../img/Chapter%20V/event-management.png)

**Create Event Component**

Este es un componente que permitirá al organizador crear un nuevo evento, definiendo el nombre del evento, la fecha, la ubicación y una breve descripción del evento.

![create-event.png](../img/Chapter%20V/create-event.png)

**Profile Management**

Este es un componente que permitirá al organizador ver su perfil, así como ver las reseñas y calificaciones que tiene el organizador.

![profile-management.png](../img/Chapter%20V/profile-management.png)

**Direct Communication**

Este es un componente que permitirá al organizador ver sus mensajes, así como enviar y recibir mensajes.

![direct-communication.png](../img/Chapter%20V/direct-communication.png)


#### 5.2.2.6.Services Documentation Evidence for Sprint Review.

Para este segundo Sprint, hemos realizado la implementación y el despliegue del FrontEnd de nuestra aplicación Web "EventGo"

<table> 
  <tr>
    <td> <strong>End Point </strong></td>
    <td align="center"> <strong>Funciones</strong> </td>
  </tr>

  <tr>
    <td> https://planificaa.github.io/EventGo-Landing-Pague/ </td>
    <td> Desplegar Landing Page de EventGo</td>
  </tr>
  <tr>
    <td> https://eventgo-e7169.web.app/ </td>
    <td> Desplegar Front End</td>
  </tr>
  <tr>
    <td> https://data-jaon-eventgo.onrender.com/ </td>
    <td> Desplegar Fake API</td>
  </tr>
</table>

#### 5.2.2.7.Software Deployment Evidence for Sprint Review.

Para el despliegue del FrontEnd utilizamos el servicio de hosting que ofrece Firebase. Para ello, hemos utilizado Firebase CLI para vincular nuestro proyecto con Firebase y mediante lineas de comandos realizar el despliegue.

![firebase.jpeg](../img/Chapter%20V/firebase.jpeg) 


#### 5.2.2.8.Team Collaboration Insights during Sprint.

La meta para este Sprint fue la implementación y despliegue de la primera versión del FrontEnd de nuestro proyecto. Para ello, utilizamos diversas herramientas como GitHub, Webstorm, Vue 3, PrimeVue, PrimeFlex, Primeicons, entre otros.
Como evidencia de que se trabajo de forma colaborativa se presentan los insights del repositorio en Github donde se desarrollo el proyecto.

![collaboration-insights.png](../img/Chapter%20V/collaboration-insights.png)

En esta imagen se muestran el total de commits que hizo cada integrante durante el desarrollo del Frontend

![Contributors.png](../img/Chapter%20V/Contributors.png)

En esta imagen se refleja el nivel de modificaciones realizadas por los commits de cada integrante en el repositorio del FrontEnd.

![gitflow-feature-branch.png](../img/Chapter%20V/gitflow-feature-branch.png)

![gitflow-feature-branch-2.png](../img/Chapter%20V/gitflow-feature-branch-2.png)

Finalmente en estas imagenes se pueden apreciar las ramas con las que se ha trabajado durante el desarrollo del FrontEnd

### 5.2.3. Sprint 3

Durante este Sprint se desarrolló la primera versión funcional del **backend de EventGo**, además de aplicar mejoras y ajustes tanto en la landing page como en el frontend. Para ello se definieron tareas orientadas a las funcionalidades esenciales del proyecto, como la gestión de cotizaciones para eventos y la creación de tareas involucradas en su organización.

---

#### 5.2.3.1. Sprint Planning 3

| **Sprint #** | **Sprint 3** |
|-------------|--------------|
| **Sprint Planning Background** | |
| **Date** | 07/11/25 |
| **Time** | 11:40 horas |
| **Location** | Reunión presencial – Aula UPC VH107 |
| **Prepared By** | **Meza Solórzano, Didier Sebastián** |
| **Attendees** | - Paucar, Jesús Fernando <br> - Deybbi Anderson Crisanto Calle <br>  - July Zelmira Paico Calderón |
| **Sprint 2 Review Summary** | Durante el Sprint 2 se logró estructurar y diseñar la landing page y el frontend inicial de EventGo, identificando secciones importantes y los componentes necesarios para ilustrar el comportamiento esperado de la aplicación. Además, se establecieron las tecnologías principales del proyecto: Angular y Angular Material. |
| **Sprint 2 Retrospective Summary** | El equipo destacó la importancia del diseño visual y la consistencia estructural para captar usuarios. Asimismo, se identificó la necesidad de definir estándares y guías de código que faciliten la escalabilidad del desarrollo. |
| **Sprint 3 Goal** | El objetivo de este Sprint es proporcionar información más completa sobre EventGo y el equipo desarrollador, además de optimizar la conversión de visitantes mediante nuevas funcionalidades. Se implementarán características como búsqueda de organizadores, planes de suscripción, mensajería entre anfitriones y organizadores, notificaciones, autenticación y la gestión de eventos, tareas y cotizaciones mediante una API. El Sprint se considerará exitoso cuando los usuarios puedan buscar organizadores, adquirir planes mensuales, comunicarse por chat, recibir notificaciones relevantes y los organizadores puedan administrar eventos, tareas y cotizaciones desde los endpoints desarrollados. |
| **Sprint 3 Velocity** | 26 (Primer Sprint estimado) |
| **Sum of Story Points** | 22 Story Points |

---

#### 5.2.3.2. Aspect Leaders and Collaborators

| **Team Member** | **GitHub Username** | **Task Management** | **Profile Management** | **Quote Management** | **Event Management** | **Review Management** |
|-----------------|---------------------|----------------------|-------------------------|-----------------------|-----------------------|------------------------|
| Paucar, Jesús Fernando | devFernando22 | L | C | C | C | C |
| Crisanto Calle, Deybbi Anderson | Dacc03 | C | L | C | C | C |
| Paico Calderón, July Zelmira | JulyP | C | C | C | L | C |
| Meza Solórzano, Didier Sebastián | Didier04 | C | C | C | C | L |

## 5.2.3.3. Sprint Backlog 3

Para el Sprint 3 se empleó **Trello** como herramienta principal para coordinar, asignar y monitorear las tareas del equipo. Esta organización permitió mantener claridad en el flujo de trabajo y asegurar el cumplimiento de los entregables.

![sprint-backlog-3](https://github.com/Planificaa/EventGo-ProjectDocumentation/blob/develop/img/Chapter%20V/trello3.PNG?raw=true)

**Enlace al tablero:**  
https://trello.com/invite/b/6919724205211f5dbfc0f78a/ATTIbc7f9255d7a4ffa73de15aa0101296923E83C54E/eventgo-sprint-3

---

### **Sprint 3 – User Stories y Tareas**

| User Story | Título                        | Tarea | Título de la Tarea                        | Descripción                                                         | Horas | Asignado a                        | Estado      |
|------------|-------------------------------|--------|--------------------------------------------|---------------------------------------------------------------------|-------|----------------------------------|-------------|
| US26       | Calificar organizador tras evento | TA09  | Crear reseña                               | Registrar una reseña vinculada al perfil y al evento.               | 2     | Meza Solórzano, Didier Sebastián | Done        |
| US26       | Calificar organizador tras evento | TA05  | Implementar reglas de reseñas              | Implementación de reglas de negocio para la generación de reseñas.  | 2     | Meza Solórzano, Didier Sebastián | Done        |
| US18       | Lista de tareas del evento       | TA01  | Cambiar estado de tarea                    | Habilitar la opción de cambiar el estado de las tareas.             | 2     | Paucar, Jesús Fernando           | In Progress |
| US18       | Lista de tareas del evento       | TA14  | Crear lista de tareas                      | Crear la sección de tareas para los organizadores.                  | 2     | Paucar, Jesús Fernando           | In Progress |
| US28       | Filtro de eventos sociales       | TA02  | Implementar filtros                         | Agregar operaciones que permitan filtrar eventos.                   | 3     | Paico Calderón, July Zelmira     | Done        |
| US19       | Gestión del presupuesto          | TA07  | Crear cotización                            | Crear una cotización para el organizador.                           | 2     | Meza Solórzano, Didier Sebastián | Done        |
| US19       | Gestión del presupuesto          | TA06  | Reglas de negocio para cotizaciones         | Implementación de reglas de negocio del módulo de cotizaciones.     | 3     | Meza Solórzano, Didier Sebastián | Done        |
| US29       | Visualización de eventos         | TA11  | Crear/eliminar eventos                      | Implementar operaciones CRUD para gestionar eventos.                | 4     | Paico Calderón, July Zelmira     | Done        |
| US31       | Perfiles de organizadores        | TA08  | Crear perfil                                 | Crear el registro de un perfil de organizador.                      | 2     | Crisanto Calle, Deybbi Anderson  | Done        |
| US31       | Perfiles de organizadores        | TA10  | Reglas de negocio de perfiles                | Implementar reglas de negocio para perfiles.                        | 2     | Crisanto Calle, Deybbi Anderson  | Done        |
| US07       | Confianza y seguridad            | TA03  | Crear sección About Us                      | Desarrollar sección informativa en el landing page.                 | 1     | Meza Solórzano, Didier Sebastián | Done        |
| US07       | Confianza y seguridad            | TA04  | Crear sección del producto                  | Añadir una sección informativa sobre el producto.                   | 1     | Meza Solórzano, Didier Sebastián | In Progress |

---

## **5.2.3.4. Evidencias de Desarrollo – Sprint Review**

A continuación, se incluyen los commits registrados entre el **01 y el 16 de noviembre del 2025** en los repositorios Backend y Frontend del proyecto **EventGo**.

---

## **Repositorio Backend — eventgo-platform-main**

**Repositorio:**  
https://github.com/Planificaa/eventgo-platform-main

| Branch                    | Commit ID  | Mensaje del Commit                                        | Fecha       |
|---------------------------|------------|------------------------------------------------------------|-------------|
| feature/quote-management  | 7a0818d3   | chore: specify type of date columns for service item       | 01/11/2025  |
| feature/profile-management| 6b1d27b0   | feat: add @operation annotations to ProfileController      | 03/11/2025  |
| feature/reviews-management| e0ee6a9f6  | fix: bean creation failure                                 | 06/11/2025  |
| feature/event-management  | c08586c4   | feat(value-object): add StatusType value object            | 10/11/2025  |
| feature/develop           | e0ee6a9f6  | fix: bean creation failure                                 | 16/11/2025  |

---

## **Repositorio Frontend — EventGo-Landing-Pague**

**Repositorio:**  
https://github.com/Planificaa/EventGo-Landing-Pague

| Branch                    | Commit ID  | Mensaje del Commit                                         | Fecha       |
|---------------------------|------------|-------------------------------------------------------------|-------------|
| feature/develop           | 0963aedf   | feat(quote): update quote section                           | 01/11/2025  |
| feature/header            | ccbd9bd8   | feat(header): add call to action for recurrent visitor      | 04/11/2025  |
| feature/header            | 256f0b9f   | feat(header): update spanish content                        | 06/11/2025  |
| feature/about-the-product | 2aaac34b   | feat(about-the-product): update bilingual content           | 08/11/2025  |
| feature/quotes-management | b49a8805   | feat(quote): add organizer id value object                  | 10/11/2025  |
| feature/functionalities   | acf90db9   | chore: update functionalities layout position               | 12/11/2025  |
| feature/plans             | 9771385f   | style: enhance plan section styles                          | 13/11/2025  |
| feature/about-us          | 669bee4d   | style(about-us): improve visuals for about us section       | 15/11/2025  |
| feature/about-the-team    | b6afb677   | feat(about-the-team): add team section in both languages    | 16/11/2025  |
| feature/header            | 34b801d0   | chore: adjust order of language switcher buttons            | 16/11/2025  |

#### 5.2.3.5. Execution Evidence for Sprint Review

Durante el Sprint 3 se completó la ejecución y validación de la segunda versión funcional del front sistema web, junto con la primera implementación operativa del backend de EventGo. A continuación, se adjuntan las capturas correspondientes al funcionamiento en tiempo real.

**Bounded Context Quote Management**

**Quote Management**

Esta es la página donde se gestionan todas las cotizaciones. Se puede crear cotizaciones nuevas, asi como actualizar los datos de cotizaciones anteriormente registradas, si en caso el organizador necesite definir cambios de último momento.

- Vista Anfitrión: 
![quotes-anfitrion.jpeg](../img/Chapter%20V/quotes-anfitrion.jpeg) 

- Vista Organizador:
![quote-org.jpeg](../img/Chapter%20V/quote-org.jpeg)
![quote-orga2.jpeg](../img/Chapter%20V/quote-orga2.jpeg)

**Quote Order Form Component**

Este es el formulario donde se define información relevante respecto al posible evento que se vaya a realizar. El organizador podrá definir el tipo de evento que se planeará, la cantidad de invitados, asi como la fecha que se celebraria. Además se podrá agregar los servicios que incluirá en la planeación.

un formulario donde se define la información del servicio a incluir en la cotización, se redacta una breve descripción del servicio, se define la cantidad, el precio unitario y se calcula el precio total. Posteriormente, al crear el servicio, se registra en la tabla de Servicios Incluidos del formulario de cotizaciones 
![quote-edit.jpeg](../img/Chapter%20V/quote-edit.jpeg)


Una vez definido la información de la cotización, se registrará en el Fake API y se mostrará en la página

**Quote Management**

![img.png](../img/Chapter%20V/img.png)



**Dashboard Anfitrion**
![dashboard-anfi.jpeg](../img/Chapter%20V/dashboard-anfi.jpeg)

**Dashboard Organizador**
![dashboard-orga.jpeg](../img/Chapter%20V/dashboard-orga.jpeg)


**Event Management**

Este es un componente que permitirá al organizador ver sus eventos creados, así como ver un resumen del evento.

![list-social-events.jpeg](../img/Chapter%20V/list-social-events.jpeg)

Así mismo podra ver los eventos que se crean a partir de las cotizaciones aceptadas
![approved-events-from-quotes.jpeg](../img/Chapter%20V/approved-events-from-quotes.jpeg)

**Create Event Component**

Este es un componente que permitirá al organizador crear un nuevo evento, definiendo el nombre del evento, la fecha, la ubicación y una breve descripción del evento.

![create-new-event.jpeg](../img/Chapter%20V/create-new-event.jpeg)

![edit-event.jpeg](../img/Chapter%20V/edit-event.jpeg) 

**Search events**
![searchForTitle.jpeg](../img/Chapter%20V/searchForTitle.jpeg)

![searchForLocation-reves.jpeg](../img/Chapter%20V/searchForLocation-reves.jpeg)

**Profile Management**

Este es un componente que permitirá al organizador ver su perfil, así como ver las reseñas y calificaciones que tiene el organizador.

![perfil-orga.jpeg](../img/Chapter%20V/perfil-orga.jpeg)

**Direct Communication**

Este es un componente que permitirá al organizador ver sus mensajes, así como enviar y recibir mensajes.

![direct-communication.png](../img/Chapter%20V/direct-communication.png)



**Backend – Evidencias de Ejecución**

![execution-backend-1](https://github.com/Planificaa/EventGo-ProjectDocumentation/blob/develop/img/Chapter%20V/swa1.jpg?raw=true)

![execution-backend-2](https://github.com/Planificaa/EventGo-ProjectDocumentation/blob/develop/img/Chapter%20V/swa2.jpg?raw=true)

![execution-backend-3](https://github.com/Planificaa/EventGo-ProjectDocumentation/blob/develop/img/Chapter%20V/swa3.jpg?raw=true)

![execution-backend-4](https://github.com/Planificaa/EventGo-ProjectDocumentation/blob/develop/img/Chapter%20V/swa4.jpg?raw=true)

![execution-backend-5](https://github.com/Planificaa/EventGo-ProjectDocumentation/blob/develop/img/Chapter%20V/swa5.jpg?raw=true)


---

#### 5.2.3.6. Services Documentation Evidence for Sprint Review

Según la documentación mostrada en Swagger durante el Sprint 3, estos son los endpoints habilitados para la gestión de cotizaciones y servicios:

| **Método HTTP** | **Endpoint** | **Descripción** |
|---|---|---|
| GET | `/api/v1/organizers/{organizerId}/quotes` | Recupera todas las cotizaciones de un organizador. |
| GET | `/api/v1/quotes/{quoteId}` | Obtiene los datos de una cotización específica. |
| PUT | `/api/v1/quotes/{quoteId}` | Actualiza una cotización por su ID. |
| DELETE | `/api/v1/quotes/{quoteId}` | Elimina una cotización. |
| POST | `/api/v1/quotes` | Crea una nueva cotización. |
| POST | `/api/v1/quotes/{quoteId}/confirmations` | Marca una cotización como “Aceptada” (Accepted). |
| POST | `/api/v1/quotes/{quoteId}/rejections` | Marca una cotización como “Rechazada” (Rejected). |
| GET | `/api/v1/quotes/{quoteId}/service-items/{serviceItemId}` | Obtiene un ítem de servicio de una cotización. |
| PUT | `/api/v1/quotes/{quoteId}/service-items/{serviceItemId}` | Actualiza un ítem de servicio existente. |
| DELETE | `/api/v1/quotes/{quoteId}/service-items/{serviceItemId}` | Borra un ítem de servicio. |
| POST | `/api/v1/quotes/{quoteId}/service-items` | Añade un nuevo servicio a una cotización. |
| GET | `/api/v1/quotes/{quoteId}/service-items` | Lista todos los ítems de servicio de esa cotización. |



#### 5.2.3.7. Software Deployment Evidence for Sprint Review

En este sprint, se completó el despliegue operativo del backend de EventGo en la plataforma Render, asegurando disponibilidad y acceso constante para pruebas del equipo.

**Backend – Evidencia de Despliegue**

![render-deploy](https://github.com/Planificaa/EventGo-ProjectDocumentation/blob/develop/img/Chapter%20V/we2.PNG?raw=true)


#### 5.2.3.8.Team Collaboration Insights during Sprint.

Esta sección demuestra la colaboración del equipo en la entrega del sprint actual, incluyendo las métricas de creación del backend.

### Backend

**Pulse**

![pulse-insights](https://github.com/Planificaa/EventGo-ProjectDocumentation/blob/develop/img/Chapter%20V/colab.PNG?raw=true)

**Network**

![network-insights](https://github.com/Planificaa/EventGo-ProjectDocumentation/blob/develop/img/Chapter%20V/colab2.PNG?raw=true)

### 5.2.4. Sprint 4

Durante el este Sprint nuestro enfoque es desarrollar la versión final de los tres productos de nuestro proyecto: la landing page, el FrontEnd y el BackEnd. Para lograrlo, definimos en el sprint backlog diversas tareas relacionadas con las funcionalidades principales del negocio, como las cotizaciones para eventos y la creación de tareas que se llevarán a cabo durante su planificación. Además, se implementarán mejoras en la experiencia del usuario y se realizarán pruebas exhaustivas para garantizar un producto de alta calidad.

#### 5.2.4.1. Sprint Planning 4.

| Sprint # | Sprint 4 |
|:------------------------------:|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------:|
| **Sprint Planning Background** |  |
| **Date** | 01/12/2025 |
| **Time** | 11:40 horas |
| **Location** | Reunión presencial - Aula UPC VH107 |
| **Prepared By** | Didier Sebastian Meza Solòrzano |
| **Attendees** | - Didier Sebastian Meza Solòrzano  <br> - Deybbi Anderson Crisanto Calle  <br> - Jesús Fernando Paucar Zenteno  <br> - July Zelmira Paico Calderon |
| **Sprint 3 Review Summary** | Se completó la documentación y el diseño de la estructura de la Landing Page y el Frontend de la aplicación web, definiendo las secciones principales e identificando los componentes esenciales para mostrar el funcionamiento de la plataforma. Además, se determinaron las tecnologías fundamentales para el proyecto: Vue en el frontend, y C# en el backend, lo que garantiza una arquitectura robusta y escalable para la gestión de la aplicación. |
| **Sprint 3 Retrospective Summary** | En el Sprint 3, se completó la integración inicial entre el frontend y backend, permitiendo el funcionamiento básico de características como generación de cotizaciones. También se hizo hincapié en la importancia de seguir con los estándares de código para garantizar la escalabilidad del proyecto. |
| **Sprint Goal & User Stories** |  |
| **Sprint 4 Goal** | En este último sprint, nuestro enfoque es finalizar e integrar todos los componentes clave de la aplicación. Esto incluye presentar información clara sobre el proyecto y el equipo detrás del desarrollo, y optimizar el sitio web para convertir a los visitantes en usuarios activos. Se implementarán funcionalidades esenciales como la búsqueda de organizadores de eventos, suscripciones mensuales, notificaciones personalizadas, autenticación de usuarios y una API robusta para gestionar eventos, tareas y cotizaciones. Estas características están diseñadas para ofrecer una experiencia completa y escalable, pensada para atraer y retener distintos tipos de usuarios, ya sean recurrentes, racionales o emocionales. El éxito de este sprint se validará cuando los usuarios puedan interactuar plenamente con el sistema: desde buscar organizadores y suscribirse a un plan, hasta recibir alertas y que los organizadores puedan administrar eficientemente sus actividades mediante la API implementada. |
| **Sprint 4 Velocity** | Velocidad de 20 - Cuarto Sprint |
| **Sum of Story Points** | Sprint 4 - 22 Story Points |

#### 5.2.4.2. Aspect Leaders and Collaborators.

|             Team Member                    |  GitHub Username  | ReviewManagement | ProfileManagement | QuoteManagement | Event Management | Subscription Management |
|:------------------------------------------:|:-----------------:|:----------------:|:-----------------:|:---------------:|:----------------:|:-----------------------:|
|   Crisanto Calle, Deybbi Anderson          |       Dacc03      |        L         |         L         |        C        |        C         |            C            |
|  Jesús Fernando Paucar Zenteno             |   devFernando22   |        L         |         C         |        L        |        C         |            C            |
|    Paico Calderon, July Zelmira            |       JulyP       |        C         |         C         |        C        |        L         |            C            |
|  Didier Sebastian Meza Solòrzano           |    DidierMeza     |        C         |         C         |        C        |        C         |            L            |

#### 5.2.4.3. Sprint Backlog 4.

Para el sprint 4 usamos la herramienta Trello para organizar las tareas del equipo.

![sprint-backlog 4](https://github.com/Planificaa/EventGo-ProjectDocumentation/blob/develop/img/Chapter%20V/Trello4.PNG?raw=true)

Enlace: https://trello.com/b/W2ZdKqqU/eventgo-sprint-backlog-4

<table>
  <tr>
    <td><strong>Sprint #</strong></td>
    <td align="center" colspan="7"><strong>Sprint 4</strong></td>
  </tr>

  <tr>
    <td align="center" colspan="2"><strong>User Story</strong></td>
    <td align="center" colspan="6"><strong>Work-item/Task</strong></td>
  </tr>

  <tr>
    <td align="center"><strong>ID</strong></td>
    <td align="center"><strong>Title</strong></td>
    <td align="center"><strong>ID</strong></td>
    <td align="center"><strong>Title</strong></td>
    <td align="center"><strong>Description</strong></td>
    <td align="center"><strong>Estimation (Hours)</strong></td>
    <td align="center"><strong>Assigned To</strong></td>
    <td align="center"><strong>Status</strong></td>
  </tr>

  <tr>
    <td align="center">US01</td>
    <td align="center">Navegación sencilla</td>
    <td align="center">TA01</td>
    <td align="center">Implementar el lenguaje por defecto</td>
    <td align="center">Quiero que el landing page esté en inglés por defecto</td>
    <td align="center">2</td>
    <td align="center">Crisanto Calle, Deybbi Anderson</td>
    <td align="center">Done</td>
  </tr>

  <tr>
    <td align="center">US05</td>
    <td align="center">Llamada a la acción</td>
    <td align="center">TA02</td>
    <td align="center">Create call to action</td>
    <td align="center">Quiero que el landing page tenga las llamadas a la acción para los tres tipos de visitantes</td>
    <td align="center">2</td>
    <td align="center">Jesús Fernando Paucar Zenteno</td>
    <td align="center">Done</td>
  </tr>

  <tr>
    <td align="center">US06</td>
    <td align="center">Visualización de tutorial de la aplicación</td>
    <td align="center">TA03</td>
    <td align="center">Add about the product video</td>
    <td align="center">Quiero insertar un video sobre el producto en nuestra web de negocio.</td>
    <td align="center">1</td>
    <td align="center">Jesús Fernando Paucar Zenteno</td>
    <td align="center">Done</td>
  </tr>

  <tr>
    <td align="center">US10</td>
    <td align="center">Diseño responsive</td>
    <td align="center">TA04</td>
    <td align="center">Configure correct loading</td>
    <td align="center">Quiero que el sitio web de negocio se cargue correctamente.</td>
    <td align="center">1</td>
    <td align="center">Crisanto Calle, Deybbi Anderson</td>
    <td align="center">Done</td>
  </tr>

  <tr>
    <td rowspan="2" align="center">US19</td>
    <td rowspan="2" align="center">Gestión de presupuesto del evento</td>
    <td align="center">TA05</td>
    <td align="center">Create an update operation for quote</td>
    <td align="center">Quiero crear una operación para actualizar cotizaciones.</td>
    <td align="center">2</td>
    <td align="center">Jesús Fernando Paucar Zenteno</td>
    <td align="center">Done</td>
  </tr>
  <tr>
    <td align="center">TA06</td>
    <td align="center">Create service item for quote management</td>
    <td align="center">Quiero crear un service item para el manejo de las cotizaciones.</td>
    <td align="center">4</td>
    <td align="center">Jesús Fernando Paucar Zenteno</td>
    <td align="center">Done</td>
  </tr>

  <tr>
    <td align="center">US21</td>
    <td align="center">Vista de cronograma del evento</td>
    <td align="center">TA08</td>
    <td align="center">Update scheduler for events</td>
    <td align="center">Quiero actualizar el calendario de los eventos.</td>
    <td align="center">2</td>
    <td align="center">Crisanto Calle, Deybbi Anderson</td>
    <td align="center">Done</td>
  </tr>

  <tr>
    <td align="center">US27</td>
    <td align="center">Editar reseña publicada</td>
    <td align="center">TA07</td>
    <td align="center">Add update operation for reviews</td>
    <td align="center">Quiero implementar una operación para actualizar las reseñas publicadas.</td>
    <td align="center">2</td>
    <td align="center">Crisanto Calle, Deybbi Anderson</td>
    <td align="center">Done</td>
  </tr>

  <tr>
    <td align="center">US29</td>
    <td align="center">Visualización de los eventos</td>
    <td align="center">TA09</td>
    <td align="center">Add update operation for social events</td>
    <td align="center">Quiero implementar una operación para actualizar los registros de eventos sociales.</td>
    <td align="center">2</td>
    <td align="center">Paico Calderon, July Zelmira</td>
    <td align="center">In Progress</td>
  </tr>

  <tr>
    <td align="center">US28</td>
    <td align="center">Filtro de evento social</td>
    <td align="center">TA10</td>
    <td align="center">Add queries for more event filters</td>
    <td align="center">Quiero implementar más opciones de filtros para los eventos.</td>
    <td align="center">1</td>
    <td align="center">Paico Calderon, July Zelmira</td>
    <td align="center">In Progress</td>
  </tr>

  <tr>
    <td rowspan="3" align="center">US31</td>
    <td rowspan="3" align="center">Visualizar perfiles de organizadores</td>
    <td align="center">TA11</td>
    <td align="center">Create update operation for profile</td>
    <td align="center">Quiero implementar una operación para actualizar los perfiles.</td>
    <td align="center">2</td>
    <td align="center">Crisanto Calle, Deybbi Anderson</td>
    <td align="center">Done</td>
  </tr>
  <tr>
    <td align="center">TA12</td>
    <td align="center">Create a service catalog for profiles</td>
    <td align="center">Quiero crear un catálogo para los perfiles.</td>
    <td align="center">2</td>
    <td align="center">Crisanto Calle, Deybbi Anderson</td>
    <td align="center">Done</td>
  </tr>
  <tr>
    <td align="center">TA13</td>
    <td align="center">Create album for profile</td>
    <td align="center">Quiero crear un álbum para los perfiles.</td>
    <td align="center">2</td>
    <td align="center">Crisanto Calle, Deybbi Anderson</td>
    <td align="center">Done</td>
  </tr>

  <tr>
    <td rowspan="2"></td>
    <td rowspan="2"></td>
    <td align="center">TA14</td>
    <td align="center">Deploy products</td>
    <td align="center">Quiero desplegar mis productos a un dominio público.</td>
    <td align="center">2</td>
    <td align="center">Jesús Fernando Paucar Zenteno</td>
    <td align="center">Done</td>
  </tr>
  <tr>
    <td align="center">TA15</td>
    <td align="center">Implement security</td>
    <td align="center">Quiero agregar autenticación para la plataforma web.</td>
    <td align="center">3</td>
    <td align="center">Didier Sebastian Meza Solòrzano</td>
    <td align="center">In Progress</td>
  </tr>
</table>

#### 5.2.4.4. Development Evidence for Sprint Review.

A continuación, se mostrarán los commits últimos registrados en el repositorio correspondiente al backend para el desarrollo del sprint 4.

<table>
  <tr>
    <td align ="center"><strong>Repository</strong></td>
    <td align ="center"><strong>Branch</strong></td>
    <td align ="center"><strong>Commit ID</strong></td>
    <td align ="center"><strong>Commit message</strong></td>
    <td align ="center"><strong>Commit Message body</strong></td>
    <td align ="center"><strong>Commit on (date)</strong></td>
  </tr>

  <tr>
    <td rowspan="27" align="center"> https://github.com/Planificaa/eventgo-platform-main.git </td>
    <td align="center">feature/quote-management</td>
    <td align="center">e851915f3f54ed55c7cdb521fd3eaf268ce1f0d7</td>
    <td align="center">feat(planning): add acl planning external profile service</td>
    <td align="center">---</td>
    <td align="center">03/12/2025</td>
  </tr>

  <tr>
    <td align="center">feature/profile-management</td>
    <td align="center">c699202593a4593bb96af9d787690243d76da12f</td>
    <td align="center">fix(pom): correct spelling of 'platform' in artifactId and name.</td>
    <td align="center">---</td>
    <td align="center">29/11/2025</td>
  </tr>

  <tr>
    <td align="center">feature/reviews-management</td>
    <td align="center">e0ee6a9f679a46df2f638830f10a0de953170703</td>
    <td align="center">fix: bean creation failure.</td>
    <td align="center">---</td>
    <td align="center">28/11/2025</td>
  </tr>

  <tr>
    <td align="center">feature/event-management</td>
    <td align="center">d3212ba217da342b3b4d99e6ad1c9e3291e80ad8</td>
    <td align="center">feat(planning): add documentation for planning bounded context and social event management.</td>
    <td align="center">---</td>
    <td align="center">03/12/2025</td>
  </tr>

  <tr>
    <td align="center">feature/develop</td>
    <td align="center">4166cc97eec4857b4008e1773bb55dd5cbcb7ae5</td>
    <td align="center">feat(iam): check properties.</td>
    <td align="center">---</td>
    <td align="center">03/12/2025</td>
  </tr>

  <tr>
    <td align="center">feature/iam</td>
    <td align="center">d78e4e4d873057d88c8000bc2b7a0c2ffdc12385</td>
    <td align="center">feat(iam): update application-prod.properties</td>
    <td align="center">---</td>
    <td align="center">03/12/2025</td>
  </tr>
</table>

<br>

<table>
  <tr>
    <td align ="center"><strong>Repository</strong></td>
    <td align ="center"><strong>Branch</strong></td>
    <td align ="center"><strong>Commit ID</strong></td>
    <td align ="center"><strong>Commit message</strong></td>
    <td align ="center"><strong>Commit Message body</strong></td>
    <td align ="center"><strong>Commit on (date)</strong></td>
  </tr>

  <tr>
    <td rowspan="27" align="center"> https://github.com/Planificaa/eventgo-frontend.git </td>
    <td align="center">feature/develop</td>
    <td align="center">051b1907d086f53f1e745007186623da9bc1ab61</td>
    <td align="center">Merge branch 'feature/event-management' into develop</td>
    <td align="center">---</td>
    <td align="center">03/12/2025</td>
  </tr>

  <tr>
    <td align="center">feature/event-management</td>
    <td align="center">35a6eac8dad523388984eadc38fd2bb03eb7a521</td>
    <td align="center">refactor(calendar): refactor calendar view path and integrate FullCalendar.</td>
    <td align="center">---</td>
    <td align="center">03/12/2025</td>
  </tr>

  <tr>
    <td align="center">feature/iam</td>
    <td align="center">3d8198364a60a020a3f2f35af491242b26a0c4a5</td>
    <td align="center">feat(iam): add authentication section in navigation bar component</td>
    <td align="center">---</td>
    <td align="center">03/12/2025</td>
  </tr>

  <tr>
    <td align="center">feature/profile-management</td>
    <td align="center">916bc3e3171e128c64c16edd415086d6629c5555</td>
    <td align="center">feat(base-service): add unit tests for BaseService with TestService implementation.</td>
    <td align="center">---</td>
    <td align="center">28/11/2025</td>
  </tr>

  <tr>
    <td align="center">feature/quotes-management</td>
    <td align="center">62258159bd17a3ab0aca2b30e651cad5cd511247</td>
    <td align="center">feat(service-item): add update service item functionality</td>
    <td align="center">---</td>
    <td align="center">03/12/2025</td>
  </tr>
</table>

<br>

<table>
  <tr>
    <td align ="center"><strong>Repository</strong></td>
    <td align ="center"><strong>Branch</strong></td>
    <td align ="center"><strong>Commit ID</strong></td>
    <td align ="center"><strong>Commit message</strong></td>
    <td align ="center"><strong>Commit Message body</strong></td>
    <td align ="center"><strong>Commit on (date)</strong></td>
  </tr>

  <tr>
    <td rowspan="27" align="center"> https://github.com/Planificaa/EventGo-Landing-Pague.git </td>
    <td align="center">develop</td>
    <td align="center">d655cbc4b5c8a03a035c167cc050d7c915c6634a</td>
    <td align="center">refactor(paths): refactor assets paths in html.</td>
    <td align="center">---</td>
    <td align="center">02/12/2025</td>
  </tr>

  <tr>
    <td rowspan="27" align="center"> https://github.com/Planificaa/EventGo-Landing-Pague.git </td>
    <td align="center">main</td>
    <td align="center">a27215605323f59a313455f164e3aa2bb2af7f8c</td>
    <td align="center">refactor(assets): refactor developers profiles.</td>
    <td align="center">---</td>
    <td align="center">02/12/2025</td>
  </tr>
</table>

#### 5.2.4.5. Execution Evidence for Sprint Review.
#### 5.2.4.6. Services Documentation Evidence for Sprint Review.
#### 5.2.4.7. Software Deployment Evidence for Sprint Review.
#### 5.2.4.8. Team Collaboration Insights during Sprint.

## 5.3. Validation Interviews.
### 5.3.1. Diseño de Entrevistas.

A continuación se presentan las preguntas de validación utilizadas para las entrevistas con usuarios. El objetivo es evaluar tanto la landing page como la aplicación web de EventGo para asegurar que la experiencia de navegación sea clara, coherente y útil para quienes organizan y gestionan eventos.


#### Preguntas sobre la Landing Page

- ¿Al ingresar a la landing page, entiendes rápidamente qué es Eventify y a quién está dirigido?
- ¿La información sobre las funcionalidades de la plataforma te resulta clara y atractiva?
- ¿El diseño visual (colores, imágenes, tipografías) te transmite confianza y profesionalismo?
- ¿Consideras que la estructura de la landing page está bien organizada y fácil de navegar?
- ¿Te motivaría registrarte o saber más sobre Eventify luego de explorar la landing page?
- ¿Hay algo que te gustaría ver en la landing que actualmente no está presente?

#### Preguntas sobre la Aplicación Web

- ¿Nota coherencia visual y funcional entre las distintas secciones (perfil, eventos, cotizaciones, etc.)?
- ¿El proceso de creación o edición de sus albums incluidos en su perfil es claro y sencillo?
- ¿Le resulta fácil acceder y gestionar las cotizaciones dentro de la plataforma?
- ¿Cómo evalúa la sección de eventos? ¿Le permite organizar y visualizar la información de manera efectiva?
- ¿La vista de calendario cubre sus expectativas para programar y revisar actividades importantes?
- ¿El tablero estilo Kanban para tareas le ayuda a organizar su flujo de trabajo? ¿Es intuitivo?
- ¿Le resulta fácil identificar el estado de cada tarea (pendiente, en progreso, finalizada)?
- ¿Hay algo que le haya confundido o que no funcionó como esperabas?
- ¿Qué mejoraría de la experiencia general al usar la aplicación web?



### 5.3.2. Registro de Entrevistas.
### 5.3.3. Evaluaciones según heurísticas.
## 5.4. Video About-the-Product

En esta sección, se adjunta el enlace al video sobre el producto de software desarrollado. En este video, se detallan funcionalidades principales y beneficios que ofrece la aplicacion a los usuarios finales que usaran la aplicacion web para sus negocios.

Enlace al video acerca del producto: [https://tinyurl.com/4xu4a6pe ](https://upcedupe-my.sharepoint.com/:v:/g/personal/u202319950_upc_edu_pe/IQAYE9dgCDEfTo2EZ5doFo7JATdk_jqCHxUjSRLAz3ucFnQ?e=08tl8w&nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifX0%3D)
<p align="center">
  <img src="https://github.com/Planificaa/EventGo-ProjectDocumentation/blob/main/img/Chapter%20V/Captura.PNG?raw=true">
</p>
