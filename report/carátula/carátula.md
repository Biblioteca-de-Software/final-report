# UNIVERSIDAD PERUANA DE CIENCIAS APLICADAS

## Carrera: Ingeniería de Software
## Desarrollo de Aplicaciones Open Source - Presencial 
## PROFESOR: Ángel Augusto
## Sección: 1ASI0729
## INFORME TB1
## START UP: BIBLIOTECA DE SOFTWARE
## PRODUCTO: KeepItFresh

### INTEGRANTES:
<table>
  <thead>
    <tr>
      <th style="background-color: #333; color: #fff;">Apellidos y Nombres</th>
      <th style="background-color: #333; color: #fff;">Código de Alumno</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Briceño Llanos, Ayrton Omar</td>
      <td>U202311077</td>
    </tr>
    <tr>
      <td>Lang Nassi, Werner Khalil</td>
      <td>U202310003</td>
    </tr>
    <tr>
      <td>Mamani Marca, Gabriel Cristian</td>
      <td>U202220659</td>
    </tr>
    <tr>
      <td>Torres Flores, Paolo Alessandro</td>
      <td>U20221F613</td>
    </tr>
    <tr>
      <td>Maita Falckenheiner, Romina Guadalupe</td>
      <td>U202213765</td>
    </tr>
  </tbody>
</table>

--- 

Ciclo 2025-01


# Registro de versiones del informe

| Versión | Fecha      | Autor | Descripción de modificación                                                                                                                                                                              |
|---------|------------|-------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| TB1     | 24/04/2025 | Briceño Llanos, Ayrton Omar<br/>Lang Nassi, Werner Khalil<br/>Mamani Marca, Gabriel Cristian<br/>Torres Flores, Paolo Alessandro<br/>Maita Falckenheiner, Romina Guadalupe      | Se realizó la documentación respectiva a los capítulos I, II, III, IV y V así como también se realizaron los diagramas correspondientes, deployment de la landing page así como la creación de la misma. |


# Project Report Collaboration Insights

# Contenido

