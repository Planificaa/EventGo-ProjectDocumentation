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



### 4.6.1. Design-Level Event Storming ###



### 4.6.2. Software Architecture Context Diagram ###



### 4.6.3. Software Architecture Container Diagrams ###



### 4.6.4. Software Architecture Components Diagrams ###



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
