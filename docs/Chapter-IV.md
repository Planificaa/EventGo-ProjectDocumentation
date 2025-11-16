# Capítulo 4: Product Design #

## _4.1. Style Guidelines_ ##
En esta sección, se expone nuestra proposición de diseño para el landing page y la aplicación web. Las directrices de estilo de EventGO establecen las pautas visuales y de comunicación, garantizando una experiencia de usuario coherente, intuitiva y accesible. Su propósito es asegurar la consistencia en todos los puntos de interacción, desde la interfaz hasta las notificaciones y mensajes del sistema.
### 4.1.1. General Style Guidelines ###
Esta sección presenta las decisiones visuales y comunicativas que definen la identidad de EvenGo. Se explican aspectos clave como el uso del logo, la tipografía elegida, la paleta de colores, el sistema de espaciado y el tono de comunicación aplicado.

Brand Overview

La identidad visual de EvenGo transmite claridad, organización y confianza desde el primer vistazo. El logo está compuesto por un ícono de calendario con un check en el centro, que representa la idea de tener un evento agendado y confirmado con éxito. A la derecha del ícono aparece el nombre de la marca en PascalCase con el acrónimo en mayúscula de GO: **EvenGO**.

El color principal del logo es un tono verde claro y vibrante que destaca sobre distintos fondos, y que transmite frescura, dinamismo

![EventGo-logo.png](../img/Chapter%20IV/EventGo-logo.png)

**Typography**

La tipografía principal de EvenGo es Poppins, una fuente sans-serif moderna y amigable que aporta claridad, equilibrio visual y un toque contemporáneo a la experiencia del usuario.

Elegida por su legibilidad y estética geométrica, Poppins permite mantener un diseño limpio, funcional y coherente en todos los tamaños de pantalla.

![Typography.png](../img/Chapter%20IV/Typography.png)

Colors

La paleta de colores de EvenGo combina profesionalismo, frescura y dinamismo, reforzando el enfoque moderno y accesible de la plataforma.

![Colors.png](../img/Chapter%20IV/Colors.png)

