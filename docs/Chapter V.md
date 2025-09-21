# Capítulo 5: Product Implementation, Validation & Deployment #

## _5.1. Software Configuration Management_ ##



### 5.1.1. Software Development Environment Configuration ###



### 5.1.2. Source Code Management ###


### 5.1.3. Source Code Style Guide & Conventions ###



### 5.1.4. Software Deployment Configuration ###



## _5.2. Landing Page, Services & Applications Implementation_ ##

### 5.2.1. Sprint 1 ###

En el Sprint 1, se enfocó el trabajo en diseñar y desarrollar la Landing Page de EventGo, con el objetivo de presentar de forma clara y atractiva los beneficios de la plataforma para organizadores y anfitriones de eventos. Durante este sprint, se trabajó en una estructura de navegación intuitiva y una disposición visual que permitiera destacar las características principales del servicio. Se organizó el equipo para distribuir las tareas y lograr un diseño completamente responsivo, asegurando que la página se visualice correctamente en distintos tamaños de pantalla.

#### 5.2.1.1. Sprint Planning 1 ####

|             Sprint #             |                                                                                                                                                                                                                                                                                                                                                                                                                                                          Sprint 1                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
|:--------------------------------:|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------:|
|  **Sprint Planning Background**  |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
|               Date               |                                                                                                                                                                                                                                                                                                                                                                                                                                                          07/09/25                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
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

#### 5.2.1.6. Software Deployment Evidence for Sprint Review ####

En el primer sprint, hemos realizado el diseño, la programación y el despligue de la Landing Page que presentará nuesta apliación web "EventiGo". A continuación, se detalla la evidencia del despliegue de la Landing Page:

<table> 
  <tr>
    <td> <strong>End Point </strong></td>
    <td align="center"> <strong>Funciones</strong> </td>
  </tr>

  <tr>
    <td> https://planificaa.github.io/EventGo-Landing-Pague </td>
    <td> Desplegar Landing Page de EventiGo</td>
  </tr>
</table>

#### 5.2.1.7. Software Deployment Evidence for Sprint Review ####

#### 5.2.1.8. Team Collaboration Insights during Sprint ####
