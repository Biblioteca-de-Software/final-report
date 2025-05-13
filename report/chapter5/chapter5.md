# Capítulo V: Product Implementation, Validation & Deployment

## 5.1. Software Configuration Management.

En esta sección se muestran las decisiones y convenciones que permitirán mantener consistencia durante el ciclo de vida del proyecto.

### 5.1.1. Software Development Environment Configuration.

En esta sección, se incluirá los productos de software que se usaron en el proyecto.
Los enlaces a cada una de las herramientas se encuentran disponibles en los anexos.

##### Project Management:
- Trello: Herramienta de gestión de proyectos basada en Kanban, utilizada para planificar tareas y asignar responsabilidades al equipo.

##### Product UX/UI Design:
- Figma: Herramienta colaborativa para crear prototipos interactivos de interfaces.
- Lucidchart: Para creación de diagramas de flujo y wireframes.
- Uxpressia: Para elaboración de mapas de empatía y recorridos del usuario (Customer Journey).
- Structurizr: Para modelado de arquitectura de software.

#### Software Development
- IntelliJ IDEA: IDE para desarrollo backend en Java. Para el primer y segundo sprint se utilizó para la redacción del informe del proyecto.
- WebStorm: IDE especializado para el desarrollo frontend. Se utilizó para el desarrollo de la Landing Page y frontend de la aplicación.
- Visual Studio Code: Editor utilizado únicamente para la exportación del reporte de formato markdown a PDF.
- GitHub: Plataforma de control de versiones y colaboración.

#### Software Deployment
- GitHub Pages: Servicio de despliegue de aplicaciones web estáticas desde repositorios GitHub.

### 5.1.2. Source Code Management.

Para la gestión del código fuente, se utilizará GitHub como plataforma central de control de versiones y colaboración entre los miembros del equipo. Se han creado repositorios separados para los distintos productos del proyecto.
Los enlaces también están disponibles en la sección de anexos.