* **Azul oscuro (#1C2541) / Azul medio (#3A506B)**: <br><br> Aplicados en la barra de navegación, el footer y fondos de secciones principales. Estos tonos transmiten confianza, estabilidad y orden, características clave para una plataforma de organización de eventos.
* **Blanco (#FFFFFF)**: <br><br> Utilizado como fondo neutro para alternar secciones, aporta limpieza visual y mejora la legibilidad de los contenidos.
* **Turquesa claro (#6FFFE9) y verde azulado (#5BC0BE)**: <br><br> Funcionan como colores de acento e interacción. Se emplean en los títulos de sección y al hacer hover sobre botones.
<br>

**Spacing**

La relación de espaciado utilizada, tanto en la aplicación como en la landing page, se basa en un múltiplo de 8 píxeles. Este sistema permite mantener una estructura visual ordenada y coherente en todo el diseño.

![spacing.png](../img/Chapter%20IV/spacing.png)
<br>

**Comunication Tone**

La comunicación está diseñada para ser cercana, clara y con un toque entusiasta, buscando conectar emocionalmente tanto con anfitriones como con organizadores de eventos, sin perder profesionalismo. Se adopta un lenguaje que guía, motiva y transmite confianza,
<br>

### 4.1.2. Web Style Guidelines ###
La interfaz web de EvenGo está diseñada bajo principios de diseño responsive, garantizando una experiencia de usuario óptima en todos los dispositivos, desde smartphones hasta pantallas de escritorio. El objetivo es ofrecer una navegación fluida, intuitiva y visualmente coherente.

Para organizar el contenido se utilizó el patrón en Z, un esquema visual que guía naturalmente la mirada del usuario desde la parte superior izquierda hasta la inferior derecha, ideal para estructurar información de forma clara y persuasiva.

![web-style-z-pattern](/img/Chapter%20IV/web-style-z-pattern.png)


## 4.2. Information Architecture

#### Sistemas de Etiquetado en EventGO

En esta sección se describen los sistemas de etiquetado utilizados en la **Landing Page** y la **Aplicación Web** de **EventGO**.  
El etiquetado está diseñado para facilitar la navegación y mejorar la experiencia del usuario, asegurando que cada sección y funcionalidad sea fácilmente reconocible y accesible.


#### Etiquetas de Encabezados (Headings)

Las etiquetas de encabezado en **EventGO** se utilizan para definir claramente las secciones principales de la página y la aplicación.  
Esto permite a los usuarios identificar rápidamente el contenido de cada sección:

- **Inicio / Home:**  
  Este encabezado se utiliza en la página principal para dar la bienvenida a los usuarios y proporcionar una introducción general a la plataforma.  
  Incluye un banner con la propuesta de valor de EventGO y botones de acceso rápido para registro de organizadores e inscripción de asistentes.

- **Eventos / Events:**  
  Sección que describe los eventos disponibles, sus categorías (conciertos, conferencias, talleres, ferias, etc.), y permite a los usuarios explorar y registrarse.

- **Planes y Precios / Pricing Plans:**  
  Encabezado que detalla las opciones de suscripción para organizadores de eventos, incluyendo características y beneficios de cada plan.

- **Contáctanos / Contact Us:**  
  Proporciona información de contacto, formulario de consulta, y enlaces para asistencia personalizada a organizadores y asistentes.

- **Sobre Nosotros / About Us:**  
  Ofrece información sobre la misión de EventGO, su visión de conectar experiencias, y el equipo detrás de la plataforma.


#### Etiquetas Textuales (Text Labels)

Las etiquetas textuales son utilizadas para identificar categorías específicas o acciones dentro de la plataforma.  
Estas etiquetas ayudan a los usuarios a navegar de manera efectiva y realizar acciones específicas:

- **Buscar Eventos / Find Events:**  
  Utilizada en la barra de búsqueda, permite a los usuarios explorar eventos disponibles según ubicación, fecha o categoría.

- **Registrarse / Register:**  
  Botón que permite a los usuarios inscribirse como asistentes o creadores de eventos.

- **Mis Eventos / My Events:**  
  Sección donde los usuarios pueden gestionar los eventos a los que están inscritos o que están organizando.

- **Historial / History:**  
  Permite a los usuarios revisar los eventos pasados a los que asistieron o que organizaron.

- **Configuraciones / Settings:**  
  Permite acceder a las preferencias de cuenta, métodos de pago, notificaciones y ajustes generales.


#### Etiquetas Icónicas (Iconic Labels)

Las etiquetas icónicas se basan en imágenes o iconos que transmiten significado visualmente.  
Estas etiquetas son intuitivas y ayudan a los usuarios a comprender rápidamente las funcionalidades sin necesidad de texto:

- **Icono de Búsqueda (Lupa):**  
  Representa la función de buscar eventos dentro de la plataforma.

- **Icono de Calendario:**  
  Utilizado para mostrar fechas relevantes de los eventos y gestionar la programación personal.

- **Icono de Estrella:**  
  Permite marcar eventos como favoritos para recibir recordatorios o guardarlos para futuras decisiones.

- **Icono de Ticket:**  
  Representa el acceso a las entradas de los eventos, tanto para la compra como para su visualización.

- **Icono de Notificación:**  
  Indica actualizaciones importantes, como cambios en la programación, nuevos eventos sugeridos o recordatorios de inscripción.



### 4.2.1. Organization Systems

#### Arquitectura de la Información de EventGO

Para estructurar la arquitectura de la información de **EventGO**, se ha adoptado un sistema de organización jerárquico tanto en la Landing Page como en la Aplicación Web. Este sistema facilita la navegación intuitiva y garantiza que los usuarios puedan encontrar fácilmente la información y las funciones que necesitan.

#### Landing Page

La Landing Page de **EventGO** se organiza de manera jerárquica para que los usuarios puedan acceder rápidamente a la información más relevante y a las acciones necesarias para interactuar con la plataforma:

#### Barra de Navegación Principal

Situada en la parte superior de la página, proporciona accesos rápidos a las secciones clave:

- **Inicio (Home):** La página de inicio que da la bienvenida a los usuarios y proporciona una visión general de los servicios de EventGO. Incluye un banner destacado con un mensaje central y botones de llamada a la acción para el registro e inicio de sesión.
- **Servicios (Services):** Presenta los servicios ofrecidos tanto para anfitriones de eventos como para organizadores profesionales. Esta sección está organizada para que cada tipo de usuario pueda identificar rápidamente cómo EventGO puede beneficiarles.
- **Planes (Plans):** Explica las diferentes opciones de planes disponibles para usuarios y organizadores, incluyendo características y beneficios de cada uno. Esta sección facilita la comparación y selección de la mejor opción.
- **Contáctanos (Contact Us):** Proporciona información de contacto, un formulario de consulta y enlaces a redes sociales, facilitando la comunicación entre los usuarios y el equipo de soporte de EventGO.
- **Nosotros (About Us):** Describe la misión, visión y el equipo detrás de EventGO, generando confianza y transparencia con los usuarios.

#### Estructura de Contenido Jerárquica

- **Encabezados y Subencabezados:** Organizan el contenido dentro de cada sección, permitiendo a los usuarios explorar más a fondo según sus intereses.
- **Botones de Llamada a la Acción (CTAs):** Colocados estratégicamente para guiar a los usuarios hacia acciones deseadas como crear un evento, contratar un organizador o contactar al equipo de EventGO.

#### Footer

Incluye enlaces a secciones importantes como políticas de privacidad, términos de servicio, contacto y enlaces a redes sociales. El footer proporciona una navegación adicional para usuarios que desean explorar más sobre EventGO.


#### Aplicación Web

La Aplicación Web de **EventGO** está diseñada para ofrecer una experiencia personalizada para dos segmentos principales de usuarios: **Anfitriones de Eventos** y **Organizadores Profesionales**. La organización del contenido permite que cada tipo de usuario navegue eficientemente por la aplicación.

#### Para Anfitriones de Eventos

- **Buscar Organizador (Search Organizer):** Permite a los anfitriones buscar organizadores de eventos según diferentes criterios, como tipo de evento, ubicación y presupuesto.
- **Mis Eventos (My Events):** Muestra una lista de eventos programados por el anfitrión, permitiendo ver detalles, asistentes y organizadores asignados.
- Cotizaciones (Quotes): Permite a los anfitriones recibir y gestionar cotizaciones de organizadores, facilitando la comparación de precios y servicios ofrecidos.
- **Mensajes (Messages):** Facilita la comunicación directa entre anfitriones y organizadores, permitiendo el intercambio de información y actualizaciones sobre eventos.
- **Reseñas (Reviews):** Permite a los anfitriones dejar reseñas y calificaciones sobre organizadores, ayudando a otros usuarios a tomar decisiones informadas.
- **Perfil (Profile):** Permite a los anfitriones gestionar su información personal, preferencias de notificación y configuración de cuenta.
- **Configuración:** Permite a los anfitriones ajustar sus preferencias de notificación, privacidad y otros aspectos de su cuenta.

#### Para Organizadores Profesionales

- **Mensajes (Messages):** Facilita la comunicación directa entre anfitriones y organizadores, permitiendo el intercambio de información y actualizaciones sobre eventos.
- **Cotizaciones (Quotes):** Permite a los anfitriones recibir y gestionar cotizaciones de organizadores, facilitando la comparación de precios y servicios ofrecidos.
- **Perfil (Profile):** Permite a los anfitriones gestionar su información personal, preferencias de notificación y configuración de cuenta.
- **Suscripción (Subscription):** Muestra el estado de la suscripción del anfitrión, incluyendo opciones de pago y renovación.
- **Tareas (Tasks):** Permite a los anfitriones gestionar tareas relacionadas con la planificación de eventos, asignando responsabilidades y fechas límite.
- **Eventos (Events):** Muestra una lista de eventos programados, permitiendo ver detalles, asistentes y organizadores asignados.
- **Calendario (Calendar):** Proporciona una vista de calendario con eventos programados, permitiendo a los anfitriones visualizar fechas y horarios de manera clara.
- **Dashboard:** Ofrece un resumen de los eventos activos, tareas pendientes, cotizaciones y mensajes recientes.


#### Interacción y Flujo de Trabajo

- Las interfaces están diseñadas para ser intuitivas y fáciles de usar, permitiendo a los usuarios completar tareas rápidamente con un mínimo de pasos.
- Cada sección dentro de la aplicación está claramente etiquetada y utiliza una combinación de texto, íconos y ayudas visuales para mejorar la usabilidad y la comprensión.


### 4.2.2. Labeling Systems

#### Sistemas de Etiquetado en EventGO ( Web Application PrimeVue)

En esta sección se describen los sistemas de etiquetado utilizados en la **Landing Page** y la **Aplicación Web** de **EventGO**, desarrollada con **PrimeVue**.  
El etiquetado está diseñado para facilitar la navegación mediante componentes UI preconstruidos, mejorando la experiencia del usuario.


#### Etiquetas de Encabezados (Headings)

Las etiquetas de encabezado se implementan utilizando componentes de PrimeVue como `<Card>`, `<Panel>` y `<Toolbar>`, facilitando la organización del contenido:

- **Inicio / Home:**  
  Banner de bienvenida utilizando `<Hero>`, botones `<Button>` de acceso rápido para registro e inicio de sesión.

- **Eventos / Events:**  
  Listado dinámico de eventos mediante `<DataTable>` o `<Listbox>`, mostrando detalles de cada evento.

- **Planes y Precios / Pricing Plans:**  
  Sección mostrada en `<Card>` para cada plan disponible, con botones de acción de registro rápido.

- **Contáctanos / Contact Us:**  
  Formulario de contacto con componentes `<InputText>`, `<Textarea>` y `<Button>` de envío.

- **Sobre Nosotros / About Us:**  
  Sección descriptiva presentada con `<Panel>` o `<Accordion>` para expandir información de misión y visión.


#### Etiquetas Textuales (Text Labels)

Las etiquetas textuales aparecen como propiedades `label` en botones y campos de entrada:

- **Buscar Eventos / Find Events:**  
  Barra de búsqueda implementada con `<InputText>` y botón `<Button label="Buscar">`.

- **Registrarse / Register:**  
  Botón de acción destacado usando `<Button>`.

- **Mis Eventos / My Events:**  
  Sección de eventos propios utilizando `<TabView>` para organizar eventos activos y pasados.

- **Historial / History:**  
  Listado de eventos anteriores con `<DataTable>` y opciones de filtrado.

- **Configuraciones / Settings:**  
  Acceso mediante `<Menu>` lateral o `<Sidebar>` a las preferencias del usuario.


#### Etiquetas Icónicas (Iconic Labels)

Se utilizan componentes `<Button>` con íconos embebidos (`icon="pi pi-search"`, `icon="pi pi-calendar"`, etc.):

- **Icono de Búsqueda (Lupa):** `pi pi-search`
- **Icono de Calendario:** `pi pi-calendar`
- **Icono de Estrella:** `pi pi-star`
- **Icono de Ticket:** `pi pi-ticket`
- **Icono de Notificación:** `pi pi-bell`


### 4.2.3. SEO Tags and Meta Tags


En el desarrollo de EventGO, la optimización para motores de búsqueda (SEO) juega un papel crucial para mejorar la visibilidad de la plataforma en línea. Los SEO tags y meta tags son herramientas esenciales que ayudan a los motores de búsqueda a comprender y clasificar el contenido de las páginas de la plataforma, asegurando que los usuarios encuentren EventGO de manera eficiente. Estos elementos permiten proporcionar información relevante, como el título de la página, la descripción, las palabras clave, y los datos específicos para mejorar la experiencia del usuario y atraer tráfico cualificado.

En este apartado, exploraremos los diferentes tipos de meta tags y SEO tags implementados en EventGO, cómo se utilizan para optimizar la indexación de nuestras páginas y las mejores prácticas que siguen los motores de búsqueda más utilizados.

#### Landing Page (Sitio Web Estático)

- **Title Tag: <br>**
  El title tag es uno de los factores más importantes en SEO, ya que determina el título que aparece en los resultados de búsqueda. Por eso decidimos que sea breve, relevante y que contenenga las palabras clave para mejorar una mejor visibilidad.
```html
<title>EventGO - Conecta, organiza y celebra tus eventos</title>
```
- **Meta Description: Tag <br>**
  La meta description proporciona un resumen conciso del contenido de la página. Es importante que sea atractiva y contenga palabras clave relevantes para aumentar la tasa de clicks en EventGO.
```html
<meta name="description" content="EventGO es la plataforma donde anfitriones encuentran al organizador ideal y organizadores hacen crecer su negocio. Conecta, organiza y celebra con confianza.">
```
- **Meta Keywords Tag: <br>**
  El meta keywords tag es menos relevante hoy en día, pero aún es útil para proporcionar información adicional sobre el contenido de la página. En este caso, hemos incluido palabras clave relacionadas con la organización de eventos y la conexión entre anfitriones y organizadores.
```html
<meta name="keywords" content="eventos, organización, anfitriones, organizadores, bodas, celebraciones, gestión de eventos, planificación de eventos">
```
- **Meta Author Tag: <br>**
  El meta author tag se utiliza para especificar el autor del contenido de la página. Aunque no impacta directamente en el SEO, lo consideramos útil para proporcionar transparencia y credibilidad.
```html
<meta name="author" content="Equipo EventGO">
```
- **Meta Viewport Tag: <br>**
  El Meta Viewport Tag es esencial para garantizar que el sitio se vea correctamente en dispositivos móviles. Asegura que la página sea responsiva, ajustando su escala según el tamaño de la pantalla del dispositivo. Decidimos implementarlo en EventGO para mejorar la experiencia del usuario en dispositivos móviles.
```html
<meta name="viewport" content="width=device-width, initial-scale=1.0">
```
- **Favicon: <br>**
  El favicon es el ícono que aparece en la pestaña del navegador. Es una forma sencilla de personalizar la apariencia de la página y mejorar la experiencia del usuario. Decidimos incluirlo en EventGO para ayudar a los usuarios a identificar nuestra plataforma de manera visual en múltiples pestañas.
```html
<link rel="icon" href="/assets/chapter-IV/EventGO_logo.png" type="image/png">
```

### Web Application (Aplicación Web Interactiva)
- **Title Tag: <br>**
  El title tag define el título que aparecerá en el navegador y en los resultados de búsqueda cuando los usuarios interactúen directamente con la aplicación. Decidimos usar un título dinámico que refleje la acción principal del usuario en la aplicación EventGO.
```html
<title>EventGO - Organiza tu evento</title>
```
- **Meta Description: <br>**
  La meta description proporciona un resumen conciso del contenido de la página. Es importante que sea atractiva y contenga palabras clave relevantes para aumentar la tasa de clicks en EventGO.
```html
<meta name="description" content="Usa EventGO para planificar, coordinar y comunicarte con organizadores o anfitriones en tiempo real. Todo desde una única plataforma eficiente y fácil de usar.">
```
- **Meta Keywords Tag: <br>**
  El meta keywords tag es menos relevante hoy en día, pero aún es útil para proporcionar información adicional sobre el contenido de la página. En este caso, hemos incluido palabras clave relacionadas con la organización de eventos y la conexión entre anfitriones y organizadores.
```html
<meta name="keywords" content="gestión de eventos, mensajería, proformas, seguimiento del evento, anfitriones, organizadores, EventGO app">
```
- **Meta Author Tag: <br>**
  El meta author tag se utiliza para especificar el autor del contenido de la página. Aunque no impacta directamente en el SEO, lo consideramos útil para proporcionar transparencia y credibilidad.
```html
<meta name="author" content="Equipo EventGO">
```
- **Meta Viewport Tag: <br>**
  El meta viewport tag es fundamental para que la aplicación web sea responsiva. Asegura que EventGO se vea y funcione correctamente en dispositivos móviles, ajustando el contenido al ancho de la pantalla del usuario. Decidimos incluirlo para ofrecer una experiencia fluida en cualquier dispositivo.
```html
<meta name="viewport" content="width=device-width, initial-scale=1.0">
```

### 4.2.4. Searching Systems

El sistema de búsqueda en la aplicación web de EventGO ha sido diseñado para facilitar el acceso rápido a información clave, permitiendo a los usuarios encontrar contenido específico dentro de las distintas secciones de la plataforma de forma eficiente y ordenada.

El sistema de búsqueda está presente en las siguientes áreas:

- **Calendario:** los usuarios pueden buscar reuniones pendientes o próximas.

- **Cotizaciones:** se permite buscar cotizaciones específicas y aplicar filtros de orden cronológico (de la más antigua a la más reciente).

- **Eventos:** se pueden buscar eventos por nombre o por nombre del organizador, así como aplicar filtros por fecha.

- **Mensajes:** los usuarios pueden localizar conversaciones específicas mediante un campo de búsqueda.

- **Perfil del Organizador:** los organizadores pueden buscar dentro de sus propios eventos en la sección “Mis eventos”.

En todos los casos, el sistema responde a una acción de búsqueda explícita del usuario, es decir, los resultados se muestran una vez se presiona el botón "Buscar". Esto permite al usuario tener un mayor control sobre cuándo desea ver los resultados filtrados o refinados.

Este enfoque contribuye a una experiencia más ágil y centrada, permitiendo que tanto anfitriones como organizadores encuentren rápidamente lo que necesitan dentro de la aplicación EventGO.

### 4.2.5. Navigation Systems

En la aplicación web interactiva de EventGO, el sistema de navegación ha sido diseñado para guiar a los usuarios de manera intuitiva hacia las funciones clave de la plataforma, asegurando una experiencia clara, accesible y eficiente.

El sistema está compuesto por:

- **Un menú superior** que permite cambiar el idioma entre español e inglés, facilitando la accesibilidad a usuarios con diferentes preferencias lingüísticas.

- **Un menú lateral** persistente con accesos rápidos a las secciones principales de la aplicación: Dashboard, Calendario, Eventos, Tareas, Cotizaciones, Mensajes, Perfil y Suscripción.

- **Para garantizar la usabilidad en dispositivos móviles**, se ha implementado un menú hamburguesa que reemplaza el menú lateral en pantallas pequeñas, asegurando una navegación responsiva.

- **En cada sección, se utilizan botones flotantes y enlaces internos** que permiten al usuario realizar acciones específicas (como crear eventos, enviar mensajes o cargar proformas) sin salir de su flujo de trabajo.

Este sistema de navegación facilita que tanto anfitriones como organizadores accedan rápida y ordenadamente a todas las funcionalidades necesarias para planificar y gestionar sus eventos en EventGO.
## _4.3. Landing Page UI Design_ ##

Esta sección expone el diseño de la Landing Page de EventGO, con el objetivo de atraer a los usuarios objetivo desde el primer momento. El enfoque del diseño es transmitir de forma clara el valor del producto, generar confianza e impulsar a la acción a través de una interfaz moderna, intuitiva y basada en principios de usabilidad.

### 4.3.1. Landing Page Wireframe
En esta sección se presentan las representaciones de bajo nivel **(wireframes)** del landing page, diseñadas para dispositivos móviles y de escritorio. [Wireframe - EventGO](https://www.figma.com/design/uPtLATLNkVL8P5xY7wBOc2/EventGO---Landing-page?node-id=0-1&t=yRuZCtcaOfFtQUmB-1)

**Desktop Web Browser**

**Header Section**: Encabezado de la landing page.

![header-section-wireframe-desktop](/img/Chapter%20IV/header-section-wireframe.png)

**Hero Section**: Sección principal de la landing page.

![hero-section-wireframe-desktop](/img/Chapter%20IV/hero-section-wireframe.png)

**About the product Section** : Sección donde se presentará información del producto.

![about-product-section-wireframe-desktop](/img/Chapter%20IV/about-the-product-section-wireframe.png)

**Functionalities Section**: Sección donde se mostrarán las funcionalidades ofrecidas.

![functionality-section-wireframe-desktop](/img/Chapter%20IV/functionality-section-wireframe.png)

**Benefits Section**: Se mostrarán los beneficios de usar EventGO.

![benefits-section-wireframe-desktop](/img/Chapter%20IV/benefits-section-wireframe.png)

**Plans Section**: Se mostrará información de los planes ofrecidos.

![plans-section-wireframe-desktop](/img/Chapter%20IV/plans-section-wireframe.png)

**About us Section**: Sección donde se presentan a los integrantes que desarrollaron EventGO.

![about-us-section-wireframe-desktop](/img/Chapter%20IV/about-us-section-wireframe.png)

**About the team Section**: Sección que contiene un video donde se resume el proceso del trabajo realizado por el equipo. 

![about-team-section-wireframe-desktop](/img/Chapter%20IV/about-the-team-section-wireframe.png)

**Footer Section** : Pie de página de la landing page

![footer-section-wireframe-desktop](/img/Chapter%20IV/footer-section-wireframe.png)

<br>

**Mobile Web Browser**

**Header Section**: Encabezado de la landing page.

![header-section-wireframe-desktop](/img/Chapter%20IV/header-section-mobile-wireframe.png)

**Hero Section**: Sección principal de la landing page.

![hero-section-wireframe-desktop](/img/Chapter%20IV/hero-section-mobile-wireframe.png)

**About the product Section**: Sección donde se presentará información del producto.

![about-product-section-wireframe-desktop](/img/Chapter%20IV/about-the-product-section-mobile-wireframe.png)

**Functionalities Section**: Sección donde se mostrarán las funcionalidades ofrecidas.

![functionality-section-wireframe-desktop](/img/Chapter%20IV/functionality-section-mobile-wireframe.png)

**Benefits Section**: Se mostrarán los beneficios de usar EventGO.

![benefits-section-wireframe-desktop](/img/Chapter%20IV/benefits-section-mobile-wireframe.png)

**Plans Section**: Se mostrará información de los planes ofrecidos.

![plans-section-wireframe-desktop](/img/Chapter%20IV/plans-section-mobile-wireframe.png)

**About us Section**: Sección donde se presentan a los integrantes que desarrollaron EventGO.

![about-us-section-wireframe-desktop](/img/Chapter%20IV/about-us-section-mobile-wireframe.png)

**About the team Section**: Sección que contiene un video donde se resume el proceso del trabajo realizado por el equipo. 

![about-team-section-wireframe-desktop](/img/Chapter%20IV/about-the-team-section-mobile-wireframe.png)

**Footer Section**: Pie de página de la landing page

![footer-section-wireframe-desktop](/img/Chapter%20IV/footer-section-mobile-wireframe.png)

### 4.3.2. Landing Page Mock-up

En esta sección se muestran los mock-ups del landing page, que sirven como una representación visual de alta fidelidad para anticipar cómo se verá y funcionará la interfaz final. Están diseñados tanto para dispositivos móviles como para escritorio. [Mock Ups - EventGO](https://www.figma.com/design/uPtLATLNkVL8P5xY7wBOc2/EventGO---Landing-page?node-id=0-1&t=yRuZCtcaOfFtQUmB-1)

**Desktop Web Browser**

**Header Section**: Encabezado de la landing page. Donde irán los botones para dirigirse directamente a alguna de las secciones de la landing page

![header-section-mockup](/img/Chapter%20IV/header-section-mockup-desktop.png)

**Hero Section**: Sección principal de la landing page. Dirigido para nuestros dos segmentos objetivos con una imagen referencial.

![hero-section-mockup](/img/Chapter%20IV/hero-section-mockup-desktop.png)

**About the product Section**: Sección donde se presentará información del producto. Cuenta con un video informativo.

![about-product-section-mockup](/img/Chapter%20IV/about-product-section-mockup-desktop.png)

**Functionalities Section**: Sección donde se mostrarán las funcionalidades ofrecidas.

![functionalities-section-mockup](/img/Chapter%20IV/functionality-section-mockup-desktop.png)

**Benefits Section**: Se mostrarán los beneficios de usar EventGO. 

![benefits-section-mockup](/img/Chapter%20IV/benefits-section-mockup-desktop.png)

**Plans Section**: Se mostrará información de los planes ofrecidos.

![plans-section-mockup](/img/Chapter%20IV/plans-section-mockup-desktop.png)

**About us Section**: Sección donde se presentan a los integrantes que desarrollaron EventGO.

![about-us-section-mockup](/img/Chapter%20IV/about-us-section-mockup-desktop.png)

**About the team Section**: Sección que contiene un video donde se resume el proceso del trabajo realizado por el equipo. 

![about-team-section-mockup](/img/Chapter%20IV/about-team-section-mockup-desktop.png)

**Footer Section**: Pie de página de la landing page

![footer-section-mockup](/img/Chapter%20IV/footer-section-mockup-desktop.png)


<br>

**Mobile Web Browser**

**Header Section**: Encabezado de la landing page. Donde irán los botones para dirigirse directamente a alguna de las secciones de la landing page

![header-section-mockup-mobile](/img/Chapter%20IV/header-section-mockup-mobile.png)

**Hero Section**: Sección principal de la landing page. Dirigido para nuestros dos segmentos objetivos con una imagen referencial.

![hero-section-mockup-mobile](/img/Chapter%20IV/hero-section-mockup-mobile.png)

**About the product Section**: Sección donde se presentará información del producto. Cuenta con un video informativo.

![about-product-section-mockup-mobile](/img/Chapter%20IV/about-the-product-section-mockup-mobile.png)

**Functionalities Section**: Sección donde se mostrarán las funcionalidades ofrecidas.

![functionalities-section-mockup-mobile](/img/Chapter%20IV/functionalities-section-mockup-mobile.png)

**Benefits Section**: Se mostrarán los beneficios de usar EventGO. 

![benefits-section-mockup-mobile](/img/Chapter%20IV/benefits-section-mockup-mobile.png)

**Plans Section**: Se mostrará información de los planes ofrecidos.

![plans-section-mockup-mobile](/img/Chapter%20IV/plans-section-mockup-mobile.png)

**About us Section**: Sección donde se presentan a los integrantes que desarrollaron EventGO.

![about-us-section-mockup-mobile](/img/Chapter%20IV/about-us-section-mockup-mobile.png)

**About the team Section**: Sección que contiene un video donde se resume el proceso del trabajo realizado por el equipo. 

![about-team-section-mockup-mobile](/img/Chapter%20IV/about-the-team-section-mockup-mobile.png)

**Footer Section**: Pie de página de la landing page

![footer-section-mockup-mobile](/img/Chapter%20IV/footer-section-mockup-mobile.png)

## 4.4. Web Applications UX/UI Design

Esta sección contiene secciones específicos donde se expone y explica la propuesta visual y de interacción de las aplicaciones, que conforman la experiencia del usuario al interactuar con los productos digitales.

### 4.4.1. Web Applications Wireframes

Esta sección presenta el diseño de los wireframes de nuestras aplicaciones, los cuales permiten planificar la estructura de la interfaz y la navegación antes de iniciar el desarrollo. Para este proyecto, se utilizó la herramienta Figma, facilitando una elaboración colaborativa y eficiente de los wireframes.

Segmento Organizadores de Eventos

Los siguientes wireframes pertenecen a la vista de login.

![wireframe-1.png](../img/Chapter%20IV/wireframe-1.png) 

Wireframes pertnenecientes a la vista de profile.

![wireframe-2.png](../img/Chapter%20IV/wireframe-2.png)

Wireframes de las vistas correspondientes al álbum de imágenes y el chat.

![wireframe-3.png](../img/Chapter%20IV/wireframe-3.png) 

Wireframes para el manejo personal de información.

![wireframe-4.png](../img/Chapter%20IV/wireframe-4.png)


Segmento Organizadores Anfitriones

Wireframes para el centro de planificación de eventos y el perfil del organizador anfitrión.

![wireframe-5a.png](../img/Chapter%20IV/wireframe-5a.png)

Wireframes correspondientes a la vista de portafolio, solicitud de prsupuesto e historial del organizador anfitrión.

![wireframe-6a.png](../img/Chapter%20IV/wireframe-6a.png)

Wireframe de la vista de los paquetes de servicio.

![wireframe-7a.png](../img/Chapter%20IV/wireframe-7a.png)

Wireframes para el contacto del host con el organizador.

![wireframe-8a.png](../img/Chapter%20IV/wireframe-8a.png)

Wireframes correspondientes a la lista de chats, rating y perfil del organizador anfitrión.

![wireframe-9a.png](../img/Chapter%20IV/wireframe-9a.png)

Wireframes correspondientes a las vistas de detalle de reseñas, y panel de notificaciones

![wireframe-10a.png](../img/Chapter%20IV/wireframe-10a.png)


### 4.4.2. Web Applications Wireflow Diagrams

Se presenta el enlace donde se realizaron los wireflows: https://tinyurl.com/3atdnfrt

Se presentaran los wireflows que competen con nuestros user goals

![wireflow-1.png](../img/Chapter%20IV/wireflow-1.png)

![wireflow-2.png](../img/Chapter%20IV/wireflow-2.png)

![wireflow-3.png](../img/Chapter%20IV/wireflow-3.png)

![wireflow-4.png](../img/Chapter%20IV/wireflow-4.png)

![wireflow-5.png](../img/Chapter%20IV/wireflow-5.png)

![wireflow-6.png](../img/Chapter%20IV/wireflow-6.png)

![wireflow-7.png](../img/Chapter%20IV/wireflow-7.png)

![wireflow-8.png](../img/Chapter%20IV/wireflow-8.png)

### 4.4.3. Web Applications Mock-ups
En esta sección se muestran los mock-ups del Web Applications, que sirven como una representación visual de alta fidelidad para anticipar cómo se verá y funcionará la interfaz final. [Mock Ups - EventGo](https://www.figma.com/design/3caqjycFbg1HlLcRI9Gpy4/EventGo?node-id=0-1&t=1Okc8pncZiyOBfWk-1)
<br>

Segmento Organizadores de Eventos

Vista de inicio de sesión

![login-screen 2.jpg](../img/Chapter%20IV/login-screen%202.jpg)

Vista para el registro de organizador

![register-organizer 1.jpg](../img/Chapter%20IV/register-organizer%201.jpg)

Vista para la recuperación de contraseña

![forgot-password 1.jpg](../img/Chapter%20IV/forgot-password%201.jpg)

Vista para la creación de una nueva contraseña
![reset-password 1.jpg](../img/Chapter%20IV/reset-password%201.jpg)

Vista para ingresar el codigo de verificación

![verification-code 1.jpg](../img/Chapter%20IV/verification-code%201.jpg)

Vista para restablecer la contraseña

![reset-password 1.jpg](../img/Chapter%20IV/reset-password%201.jpg)

Vista de perfil de organizador

![organizer-profile 1.jpg](../img/Chapter%20IV/organizer-profile%201.jpg)

Vista de actualización del perfil del organizador

![update-organizer-profile 1.jpg](../img/Chapter%20IV/update-organizer-profile%201.jpg)

Vista del álbum en el perfil del organizador

![almuns-profile-organizer.jpg](../img/Chapter%20IV/almuns-profile-organizer.jpg)

Vista para la edición del álbum

![album-detail 1.jpg](../img/Chapter%20IV/album-detail%201.jpg)

Vista para crear álbum

![create-album 1.jpg](../img/Chapter%20IV/create-album%201.jpg)

Vista para chat con los clientes

![direct-communication-mockup1-Org.jpg](../img/Chapter%20IV/direct-communication-mockup1-Org.jpg)


Segmento Organizadores Anfitriones 

Vista para el centro de planificaciones de eventos

![event-planning-hub 1.jpg](../img/Chapter%20IV/event-planning-hub%201.jpg)

Vista de portafolio con los eventos recientes

![service-portfolio 1.jpg](../img/Chapter%20IV/service-portfolio%201.jpg) 

Vista de las reseñas hacia los organizadores

![organizer-Historial-reseña-anfitrion2.jpg](../img/Chapter%20IV/organizer-Historial-rese%C3%B1a-anfitrion2.jpg) 

Vista del perfil de los anfitriones 

![organizer-profile-public 1.jpg](../img/Chapter%20IV/organizer-profile-public%201.jpg)

Vista de los detalles de las reseñas

![review-detail-mockup-continuation 1.jpg](../img/Chapter%20IV/review-detail-mockup-continuation%201.jpg)

Vista de historial de reseñas

![review-rating-mockup 1.jpg](../img/Chapter%20IV/review-rating-mockup%201.jpg)

Vista para contactar con el organizador

![Contact-to-organizator-from-host.jpg](../img/Chapter%20IV/Contact-to-organizator-from-host.jpg)

Vista para escribir una reseña

![write-review 1.jpg](../img/Chapter%20IV/write-review%201.jpg)

## _4.5. Web Applications Prototyping_ ##

El prototipo de EventGo, diseñado en Figma, muestra de manera visual e interactiva cómo sería la experiencia del usuario, considerando tanto a anfitriones como a organizadores de eventos. Cada tipo de usuario cuenta con funciones propias: los anfitriones pueden localizar organizadores, comunicarse mediante mensajes, administrar sus eventos y solicitar cotizaciones; mientras que los organizadores pueden gestionar las solicitudes recibidas, enviar formularios, preparar cotizaciones y hacer seguimiento de los eventos en curso.

![prototype-eventgo](../img/Chapter%20IV/prototype.png)

**link del prototipo:**  [Prototype](https://www.figma.com/design/3caqjycFbg1HlLcRI9Gpy4/EventGo?node-id=296-1170&t=1Okc8pncZiyOBfWk-1)

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

En esta sección se presentan los diagramas de clases que representan la estructura del sistema, incluyendo las entidades principales, sus atributos y métodos, así como las relaciones entre ellas. Estos diagramas son fundamentales para comprender cómo se modelan los datos y las interacciones dentro de la aplicación.

![class-diagram.png](../img/Chapter%20IV/class-diagram.png)

#### Authentication

| Clase/Enum | Descripción | Atributos | Métodos |
|------------|-------------|-----------|---------|
| **User** | Representa a un usuario del sistema EventGO | - `id`: UUID - Identificador único<br>- `email`: String - Correo electrónico<br>- `password`: String - Contraseña<br>- `name`: String - Nombre completo<br>- `role`: UserRole - Rol en el sistema<br>- `isActive`: boolean - Estado de activación<br>- `createdAt`: Date - Fecha de creación | - `register()`: Registra un nuevo usuario<br>- `login()`: Autentica al usuario<br>- `resetPassword()`: Restablece contraseña<br>- `validateEmail()`: Valida el correo |
| **UserRole** | Define los posibles roles de usuario | - `ORGANIZER`: Organizador de eventos<br>- `HOST`: Anfitrión de eventos | |

#### Profile Management

| Clase/Enum | Descripción | Atributos | Métodos |
|------------|-------------|-----------|---------|
| **Profile** | Información básica del perfil de usuario | - `id`: UUID - Identificador único<br>- `userId`: UUID - ID de usuario asociado<br>- `description`: String - Descripción<br>- `phone`: String - Teléfono<br>- `profilePicture`: String - URL de imagen<br>- `contactEmail`: String - Email de contacto<br>- `address`: String - Dirección<br>- `updatedAt`: Date - Última actualización | - `updateInformation()`: Actualiza información |
| **OrganizerProfile** | Perfil específico para organizadores | - Hereda atributos de Profile<br>- `yearsOfExperience`: int - Años de experiencia<br>- `specialties`: List<String> - Especialidades<br>- `ratings`: float - Calificación promedio | - `updateProfileOrganizer()`: Actualiza info del organizador |
| **HostProfile** | Perfil específico para anfitriones | - Hereda atributos de Profile<br>- `preferences`: List<String> - Preferencias | - `updateProfileHost()`: Actualiza info del anfitrión |
| **Album** | Colección de fotos de eventos | - `id`: UUID - Identificador único<br>- `organizerId`: UUID - ID del organizador<br>- `title`: String - Título<br>- `description`: String - Descripción<br>- `createdAt`: Date - Fecha de creación | - `createAlbum()`: Crea un nuevo álbum<br>- `addPicture()`: Añade una foto |
| **Picture** | Imagen almacenada en un álbum | - `id`: UUID - Identificador único<br>- `albumId`: UUID - ID del álbum<br>- `imageUrl`: String - URL de la imagen<br>- `description`: String - Descripción<br>- `uploadedAt`: Date - Fecha de carga | - `uploadPicture()`: Sube una imagen |

#### Event Management

| Clase/Enum | Descripción | Atributos | Métodos |
|------------|-------------|-----------|---------|
| **Event** | Representa un evento gestionado | - `id`: UUID - Identificador único<br>- `organizerId`: UUID - ID del organizador<br>- `hostId`: UUID - ID del anfitrión<br>- `title`: String - Título<br>- `description`: String - Descripción<br>- `location`: String - Ubicación<br>- `startDate`: Date - Fecha de inicio<br>- `endDate`: Date - Fecha de fin<br>- `status`: EventStatus - Estado<br>- `budget`: float - Presupuesto<br>- `maxAttendees`: int - Máx. asistentes<br>- `createdAt`: Date - Fecha de creación | - `createEvent()`: Crea un evento<br>- `updateEvent()`: Actualiza un evento<br>- `cancelEvent()`: Cancela un evento<br>- `completeEvent()`: Finaliza un evento |
| **EventStatus** | Estados posibles de un evento | - `PLANNING`: En planificación<br>- `CONFIRMED`: Confirmado<br>- `IN_PROGRESS`: En curso<br>- `COMPLETED`: Finalizado<br>- `CANCELLED`: Cancelado | |
| **Task** | Tarea relacionada a un evento | - `id`: UUID - Identificador único<br>- `eventId`: UUID - ID del evento<br>- `title`: String - Título<br>- `description`: String - Descripción<br>- `dueDate`: Date - Fecha límite<br>- `status`: TaskStatus - Estado<br>- `assignedTo`: String - Responsable<br>- `priority`: TaskPriority - Prioridad<br>- `createdAt`: Date - Fecha de creación | - `createTask()`: Crea una tarea<br>- `updateTaskStatus()`: Actualiza estado<br>- `assignTask()`: Asigna la tarea |
| **TaskStatus** | Estados posibles de una tarea | - `TODO`: Pendiente<br>- `IN_PROGRESS`: En progreso<br>- `DONE`: Completada | |
| **TaskPriority** | Prioridades de una tarea | - `LOW`: Baja<br>- `MEDIUM`: Media<br>- `HIGH`: Alta | |
| **Calendar** | Calendario de eventos | - `id`: UUID - Identificador único<br>- `userId`: UUID - ID del usuario<br>- `syncedWithGoogle`: boolean - Sincronizado<br>- `lastSyncDate`: Date - Última sincronización | - `syncWithGoogleCalendar()`: Sincroniza<br>- `addEvent()`: Añade evento<br>- `removeEvent()`: Elimina evento |

#### Payment and Subscription

| Clase/Enum | Descripción | Atributos | Métodos |
|------------|-------------|-----------|---------|
| **PaymentMethod** | Método de pago registrado | - `id`: UUID - Identificador único<br>- `userId`: UUID - ID del usuario<br>- `type`: PaymentMethodType - Tipo<br>- `cardNumber`: String - Número (parcial)<br>- `expiryDate`: Date - Vencimiento<br>- `isDefault`: boolean - Predeterminado<br>- `createdAt`: Date - Fecha de registro | - `addPaymentMethod()`: Registra método<br>- `removePaymentMethod()`: Elimina método<br>- `setAsDefault()`: Establece como predeterminado |
| **PaymentMethodType** | Tipos de métodos de pago | - `CREDIT_CARD`: Tarjeta de crédito<br>- `DEBIT_CARD`: Tarjeta de débito | |
| **Plan** | Plan de suscripción | - `id`: UUID - Identificador único<br>- `name`: String - Nombre<br>- `description`: String - Descripción<br>- `price`: float - Precio<br>- `duration`: int - Duración en días<br>- `features`: List<String> - Características<br>- `isActive`: boolean - Disponibilidad | - `activatePlan()`: Activa el plan<br>- `deactivatePlan()`: Desactiva el plan |
| **Subscription** | Suscripción de usuario a un plan | - `id`: UUID - Identificador único<br>- `userId`: UUID - ID del usuario<br>- `planId`: UUID - ID del plan<br>- `paymentMethodId`: UUID - ID del método de pago<br>- `startDate`: Date - Inicio<br>- `endDate`: Date - Fin<br>- `status`: SubscriptionStatus - Estado<br>- `autoRenew`: boolean - Renovación automática | - `subscribeToPlan()`: Suscribe al plan<br>- `cancelSubscription()`: Cancela suscripción<br>- `changePlan()`: Cambia de plan<br>- `renewSubscription()`: Renueva suscripción |
| **SubscriptionStatus** | Estados de una suscripción | - `ACTIVE`: Activa<br>- `CANCELLED`: Cancelada<br>- `EXPIRED`: Expirada | |

#### Quote Management

| Clase/Enum | Descripción | Atributos | Métodos |
|------------|-------------|-----------|---------|
| **Quote** | Cotización para un evento | - `id`: UUID - Identificador único<br>- `organizerId`: UUID - ID del organizador<br>- `hostId`: UUID - ID del anfitrión<br>- `eventId`: UUID - ID del evento<br>- `title`: String - Título<br>- `description`: String - Descripción<br>- `totalAmount`: float - Monto total<br>- `validUntil`: Date - Validez<br>- `status`: QuoteStatus - Estado<br>- `createdAt`: Date - Fecha de creación | - `createQuote()`: Crea cotización<br>- `acceptQuote()`: Acepta cotización<br>- `rejectQuote()`: Rechaza cotización<br>- `updateQuote()`: Actualiza cotización |
| **QuoteStatus** | Estados de una cotización | - `DRAFT`: Borrador<br>- `SENT`: Enviada<br>- `ACCEPTED`: Aceptada<br>- `REJECTED`: Rechazada<br>- `EXPIRED`: Expirada | |
| **ServiceItem** | Elemento de servicio en cotización | - `id`: UUID - Identificador único<br>- `quoteId`: UUID - ID de la cotización<br>- `name`: String - Nombre<br>- `description`: String - Descripción<br>- `unitPrice`: float - Precio unitario<br>- `quantity`: int - Cantidad<br>- `totalPrice`: float - Precio total | - `createServiceItem()`: Crea elemento<br>- `updateServiceItem()`: Actualiza elemento<br>- `removeServiceItem()`: Elimina elemento |

#### Communication

| Clase/Enum | Descripción | Atributos | Métodos |
|------------|-------------|-----------|---------|
| **Chat** | Conversación entre usuarios | - `id`: UUID - Identificador único<br>- `participantIds`: List<UUID> - Participantes<br>- `createdAt`: Date - Fecha de creación<br>- `lastActivity`: Date - Última actividad | - `createChat()`: Crea un chat<br>- `closeChat()`: Cierra un chat |
| **Message** | Mensaje enviado en un chat | - `id`: UUID - Identificador único<br>- `chatId`: UUID - ID del chat<br>- `senderId`: UUID - ID del remitente<br>- `content`: String - Contenido<br>- `sentAt`: Date - Fecha de envío<br>- `readAt`: Date - Fecha de lectura<br>- `status`: MessageStatus - Estado | - `sendMessage()`: Envía mensaje<br>- `markAsRead()`: Marca como leído |
| **MessageStatus** | Estados de un mensaje | - `SENT`: Enviado<br>- `DELIVERED`: Entregado<br>- `READ`: Leído | |
| **Notification** | Notificación del sistema | - `id`: UUID - Identificador único<br>- `userId`: UUID - ID del destinatario<br>- `type`: NotificationType - Tipo<br>- `content`: String - Contenido<br>- `isRead`: boolean - Estado de lectura<br>- `createdAt`: Date - Fecha de creación | - `createNotification()`: Crea notificación<br>- `markAsRead()`: Marca como leída |
| **NotificationType** | Tipos de notificaciones | - `MESSAGE`: Mensaje nuevo<br>- `QUOTE_REQUEST`: Solicitud de cotización<br>- `PAYMENT`: Relacionada con pagos<br>- `REMINDER`: Recordatorio<br>- `SYSTEM`: Del sistema | |

#### Reviews and Ratings

| Clase/Enum | Descripción | Atributos | Métodos |
|------------|-------------|-----------|---------|
| **Review** | Reseña sobre evento o servicio | - `id`: UUID - Identificador único<br>- `eventId`: UUID - ID del evento<br>- `hostId`: UUID - ID del anfitrión<br>- `organizerId`: UUID - ID del organizador<br>- `rating`: float - Calificación<br>- `comment`: String - Comentario<br>- `createdAt`: Date - Fecha de creación | - `createReview()`: Crea reseña<br>- `updateReview()`: Actualiza reseña |# Diccionario de Clases - Sistema EventGO

## _4.8. Database Design_ ##
### 4.8.1. Database Diagram ###
En esta sección, se presenta nuestro diagrama de base de datos desarrollado en Vertabelo, con sus respectivas relaciones y entidades.

![database-diagram.png](../img/Chapter%20IV/database-diagram.png)
[Link diagrama Vertabelo](https://my.vertabelo.com/public-model-view/FULssyMHN0FcM2xM3exStZY4DopgWkvqmmBCXcTuCWpZyZGKwu3ksoDXA1VBUtV7?x=4300&y=5000&zoom=0.75)