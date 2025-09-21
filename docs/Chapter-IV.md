# Capítulo 4: Product Design #

## _4.1. Style Guidelines_ ##

### 4.1.1. General Style Guidelines ###



### 4.1.2. Web Style Guidelines ###



## _4.2. Information Architecture_ ##

### 4.2.1. Organization Systems ###



### 4.2.2. Labeling Systems ###



### 4.2.3. SEO Tags and Meta Tags ###



### 4.2.4. Searching Systems ###



### 4.2.5. Navigation Systems ###



## _4.3. Landing Page UI Design_ ##

### 4.3.1. Landing Page Wireframe ###


### 4.3.2. Landing Page Mock-up ###

## _4.4. Web Applications UX/UI Design_ ##

### 4.4.1. Web Applications Wireframes ###


### 4.4.2. Web Applications Wireflow Diagrams ###


### 4.4.3. Web Applications Mock-ups ###


## _4.5. Web Applications Prototyping_ ##



## _4.6. Domain-Driven Software Architecture_ ##
Se trata de una metodología que estructura el software a partir de los dominios de negocio, lo que facilita la comprensión y el manejo de la complejidad del sistema. A continuación, se presentan los diagramas que ilustran la arquitectura del software. En **EventGo** expone el proceso seguido por el equipo para refinar y mejorar el modelado general del dominio del problema.

![WineInvetoryDomain-Driven](../img/Chapter%20IV/step-1.png)

![WineInvetory Domain-Driven](../img/Chapter%20IV/step-2.png)

![WineInvetory Domain-Driven](../img/Chapter%20IV/step-3.png)

![WineInvetory Domain-Driven](../img/Chapter%20IV/step-4.png)

![WineInvetory Domain-Driven](../img/Chapter%20IV/step-5.png)

![WineInvetory Domain-Driven](../img/Chapter%20IV/step-6.png)

![WineInvetory Domain-Driven](../img/Chapter%20IV/step-7.png)

![WineInvetory Domain-Driven](../img/Chapter%20IV/step-8.png)

![WineInvetory Domain-Driven](../img/Chapter%20IV/step-9.png)
### 4.6.1. Design-Level Event Storming ###

El objetivo es alcanzar un mayor nivel de detalle en la comprensión del sistema, a través de una sesión estructurada y concentrada en identificar los elementos clave.

### 4.6.2. Software Architecture Context Diagram ###
En esta sección se muestra una visión general del sistema en su entorno, identificando los actores externos, sistemas relacionados y las principales interacciones que definen sus límites funcionales.

![SystemContext.png](../img/Chapter%20IV/SystemContext.png)

### 4.6.3. Software Architecture Container Diagrams ###
En esta sección se descompone el sistema en sus contenedores principales, ilustrando las tecnologías utilizadas, las responsabilidades de cada uno y cómo se comunican entre sí.

![ContainerView.png](../img/Chapter%20IV/ContainerView.png)

### 4.6.4. Software Architecture Components Diagrams ###
En esta sección se detallan los componentes internos de la Single Page Application (SPA), asi como del API Application, los cuales estan divididos en diferentes bounded contexts que encapsulan funcionalidades específicas del dominio. Cada bounded context agrupa componentes que colaboran entre sí para cumplir con responsabilidades concretas, lo que facilita la escalabilidad, el mantenimiento y la alineación con los procesos del negocio.

**Single Page Application (SPA)**

**Event Design and Planning Bounded Context**

![SPA-Event-Design-and-Planning-Bounded-Context-ComponentView.png](../img/Chapter%20IV/SPA-Event-Design-and-Planning-Bounded-Context-ComponentView.png)

**Event Operations and Monitoring Bounded Context**

![EventOperationsMonitoringComponentView.png](../img/Chapter%20IV/EventOperationsMonitoringComponentView.png)

**Profiles and Preferences Bounded Context**

![ProfilesPreferencesComponentView.png](../img/Chapter%20IV/ProfilesPreferencesComponentView.png)

**Payments and Subscriptions Bounded Context**

![PaymentsSubscriptionsComponentView.png](../img/Chapter%20IV/PaymentsSubscriptionsComponentView.png)

**Direct Communication Bounded Context**

![DirectCommunicationComponentView.png](../img/Chapter%20IV/DirectCommunicationComponentView.png)

**Identity and Access Management Bounded Context (IAM)**

![IAMComponentView.png](../img/Chapter%20IV/IAMComponentView.png)

**API Application - EventGO Platform**

![EventGOPlatformAPIComponentView.png](../img/Chapter%20IV/EventGOPlatformAPIComponentView.png)

## _4.7. Software Object-Oriented Design_ ##



### 4.7.1. Class Diagram ###



## _4.8. Database Design_ ##

### 4.8.1. Database Diagram ###