- **Organización en GitHub:** [https://github.com/Biblioteca-de-Software](https://github.com/Biblioteca-de-Software)
- **Repositorio del informe final:** [https://github.com/Biblioteca-de-Software/final-report](https://github.com/Biblioteca-de-Software/final-report)
- **Repositorio de la Landing Page:** [https://github.com/Biblioteca-de-Software/landing-page](https://github.com/Biblioteca-de-Software/landing-page)
- **Repositorio del FrontEnd:** [https://github.com/Biblioteca-de-Software/frontend](https://github.com/Biblioteca-de-Software/frontend)

#### Modelo de ramificación: GitFlow

Para el modelo de desarrollo, se decidió usar GitFlow como modelo de ramificación. Este modelo permite una gestión eficiente de las ramas y facilita la colaboración entre los desarrolladores.

Para el repositorio del informe final se crearon las siguientes ramas:
- **dev:** Rama principal de desarrollo, donde se integrarán todas las características y correcciones de errores.
- **chapter-1:** Rama para el desarrollo del capítulo 1 del informe.
- **chapter-2:** Rama para el desarrollo del capítulo 2 del informe.
- **chapter-3:** Rama para el desarrollo del capítulo 3 del informe.
- **chapter-4:** Rama para el desarrollo del capítulo 4 del informe.
- **chapter-5:** Rama para el desarrollo del capítulo 5 del informe.

Para el repositorio de Landing Page se crearon las siguientes ramas:

Para el repositorio del Fronted se crearon las siguientes ramas:
- **develop**: Rama principal donde una vez concluida la programación de un bounded context se hace un merge a esta rama.
- **feature/orders**: Rama en la que se desarrolla el bounded context de órdenes donde una persona del segmento trabajadores del restaurante registra las órdenes de cada mesa.
- **feature/inventory**: Rama donde se desarrolla el bounded context del inventario donde una persona del segmento dueños de restaurante puede ingresar productos al inventario y revisar su fecha de caducidad.
- **feature/notifications**: Rama donde se desarrolla del bounded context de notificaciones donde el usuario, ya sea dueño o trabajador, puede ver todas las notificaciones. Es parte del core del negocio, ya que para el segmento de dueños las notificaciones le permiten estar alerta de la fecha de vencimiento de los productos. 
- **feature/userManagement**: Rama donde se desarrolla el código respecto a el registro o ingreso a la cuenta de cada segmento objetivo.

#### Estilo de commits: Conventional Commits
Para asegurar mensajes de commits claros y estandarizados, se seguirá la convención [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/). Algunos ejemplos:

- `feat: add search by name functionality`
- `fix: correct form validation error`
- `docs: update installation instructions`
- `refactor: simplify calculation logic`

El prefijo de categorías se define de la siguiente forma:
- `feat`: A new feature
- `fix`: A bug fix
- `docs`: Documentation only changes
- `style`: Changes that do not affect the meaning of the code (formatting, missing semicolons, etc.)
- `refactor`: A code change that neither fixes a bug nor adds a feature
- `test`: Adding missing tests or correcting existing ones
- `chore`: Changes to the build process or auxiliary tools

### 5.1.3. Source Code Style Guide & Conventions.

En esta sección se definen las convenciones de nombres y codificación adoptadas por el equipo para los lenguajes utilizados en el proyecto: HTML, CSS, JavaScript, TypeScript y Java. El idioma estándar para todo el código (nombres de variables, funciones, clases, archivos, etc.) es el **inglés**.

#### Principios generales

- **Idioma estándar:** Todo el código fuente está escrito en inglés, incluyendo nombres de archivos, clases, variables y funciones.
- **Legibilidad ante todo:** Se prioriza el uso de nombres descriptivos y claros por encima de abreviaciones o tecnicismos innecesarios.
- **Formato consistente:** Se aplica un estilo uniforme en todo el equipo y en todos los lenguajes, reforzado por herramientas automáticas.
- **Nombres semánticos:** Se usan **sustantivos** para clases, componentes y archivos, y **verbos** para funciones o métodos.
- **Indentación:** 2 espacios para HTML, CSS, JS y TS. 4 espacios para Java.

#### HTML y CSS

**HTML**
- Archivos terminan en `.html`.
- Se utilizan etiquetas semánticas como `<header>`, `<section>`, `<nav>`, `<footer>`, etc.
- Se incluye `alt` en imágenes y atributos `aria-*` para accesibilidad.
- Atributos con comillas dobles (`"`).
- Se usa `camelCase` para IDs y `kebab-case` para clases.
- Indentación: 2 espacios.

**CSS**
- Archivos terminan en `.css`.
- Se usa `kebab-case` para nombres de clases y archivos: `main-header`, `product-card`, `login-form`.
- Se agrupan estilos relacionados y se separan con comentarios.

#### JavaScript y TypeScript

- Archivos terminan en `.js` o `.ts`.
- Se usa `camelCase` para variables y funciones: `userName`, `getUserData()`.
- Se usa `PascalCase` para clases y componentes: `UserProfile`, `LoginForm`.
- Se prefiere `const` y `let` en lugar de `var`.
- Se prefieren funciones flecha (`=>`) y nombres explícitos.
- Cada archivo debe tener una única responsabilidad o componente.

Basado en:
- [Guía de estilo TypeScript de Google](https://google.github.io/styleguide/tsguide.html)
- [Guía de estilo JavaScript de Airbnb](https://github.com/airbnb/javascript)


#### Java

- Archivos terminan en `.java`.
- Clases con `PascalCase`: `UserService`, `OrderController`.
- Métodos y variables con `camelCase`: `getUserById()`, `userEmail`.
- Constantes con `UPPER_SNAKE_CASE`: `MAX_ATTEMPTS`.
- Una clase pública por archivo.
- Se documentan métodos y clases públicas con JavaDoc.

Basado en:
- [Guía de estilo Java de Google](https://google.github.io/styleguide/javaguide.html)
- [Buenas prácticas de Spring Boot](https://docs.spring.io/spring-boot/docs/current/reference/htmlsingle/)

### 5.1.4. Software Deployment Configuration.

En esta sección se describe la configuración necesaria para desplegar cada uno de los componentes del proyecto: Landing Page, Web Services y Frontend Web Application. El objetivo es garantizar que, a partir del código fuente almacenado en los repositorios, se pueda lograr una publicación funcional y accesible para los usuarios.

#### Despliegue de Landing Page

La **Landing Page** fue desarrollada usando HTML y CSS, y fue desplegada mediante **GitHub Pages**, un servicio gratuito de hosting para sitios estáticos.

**Pasos de despliegue:**
1. Se creó el repositorio `landing-page` en GitHub.
2. Se subió el código fuente HTML, CSS y recursos estáticos.
3. Desde la configuración del repositorio, se activó **GitHub Pages** seleccionando la rama `main` y la carpeta raíz (`/`).
4. Automáticamente, GitHub publicó el sitio web en una URL pública.

**Repositorio:** [https://github.com/Biblioteca-de-Software/landing-page](https://github.com/Biblioteca-de-Software/landing-page)  
**URL desplegada:** [https://biblioteca-de-software.github.io/landing-page/](https://biblioteca-de-software.github.io/landing-page/)

#### Frontend Web Application
El frontend se desplegó utilizando la herramienta Netlify.

**Pasos de despliegue:**
1. Build del proyecto: Generar los archivos estáticos de producción (ng build --configuration=production)
2. Verificar que el proyecto esté completado en la rama develop.
3. Creación de cuenta en Netlify
4. Click en "Add new site" → "Import an existing project" y elegir el repositorio y rama (develop)
5. Configurar build:
- Build command: ng build --configuration=production
- Publish directory: dist/nombre-de-tu-app

**Repositorio:** https://github.com/Biblioteca-de-Software/frontend

#### Restful API

Los servicios backend serán desarrollados en **Java (Spring Boot)** más adelante.

## 5.2. Landing Page, Services & Applications Implementation.

En esta sección se detalla y evidencia la implementación de cada entregable de KeepItFresh.

#### Landing page:
La landing page fue realizada de manera grupal y desplegada debidamente con la herramienta GitHub Pages.
A continuación las siguientes imágenes sirven de referencia para evidencia la implementación de la Landing Page.

![img_3.png](img_3.png)
![img_4.png](img_4.png)
![img_5.png](img_5.png)
![img_6.png](img_6.png)
![img_7.png](img_7.png)

#### Frontend:
El frontend fue realizado de manera grupal utilizando el framework Angular.
A continuación las siguientes imágenes sirven de referencia para evidencia la implementación del frontend.

![img_15.png](img_15.png)
![img_16.png](img_16.png)
![img_17.png](img_17.png)
![img_18.png](img_18.png)

### 5.2.1. Sprint 1

#### 5.2.1.1. Sprint Planning 1.

<table>
<tr>
    <th colspan="5">Sprint 1</th>
    <th colspan="9">Sprint 1</th>
  </tr>
      <tr>
    <td colspan="13">Sprint Planning Background</td>
  </tr>
  <tr>
    <td colspan="5">Date</td>
    <td colspan="8">2025-04-16</td>
</tr>
  <tr>
    <td colspan="5">Time</td>
    <td colspan="8">5:30 PM</td>
  </tr>
  <tr>
    <td colspan="5">Location</td>
    <td colspan="8">Via Discord</td>
<tr>
    <td colspan="5">Prepared By</td>
    <td colspan="8">Ayrton Omar Briceño Llanos</td>
</tr>
<tr>
    <td colspan="5">Attendees (to planning meeting)</td>
    <td colspan="8">Ayrton Omar Briceño Llanos, Maita Falckenheiner Romina Guadalupe, Lang Nassi Werner Khalil, Torres Flores Paolo Alessandro, Mamani Marca Gabriel Cristian.</td>
</tr>
<tr>
    <td colspan="5">Sprint  1 Review Summary</td>
    <td colspan="8">En este primer sprint se asignaron responsabilidades a cada integrante y planteo los requerimientos para el desarrollo de la Landing Page.</td>
</tr>
<tr>
    <td colspan="5">Sprint 1 Retrospective Summary</td>
    <td colspan="8">En esta sección todos los integrantes mencionaron tener aciertos en partes del codigo y en otras partes poder mejorar sus habilidades realizando la Landing Page</td>
</tr>
<tr>
    <td colspan="13">Sprint Goal & User Stories</td>
</tr>
<tr>
    <td colspan="5">Sprint 1 Goal</td>
    <td colspan="8">
Desarrollar y desplegar una landing page que presente información a los usuarios a través de imágenes. La página debe ser completamente adaptable a cualquier tipo de dispositivo que utilicen los usuarios, garantizando una experiencia de usuario fluida y responsiva.</td>
</tr>
</table>

#### 5.2.1.2. Aspect Leaders and Collaborators.

En esta sección se detalla los líderes de cada aspecto. Para el primer Sprint hemos segmentado en 3 aspectos relacionados a los entregables.

| Team member (LastName, First Name) | GitHub UserName | Aspect 1: Landing Page Leader (L) / Collaborator (C) | Aspect 2: Diseños Figma: Leader (L) / Collaborator (C) | Aspect 3: Reporte (L) / Collaborator (C) |
|------------------------------------|-----------------|------------------------------------------------------|--------------------------------------------------------|------------------------------------------|
| Maita Romina                       | RominaMaita     | C                                                    | C                                                      | L                                        |
| Torres Paolo                       | PaleToFo        | L                                                    | C                                                      | L                                        |
| Lang Werner                        | 00WernerLang    | C                                                    | L                                                      | L                                        |
| Briceño Ayrton                     | Ayrton          | C                                                    | L                                                      | L                                        |
| Mamani Gabriel                     | Gabriel0105     | C                                                    | C                                                      | L                                        |

#### 5.2.1.3. Sprint Backlog 1.

|  Sprint 1  |             Sprint 1            |     |                              |                                                                     |                    |             |                                                |
|:----------:|:-------------------------------:|:---:|:----------------------------:|:-------------------------------------------------------------------:|:------------------:|:-----------:|:----------------------------------------------:|
| User Story | Work-Item / Task                |     |                              |                                                                     |                    |             |                                                |
| Id         | Title                           | Id  | Title                        | Description                                                         | Estimation (Hours) | Assigned To | Status (To do / In process / To review / Done) |
| US01       | Registro de Producto            | W01 | Crear formulario de registro | Diseñar y codificar el formulario para ingresar datos del producto. | 3                  |   Ayrton    |                     To do                      |
| US02       | Consulta de inventario          | W02 | Crear vista de inventario    | Mostrar los productos almacenados y su stock actual.                | 4                  |   Romina    |                      Done                      |
| US03       | Registro de usuario             | W03 | Formulario de registro       | Crear un formulario de registro con validación de datos.            | 3                  |   Ayrton    |                    To review                    |
| US04       | Inicio de sesión                | W04 | Interfaz de login            | Crear pantalla de inicio de sesión con validación.                  | 2                  |    Paolo    |                   To review                    |
| US05       | Alertas de vencimiento          | W05 | Programar lógica de alerta   | Generar alertas automáticas según fecha de vencimiento.             | 1                  |   Werner    |                      Done                      |
| US06       | Registro de tiempo de respuesta | W06 | Medir tiempo de atención     | Registrar tiempo desde la solicitud hasta la atención.              | 2                  |   Gabriel   |                      Done                      |
| US07       | Solicitud de atención           | W07 | Crear formulario de atención | Interfaz para solicitar atención con datos necesarios.              | 2                  |   Gabriel   |                   To review                    |
| US08       | Resumen general para dueños     | W08 | Panel de resumen             | Crear dashboard con métricas clave (ventas, pedidos, etc).          | 2                  |    Paolo    |                      Done                      |
| US09       | Alertas visuales en dashboard   | W09 | Integrar alertas al panel    | Mostrar alertas de demora o alto volumen de pedidos.                | 2                  |   Werner    |                   To review                    |
<br>

#### 5.2.1.4. Development Evidence for Sprint Review.
En esta sección se demuestran los commits relacionados con los principales avances en la implementación.
Estos commits provienen del repositorio del frontend de la organización de GitHub.

🔗 Enlace al repositorio de la Landing Page: https://github.com/Biblioteca-de-Software/landing-page

| Repository                           | Branch | Commit Id                                 | Commit Message                 | Commit Message Body | Commited on (Date) |
|--------------------------------------|--------|-------------------------------------------|--------------------------------|---------------------|--------------------|
| Biblioteca-de-Software/landing-page  | main   | ac5503593079bdd29fcee4682e28a29cac8cc300  | feat(main): basic structure    |                     | 24/4/2025          |
| Biblioteca-de-Software/landing-page  | main   | f0d37bfbf9cd357a095eaea176d9515738bbc38e  | feat: added suscriptions plans |                     | 24/4/2025          |
| Biblioteca-de-Software/landing-page  | main   | 1312725155bd1bafd3abc0682592e7686a26ebd1  | feat: add opinions             |                     | 27/4/2025          |

#### 5.2.1.5. Execution Evidence for Sprint Review.
Este sprint estuvo únicamente enfocado en el desarrollo de la Landing Page. La cual fue programada en el repositorio "landing-page" de nuestra organización de Github.
![img_3.png](img_3.png)
![img_4.png](img_4.png)
![img_5.png](img_5.png)
![img_6.png](img_6.png)
![img_7.png](img_7.png)

#### 5.2.1.6. Services Documentation Evidence for Sprint Review.
Como se mencionó previamente, Este sprint solo tuvo como objetivo el desarrollo de Landing Page .Aún no se han implementado ni documentado Endpoints con OpenAPI, ya que el desarrollo de los servicios web está planificado para los siguientes Sprints, conforme al roadmap del proyecto.

#### 5.2.1.7. Software Deployment Evidence for Sprint Review.

Durante este Sprint, se completó el desarrollo de la Landing Page y se realizó su despliegue utilizando GitHub Pages como plataforma de publicación gratuita. El objetivo fue contar con una primera versión accesible en línea del producto digital para revisión y retroalimentación.

Actividades realizadas:
Se creó el repositorio en GitHub: https://github.com/Biblioteca-de-Software/landing-page

Se subió el código fuente de la Landing Page, incluyendo los archivos HTML, CSS necesarios.

Se configuró GitHub Pages desde la pestaña Settings > Pages, seleccionando la rama principal y la carpeta raíz.

Se verificó la correcta publicación de la Landing Page en la siguiente URL:

🔗 Landing Page desplegada: https://biblioteca-de-software.github.io/landing-page/

**Evidencia del despliegue:**
![img_2.png](img_2.png)

#### 5.2.1.8. Team Collaboration Insights during Sprint.
En esta sección se evidencia la colaboración de cada integrante en el repositorio de la Landing Page.

🔗 Repositorio de Landing Page: https://github.com/Biblioteca-de-Software/landing-page

#### Capturas de Insights del repositorio:
![img_9.png](img_9.png)


### 5.2.2. Sprint 2
### 5.2.2.1. Sprint Planning 2.

<table>
<tr>
    <th colspan="5">Sprint 2</th>
    <th colspan="9">Sprint 2</th>
  </tr>
      <tr>
    <td colspan="13">Sprint Planning Background</td>
  </tr>
  <tr>
    <td colspan="5">Date</td>
    <td colspan="8">06/05/2025</td>
</tr>
  <tr>
    <td colspan="5">Time</td>
    <td colspan="8">8:00 pm</td>
  </tr>
  <tr>
    <td colspan="5">Location</td>
    <td colspan="8">Via Discord</td>
<tr>
    <td colspan="5">Prepared By</td>
    <td colspan="8">Ayrton Omar Briceño Llanos</td>
</tr>
<tr>
    <td colspan="5">Attendees (to planning meeting)</td>
    <td colspan="8">Ayrton Omar Briceño Llanos, Maita Falckenheiner Romina Guadalupe, Lang Nassi Werner Khalil, Torres Flores Paolo Alessandro, Mamani Marca Gabriel Cristian.</td>
</tr>
<tr>
    <td colspan="5">Sprint  1 Review Summary</td>
    <td colspan="8">En este segundo sprint se definió los procesos necesarios para el desarrollo del frontend y correcciones necesarias de la landing page. Para ello, se asignaron responsabilidades a cada integrante.</td>
</tr>
<tr>
    <td colspan="5">Sprint 1 Retrospective Summary</td>
    <td colspan="8">Los integrantes mencionaron sus habilidades y puntos de mejora con respecto a la programación y diseño del frontend.</td>
</tr>
<tr>
    <td colspan="13">Sprint Goal & User Stories</td>
</tr>
<tr>
    <td colspan="5">Sprint 2 Goal</td>
    <td colspan="8">Desarrollar y desplegar una primera versión del frontend con las características más fundamentales con relación al negocio, con la finalidad de que los usuarios puedan interactuar con una interfaz funcional, validar los flujos principales del sistema y brindar retroalimentación temprana que permita ajustar el desarrollo de las siguientes iteraciones. </td>
</tr>
</table>

#### 5.2.2.2. Aspect Leaders and Collaborators.

En esta sección se detalla los líderes de cada aspecto. Para este segundo sprint se crearon 

| Team member (LastName, First Name) | GitHub UserName | Aspect 1: Landing Page Leader (L) / Collaborator (C) | Aspect 2: Figma Designs: Leader (L) / Collaborator (C) | Aspect 3: Report Leader (L) / Collaborator (C) | Aspect 4: Frontend (L) / Collaborator (C) | Aspect 5: Videos (L) / Collaborator (C) |
|------------------------------------|-----------------|------------------------------------------------------|--------------------------------------------------------|------------------------------------------------|-------------------------------------------|-----------------------------------------|
| Maita Romina                       | RominaMaita     | C                                                    | C                                                      | C                                              | L                                         | C                                       |
| Torres Paolo                       | PaleToFo        | C                                                    | C                                                      | L                                              | C                                         | C                                       |
| Lang Werner                        | 00WernerLang    | C                                                    | L                                                      | C                                              | C                                         | C                                       |
| Briceño Ayrton                     | Ayrton          | L                                                    | C                                                      | C                                              | C                                         | C                                       |
| Mamani Gabriel                     | Gabriel0105     | C                                                    | C                                                      | C                                              | C                                         | L                                       |

#### 5.2.2.3. Sprint Backlog 2.
| User Story ID | Title                               | Task ID | Title                          | Description                                                                                                      | Estimation | Assigned to | Status (To-do) |
|---------------|-------------------------------------|---------|--------------------------------|------------------------------------------------------------------------------------------------------------------|------------|-------------|----------------|
| US13          | Registro de Producto                | T01     | Crear formulario de registro   | Crear formulario en el frontend para registrar productos con nombre, categoría, cantidad y fecha de vencimiento. | 3h         | Paolo       | Done           |
|               |                                     | T02     | Configurar servicio HTTP       | Implementar servicio Angular para enviar los datos del producto al backend (JSON Server).                        | 2h         | Paolo       | Done           |
| US14          | Consulta de inventario              | T03     | Crear vista de inventario      | Desarrollar una página que muestre todos los productos registrados usando PrimeVue o Angular Material.           | 3h         | Paolo       | Done           |
| US15          | Alertas de vencimiento              | T06     | Mostrar alerta visual          | Mostrar alertas visuales (badge o toast) para productos próximos a vencer.                                       | 2h         | Paolo       | Done           |
| US16          | Ingresar nuevo pedido para una mesa | T07     | Creación de formulario         | Crear un formulario donde el trabajador del restaurante puede ingresar los pedidos de acuerdo al menú del día.   | 3h         | Paolo       | Done           |
|               |                                     | T08     | Validación y guardado          | Validar campos y guardar pedidos en el JSON Server.                                                              | 2h         | Romina      | Done           |
| US19          | Visualizar los pedidos por mesa     | T09     | Creación de cards de cada mesa | Crear cards que muestren las órdenes por mesa obtenidas desde el db.json.                                        | 3h         | Romina      | Done           |
|               |                                     | T12     | Enviar notificación            | Mostrar resumen al usuario mediante toast o modal al iniciar sesión cada día.                                    | 2h         | Werner      | Done           |
|               | Historial de alertas                | T13     | Guardar alertas en el backend  | Modificar backend (db.json) para almacenar historial de alertas de vencimiento.                                  | 2h         | Werner      | Done           |
|               |                                     | T14     | Mostrar historial al usuario   | Crear vista donde se pueda ver el historial de alertas con fecha y producto relacionado.                         | 2.5h       | Werner      | Done           |
|               | Reportes de ventas                  | T15     | Calcular totales de ventas     | Calcular ventas por día, semana o mes a partir de los pedidos registrados.                                       | 3h         | Ayrton      | Done           |
|               |                                     | T16     | Crear gráficos de reportes     | Mostrar resultados en gráficos usando alguna librería como Chart.js o ngx-charts.                                | 2.5h       | Ayrton      | Done           |
|               | Registro de usuario                 | T17     | Crear formulario de registro   | Crear formulario con campos como nombre, email, rol y contraseña.                                                | 2.5h       | Gabriel     | Done           |
|               |                                     | T18     | Guardar datos en backend       | Usar servicio HTTP para registrar usuario en el backend simulado.                                                | 2h         | Gabriel     | Done           |
|               | Inicio de sesión                    | T19     | Crear formulario de login      | Crear formulario de inicio de sesión con validación.                                                             | 2h         | Gabriel     | Done           |
|               |                                     | T20     | Verificar credenciales         | Comparar email y contraseña con lo almacenado en JSON Server y redirigir si es correcto.                         | 2h         | Gabriel     | Done           |

#### 5.2.X.4. Development Evidence for Sprint Review.
En esta sección se demuestran los commits relacionados con los principales avances en la implementación.
Estos commits provienen del repositorio del frontend de la organización de GitHub.

🔗 Enlace al repositorio del frontend: https://github.com/Biblioteca-de-Software/frontend

| Repository                       | Branch                 | Commit Id                                | commit Message                                                         | Commit Message Body | Commited on (Date) |
|----------------------------------|------------------------|------------------------------------------|------------------------------------------------------------------------|---------------------|--------------------|
| Biblioteca-de-Software/frontend  | feature/inventory      | 511a28fc33a708a84805bdb0b51526931a4acd77 | feat(inventory): add inventory entities.                               |                     |                    |
| Biblioteca-de-Software/frontend  | feature/inventory      | 7d9aee295dedaea2622e7e68466a5ee36be04dcc | feat(inventory): add inventory services.                               |                     |                    |
| Biblioteca-de-Software/frontend  | feature/inventory      | 3f49d70cbc19da5d44b5ed65bb4159d94be42f51 | feat(inventory): add inventory components.                             |                     |                    |
| Biblioteca-de-Software/frontend  | feature/orders         | 19e93de97fde7839a4f5c8c3bac2f5117eb9cca9 | feat(order): add order form component.                                 |                     | 09/05/2025         |
| Biblioteca-de-Software/frontend  | feature/orders         | d050f5b9c193e3c64e936f4b868b04dc640f7f43 | feat(order): add order page component.                                 |                     | 09/05/2025         |
| Biblioteca-de-Software/frontend  | feature/orders         | 1afe4f2d4c61966ed03286e5b2dabef5e78b8720 | feat(order): add order list component.                                 |                     | 09/05/2025         |
| Biblioteca-de-Software/frontend  | feature/orders         | 2913232089867f2da8fc86bb9f2c21e64637b48c | feat(order): add order response and assembler.                         |                     | 09/05/2025         |
| Biblioteca-de-Software/frontend  | feature/notifications  | 7e2b469de1cfe2d9eeb15b16dcea0a6029579b6b | feat(notification): add clickable notification.                        |                     | 12/05/2025         |
| Biblioteca-de-Software/frontend  | feature/notifications  | 0b0266c554c3a1c88d5c7425f6ff34f335403d8f | feat(notification): add notification filter for workers and inventory. |                     | 12/05/2025         |
| Biblioteca-de-Software/frontend  | feature/notifications  | 645fe146147833215d3470f41ac565c78cf89764 | feat(notification): add notification database example and route.       |                     | 12/05/2025         |

#### 5.2.2.5. Execution Evidence for Sprint Review.
Para este sprint se desarrolló una primera versión del frontend con el framework Angular.
A continuación, se evidencian las imágenes del frontend.

![img_15.png](img_15.png)
![img_16.png](img_16.png)
![img_17.png](img_17.png)
![img_18.png](img_18.png)

#### 5.2.2.6. Services Documentation Evidence for Sprint Review.
Durante el desarrollo del frontend de la aplicación, se utilizó JSON Server como una API falsa (fake API) con el objetivo de simular las funcionalidades del backend. Esta decisión se tomó debido a que el backend aún no se encuentra implementado. JSON Server permitió crear un entorno de pruebas funcional que responde a peticiones HTTP (GET, POST, PUT, DELETE) como lo haría un servidor real, utilizando un archivo db.json como fuente de datos persistente. Gracias a esto, fue posible desarrollar, probar y validar las interfaces de usuario y los servicios del frontend de manera efectiva, manteniendo una arquitectura desacoplada y preparada para integrarse con el backend real en el futuro.

#### 5.2.2.7. Software Deployment Evidence for Sprint Review.

#### 5.2.2.8. Team Collaboration Insights during Sprint.
En esta sección se evidencia la colaboración de cada integrante en el repositorio de la Landing Page.
🔗 Repositorio de Frontend: https://github.com/Biblioteca-de-Software/frontend

#### Capturas de Insights del repositorio:
![img_14.png](img_14.png)


# Conclusiones
Durante el proceso de creación y desarrollo de este trabajo pudimos llegar a las siguientes conclusiones:
- La importancia del trabajo en equipo y la colaboración entre los miembros del grupo.
- La importancia de la planificación y organización en el desarrollo de software.
- La importancia de la tecnología y las herramientas en el desarrollo de software aplicado a la realidad.
- Se concluye que este trabajo es una solución rentable y sostenible para la problemática de la reducción de desperdicios alimentarios en el Perú por medio de los restaurantes.
- Se usa la tecnología de la información y la comunicación para poder llegar a un público más amplio y poder ayudar a la reducción de desperdicios alimentarios en el Perú.
- Se concluye que la aplicación es fácil de usar y tiene una buena usabilidad, lo que permite a los usuarios interactuar con ella de manera eficiente.
- Se concluye que la aplicación es escalable y puede adaptarse a diferentes necesidades y requerimientos de los usuarios.

# Video About-the-Team.

# Bibliografía

- Digitalización de las instituciones hospitalarias._ (s/f). Cepal.org. Recuperado el 5 de septiembre de 2024, de https://desarrollodigital.cepal.org/es/datos-y-hechos/digitalizacion-de-las-instituciones-hospitalarias

- Conne, M(2024). _The Markdown Guide_. MarkdownGuide. Recuperado de: https://www.markdownguide.org/

- Conventional Commits. (n.d.). *Conventional commits v1.0.0.* Retrieved from https://www.conventionalcommits.org/en/v1.0.0/

- Angular. (n.d.). *Angular Material components.* Retrieved from https://material.angular.io/components/categories

- AngularJS. (n.d.). *AngularJS Material.* Retrieved from https://material.angularjs.org/latest/

- BrowserStack. (n.d.). Responsive Web Design: A Complete Guide. Recuperado de https://www.browserstack.com/guide/responsive-web-design

- Spring Boot. (n.d.). Spring Boot Documentation. Retrieved from https://docs.spring.io/spring-boot/documentation.html#documentation.web

- Modyo. (n.d.). Domain-Driven Design (DDD) - Patrones de arquitectura. Retrieved from https://docs.modyo.com/es/architecture/patterns/ddd.html


# Anexos

### VIDEOS:

| Título                  | Descripción                                        | Enlace                          |
|-------------------------|----------------------------------------------------|---------------------------------|
| Video de exposición TB1 | Video explicativo de los avances de la entrega TB1 | https://acortar.link/Vr5XIl     |
| Video de entrevistas    | Video recopilatorio de todas las entrevistas       | https://acortar.link/9818Zn     |  

### DIAGRAMAS:
**Anexo B: Diagrama de clases**<br>

| Título                    | Descripción                                                 | Enlace |
|---------------------------|-------------------------------------------------------------|--------|
| Diagrama de base de datos | Enlace al diagrama de base de datos realizado en Lucidchart |        | 
| Diagrama de clases        | Enlace al diagrama clases realizado en Lucidchart           |        | 

### UX/UI
| Título | Descripción                                                                                                | Enlace                       |
|--------|------------------------------------------------------------------------------------------------------------|------------------------------|
| Figma  | Enlace hacia el documento de Figma con todos los diseños planteados para tanto Frontend como Landing Page. | https://acortar.link/4Ym8OK  | 

### GITHUB

| Título       | Descripción                            | Enlace                                                |
|--------------|----------------------------------------|-------------------------------------------------------|
| Reporte      | Enlace al repositorio del reporte      | https://biblioteca-de-software.github.io/final-report |
| Landing Page | Enlace al repositorio del Landing Page | https://biblioteca-de-software.github.io/landing-page |
| Frontend     | Enlace al repositorio del frontend     | https://biblioteca-de-software.github.io/frontend     |