## Tabla de Contenidos
### [Registro de versiones del informe](#registro-de-versiones-del-informe)
### [Project Report Collaboration Insights](#project-report-collaboration-insights)
### [Contenido](#contenido)
### [Student Outcome](#student-outcome-1)
### [Capítulo I: Introducción](#capc3adtulo-i-introduccic3b3n-1)
- [1.1. Startup Profile](#11-startup-profile)
    - [1.1.1. Descripción de la Startup](#111-description-de-la-startup)
    - [1.1.2. Perfiles de integrantes del equipo](#112-perfiles-de-integrantes-del-equipo)
- [1.2. Solution Profile](#12-solution-profile)
    - [1.2.1 Antecedentes y problemática](#121-antecedentes-y-problemática)
    - [1.2.2 Lean UX Process](#122-lean-ux-process)
        - [1.2.2.1. Lean UX Problem Statements](#1221-lean-ux-problem-statements)
        - [1.2.2.2. Lean UX Assumptions](#1222-lean-ux-assumptions)
        - [1.2.2.3. Lean UX Hypothesis Statements](#1223-lean-ux-hypothesis-statements)
        - [1.2.2.4. Lean UX Canvas](#1224-lean-ux-canvas)
- [1.3. Segmentos objetivo](#13-segmentos-objetivo)

### [Capítulo II: Requirements Elicitation & Analysis](#capc3adtulo-ii-requirements-elicitation--analysis-1)
- [2.1. Competidores](#21-competidores)
    - [2.1.1. Análisis competitivo](#211-análisis-competitivo)
    - [2.1.2. Estrategias y tácticas frente a competidores](#212-estrategias-y-tácticas-frente-a-competidores)
- [2.2. Entrevistas](#22-entrevistas)
    - [2.2.1. Diseño de entrevistas](#221-diseño-de-entrevistas)
    - [2.2.2. Registro de entrevistas](#222-registro-de-entrevistas)
    - [2.2.3. Análisis de entrevistas](#223-análisis-de-entrevistas)
- [2.3. Needfinding](#23-needfinding)
    - [2.3.1. User Personas](#231-user-personas)
    - [2.3.2. User Task Matrix](#232-user-task-matrix)
    - [2.3.3. User Journey Mapping](#233-user-journey-mapping)
    - [2.3.4. Empathy Mapping](#234-empathy-mapping)
    - [2.3.5. As-is Scenario Mapping](#235-as-is-scenario-mapping)
    - [2.4. Ubiquitous Language](#24-Ubiquitous-language)
### [Capítulo III: Requirements Specification](#capc3adtulo-iii-requirements-specification-1)
- [3.1. To-Be Scenario Mapping](#31-to-be-scenario-mapping)
- [3.2. User Stories](#32-user-stories)
- [3.3. Impact Mapping](#33-impact-mapping)
- [3.4. Product Backlog](#34-product-backlog)

### [Capítulo IV: Product Design](#capc3adtulo-iv-product-design-1)
- [4.1. Style Guidelines](#41-style-guidelines)
    - [4.1.1. General Style Guidelines](#411-general-style-guidelines)
    - [4.1.2. Web Style Guidelines](#412-web-style-guidelines)
- [4.2. Information Architecture](#42-information-architecture)
    - [4.2.1. Organization Systems](#421-organization-systems)
    - [4.2.2. Labeling Systems](#422-labeling-systems)
    - [4.2.3. SEO Tags and Meta Tags](#423-seo-tags-and-meta-tags)
    - [4.2.4. Searching Systems](#424-searching-systems)
    - [4.2.5. Navigation Systems](#425-navigation-systems)
- [4.3. Landing Page UI Design](#43-landing-page-ui-design)
    - [4.3.1. Landing Page Wireframe](#431-landing-page-wireframe)
    - [4.3.2. Landing Page Mock-up](#432-landing-page-mock-up)
- [4.4. Web Applications UX/UI Design](#44-web-applications-uxui-design)
    - [4.4.1. Web Applications Wireframes](#441-web-applications-wireframes)
    - [4.4.2. Web Applications Wireflow Diagrams](#442-web-applications-wireflow-diagrams)
    - [4.4.3. Web Applications Mock-ups](#443-web-applications-mock-ups)
    - [4.4.4. Web Applications User Flow Diagrams](#444-web-applications-user-flow-diagrams)
- [4.5. Web Applications Prototyping](#45-web-applications-prototyping)
- [4.6. Domain-Driven Software Architecture](#46-domain-driven-software-architecture)
    - [4.6.1. Software Architecture Context Diagram](#461-software-architecture-context-diagram)
    - [4.6.2. Software Architecture Container Diagrams](#462-software-architecture-container-diagrams)
    - [4.6.3. Software Architecture Components Diagrams](#463-software-architecture-components-diagrams)
- [4.7. Software Object-Oriented Design](#47-software-object-oriented-design)
    - [4.7.1. Class Diagrams](#471-class-diagrams)
    - [4.7.2. Class Dictionary](#472-class-dictionary)
- [4.8. Database Design](#48-database-design)
    - [4.8.1. Database Diagram](#481-database-diagram)

### [Capítulo V: Product Implementation, Validation & Deployment](#capc3adtulo-v-product-implementation-validation--deployment-1)
- [5.1. Software Configuration Management](#51-software-configuration-management)
    - [5.1.1. Software Development Environment Configuration](#511-software-development-environment-configuration)
    - [5.1.2. Source Code Management](#512-source-code-management)
    - [5.1.3. Source Code Style Guide & Conventions](#513-source-code-style-guide--conventions)
    - [5.1.4. Software Deployment Configuration](#514-software-deployment-configuration)
- [5.2. Landing Page, Services & Applications Implementation](#52-landing-page-services--applications-implementation)
    - [5.2.1. Sprint 1](#521-sprint-1)
        - [5.2.1.1. Sprint Planning 1](#5211-sprint-planning-1)
        - [5.2.1.2. Sprint Backlog 1](#5212-sprint-backlog-1)
        - [5.2.1.3. Development Evidence for Sprint Review](#5213-development-evidence-for-sprint-review)
        - [5.2.1.4. Testing Suite Evidence for Sprint Review](#5214-testing-suite-evidence-for-sprint-review)
        - [5.2.1.5. Execution Evidence for Sprint Review](#5215-execution-evidence-for-sprint-review)
        - [5.2.1.6. Services Documentation Evidence for Sprint Review](#5216-services-documentation-evidence-for-sprint-review)
        - [5.2.1.7. Software Deployment Evidence for Sprint Review](#5217-software-deployment-evidence-for-sprint-review)
        - [5.2.1.8. Team Collaboration Insights during Sprint](#5218-team-collaboration-insights-during-sprint)

### [Conclusiones](#conclusiones-1)
- [Conclusiones y recomendaciones](#conclusiones-y-recomendaciones)

### [Bibliografía](#bibliografc3ada-1)
### [Anexos](#anexos-1)

# Student Outcome

ABET – EAC - Student Outcome 3

Se refiere a la capacidad de comunicarse efectivamente con un rango de audiencias.
En el siguiente cuadro se describe las acciones realizadas y enunciados de
conclusiones por parte del grupo, que permiten sustentar el haber alcanzado el logro
del ABET – EAC - Student Outcome 3.


| Criterio específico                                                   | Acciones realizadas                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 | Conclusiones |
|-----------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|--------------|
| Comunica oralmente con efectividad a diferentes rangos de audiencia.  | TB1:<br>        **Romina Guadalupe Maita Falckenheiner:** En esta entrega hice uso de mis habilidades de comunicación para poder coordinar y realizar las entrevistas, además que me mantuve al tanto con el equipo para completar las siguientes tareas: Landing Page, Impact Mapping, Carátula, Diagrama de Clases, Diagrama Base de Datos, entrevistas, etc. <br/> **Paolo Alessandro Torres Flores:** Para este entregable, puse en práctica mi efectividad de comunicación oral al momento de coordinar las tareas mediante la repartición de las mismas. Además, por medio del desarrollo de puntos como las entrevistas, su resumen y su análisis respectivo. Por último, pude aplicar la comunicación oral al momento de grabar el video expositivo y comunicando eficazmente a lo que apunta nuestro proyecto. Cabe resaltar, que lo puntos mencionados son donde resalta la comunicación oral más no son los únicos desarrollados por mi persona.<br> **Werner Khalil Lang Nassi:** En este enregable, di uso de mis habilidades comunicativas de forma oral cuando se cordinaron los tiempos y temas que tomariamos. Asi mismo por medio de la misma, logre desarollar la entrevista a uno de nuestros segmentos objetivos. Al final logre usar mis habilidades orales de forma efectiva en el momento de la grabacion del video sobre la documentacion.                         |Adapto mi forma de comunicarme según el perfil de la audiencia, utilizando códigos y recursos adecuados para asegurar la correcta transmisión del mensaje. Empleo medios audiovisuales pertinentes al contenido que deseo presentar, y verifico constantemente que la comunicación haya sido clara y efectiva. Durante la presentación de resultados, oriento mi discurso hacia los objetivos específicos, garantizando la comprensión del mensaje. Además, practico la escucha activa y objetiva antes de emitir juicios, promoviendo siempre el diálogo y la conciliación.              |
| Comunica por escrito con efectividad a diferentes rangos de audiencia | TB1:<br>        **Romina Guadalupe Maita Falckenheiner:** En esta entrega, coordiné con el equipo a través de WhatsApp y Discord. Usé WhatsApp para asignar tareas de manera rápida y efectiva, mientras que en Discord mantuvimos conversaciones más detalladas sobre las entrevistas que estaba realizando. Esta combinación me permitió tener una comunicación fluida y asegurarme de que el equipo tuviera claro el progreso de cada tarea.<br/> **Paolo Alessandro Torres Flores:** Para la presente entrega, pude aplicar mis habilidades comunicativas escritas mediante la coordinación de tareas y toma de posta para el liderazgo del equipo cuando se necesitaba. Repartiendo tareas y delegando las mismas mediante aplicaciones de mensajería como: Whatsapp o Discord. En el desarollo, pude aplicar estas habilidades en el desarrollo de la diapositiva de exposición y el análisis de entrevistas, así como también pude aplicarlo la creación de la landing page. <br> **Werner Khalil Lang Nassi:** En esta entrega logre usar mis habilidades comunicativas escritas cuando fue requerido coordinar entre el equipo diversas tareas. Asi mismo logre comunicar varias secciones de este entrgable de forma efectiva usando mis capacidades escritas. Considero que el uso de las diferentes aplicacion tales como: Whatssap y Discord ayudaron al equipo a consolidar la comunicacion escrita entre todos, teniando una coordinacion de alto nivel y cumplir con lo coordinado. | Elaboro informes técnicos siguiendo los estándares establecidos para el desarrollo de proyectos de ingeniería, asegurando la calidad del contenido antes de su entrega. Me esfuerzo por transmitir ideas y conceptos clave de forma clara y empática, adaptando el nivel de detalle y el lenguaje escrito a las características del público, independientemente de su especialidad o jerarquía. Selecciono de manera cuidadosa los medios y formatos más adecuados para facilitar la comprensión del mensaje, y verifico sistemáticamente que todos los atributos de calidad estén presentes antes de la presentación final.             |