# Capítulo I: Introducción

## 1.1. Startup Profile
A continuación, se brindará información sobre a qué se dedica nuestra empresa, Go4U.

### 1.1.1. Descripción de la Startup

**Go4U** es una startup dedicada a soluciones digitales enfocadas en restaurantes. Utilizamos tecnologías IoT para agilizar la gestión de restaurantes. Nuestro enfoque es preventivo, proporcionando sensores y herramientas para evitar problemas tales como la descomposición de alimentos. No ofrecemos servicios de intervención, ni de acción inmediata.<br>

- **Misión:** Facilitar la gestión de los restaurantes a través de tecnologías las cuales permiten el monitoreo continuo del restaurante, al igual que optimizan la atención de los trabajadores, para que estos puedan ofrecer un mejor servicio a sus consumidores. 
- **Visión:** Ser la empresa más importante en Perú, en el ámbito de gestión y optimización de restaurantes con el uso de soluciones tecnológicas.
- **Producto:** “KeepItFresh” es un servicio el cual permite el monitoreo de puntos críticos del inventario de un restaurante, monitoreando fechas de caducidad, temperaturas y gases (tales como etileno y calidad de aire) para confirmar los niveles de descomposición de los productos en el inventario del restaurante. Así mismo este servicio también ofrece un botón para llamar a los trabajadores del restaurante desde la mesa, con el fin de optimizar la atención dirigida al consumidor.

### 1.1.2. Perfiles de integrantes del equipo

|                                                            | Apellido y Nombre | Carrera                | Acerca de                                                                                                                                                                                                                                                                                                                                                         | Habilidades                                                                                                                                                                        |
|------------------------------------------------------------|----------------|------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| ![Ayrton_Llanos.jpeg](../../assets/chapter1/Ayrton_Llanos.jpeg)                                                           | Briceño Llanos, Ayrton Omar | Ingeniería de Software | Soy Ayrton Briceño. Me apasiona el desarrollo de Software y la creación de soluciones tecnológicas que impacten positivamente en las personas. | JavaScript, CSS, C#, HTML, Java, SQL Server, MongoDB                                                                                                                               |
| <img src="/assets/chapter1/RominMaita.jpeg">               | Maita Falckenheiner, Romina Guadalupe | Ingeniería de Software | Soy estudiante a tiempo completo, me apasiona programar y me gustaría especializarme en Data Science o Desarrollo de Videojuegos en un futuro. | Liderazgo, competitividad y organización.                                                                                                                                          |
| <img src="/assets/chapter1/Perfil_Werner_Lang.jpg">        | Lang Nassi, Werner Khalil | Ingeniería de Software | Estudiante de la Universidad Peruana de Ciencias Aplicadas (UPC), cursando en 5.º ciclo. Soy un estudiante que le gusta investigar cosas nuevas. | Investigador, Innovador, Analista, Cooperativo.                                                                                                                                    |
| ![Perfil_Paolo.png](../../assets/chapter1/Perfil_Paolo.png) | Torres Flores, Paolo Alessandro | Ingeniería de Software | Soy un estudiante de 5to ciclo con afán de mejorar cada día que pasa. Tengo muchas aspiraciones, ya sea en mi carrera como personalmente, y lucho diariamente para acercarme cada vez más a ellas. | Me considero una persona adaptable al entorno, sé trabajar en equipo y aprendo rápido. Mentalidad para resolver problemas. Conocimiento básico de las funcionalidades de software. |
|  ![GabrielMamani.jpg](../../assets/chapter1/GabrielMamani.jpg)                                                          | Mamani Marca, Gabriel Cristian(u202220659)               | Ingeniería de Software | Soy estudiante de sexto ciclo de la carrera de Ingeniería de Software.En mis tiempos libres estudio otras tecnologías,juego y veo futbol | Durante el camino aprendi lenguajes como c++,python y java.Tambien,sobre motores de base de datos como MongoDb y MYSQL                                                             |

## 1.2. Solution Profile

**Product Name:** KeepItFresh <br>
**Product Description:** KeepItFresh, es una Web App que tiene como objetivo optimizar la gestión de los restaurantes. Para ello, esta permite al usuario monitorear los IoT que este tiene, mostrando información útil, ayudando con la gestión de inventarios y agilizando el trabajo de los trabajadores en la tienda. Los dueños de los restaurantes pueden usar KeepItFresh con el fin de optimizar varios procesos. <br>
**Monetización:** KeepItFresh funciona mediante un modelo de suscripción mensual o anual, en el cual se alquilan los diferentes dispositivos IoT.

 **Plan Básico:**

Ideal para restaurantes pequeños que desean iniciarse en la digitalización operativa con funciones esenciales.

- Monitoreo en tiempo real de temperatura y humedad en cámaras y vitrinas
- Alertas automáticas ante condiciones fuera de rango
- Reportes básicos semanales del estado de los dispositivos IoT
- Gestión sencilla de inventario (registro manual de productos y vencimientos)
- Soporte técnico en horario laboral


 **Plan Gestión Pro:**

Pensado para negocios que requieren mayor control, eficiencia operativa y soporte avanzado. Incluye todo lo del Plan Básico, más:

- Integración avanzada con sensores IoT adicionales (puertas, energía, etc.)
- Análisis automático de inventario (con predicciones de rotación y vencimiento)
- Notificaciones inteligentes para compras, caducidades y mantenimiento
- Informes personalizados de desempeño por sucursal
- Soporte técnico 24/7 y mantenimiento preventivo de hardware
### 1.2.1 Antecedentes y problemática

**Antecedentes:**


Estudios recientes han analizado los factores que impulsan el desperdicio de alimentos en restaurantes informales de gama media, diferenciado entre el desperdicio generado por el cliente y el generado en la cocina. Una investigación en destinos turísticos de Lituania (Morkunas et al, 2025), empleo entrevistas con gerentes y un Proceso Analítico Jerárquico (AHP) difuso para priorizar las causas, revelando hallazgos clave:

* Cliente: Destacaron el sentimiento de vergüenza, barrera lingüística, presentación inadecuada de platos tradicionales, tanto en destinos locales e internacionales.

* Cocina: Asociado a fallas en la planificación de demanda, ineficiencias operativas y limitaciones en infraestructura de almacenamiento.

Dicho estudio, propone soluciones adaptadas a cada factor identificado, ofreciendo un marco relevante para abordar problemáticas similares en contextos gastronómicos. 

**Problemáticas:**

La gestión del inventario de un restaurante suele llegar a consumir muchos recursos y tiempo. Además también es muy complicado estar al tanto de la fecha de vencimiento por producto, al igual que la temperatura idónea de los mismos. También cuando un restaurante tiene una gran cantidad de clientela se le suele dificultar a los mozos darse cuenta cuando un cliente requiere de atención.

**Técnica de The 5 'W's y 2 'H's**

**What?** <br>
El problema es la mala gestión del inventario en los restaurantes, lo que genera desperdicio de alimentos y un alto consumo de recursos debido al
vencimiento de productos y a la falta de control eficiente. Además, el personal de atención enfrenta dificultades para identificar cuándo un cliente requiere
asistencia, lo que puede afectar la calidad del servicio y la experiencia del cliente.

**When?** <br>
La problemática sucede en cualquier momento del día, ya que los restaurantes operan constantemente y deben gestionar su inventario y atención al
cliente en todo momento.

**Where?** <br>
La problemática ocurre en los restaurantes, tanto en la cocina como en el área de atención al cliente.

**Who?** <br>
Los dueños, gerentes y trabajadores de un restaurante son los principales afectados por esta problemática. La mala gestión del inventario impacta en su
rentabilidad y eficiencia operativa.

**Why?** <br>
La mala o dificultosa gestión de inventario en restaurantes se debe a la falta de herramientas adecuadas para monitorear y gestionar eficientemente el
inventario, así como a la falta de visibilidad y datos concretos sobre el estado de los productos.

**How?** <br>
KeepItFresh facilitará el proceso de gestión de inventario mediante el monitoreo de los mismos gracias a sus modernos sensores conectados a la app.

**How much?** <br>
KeepItFresh tendrá el alcance de resolver esta problemática a todo aquel restaurante que compre sus servicios.

### 1.2.2 Lean UX Process.

En esta sección, se presenta el proceso de Lean UX que se ha seguido para el desarrollo de la plataforma KeepItFresh. Este proceso incluye la creación de un Lean UX Problem Statement, Assumptions, Hypothesis Statements y un Lean UX Canvas. El objetivo es definir claramente el problema que se busca resolver, las suposiciones que se tienen sobre los usuarios y el producto, así como las hipótesis que guiarán el desarrollo del mismo.

#### 1.2.2.1. Lean UX Problem Statements.

En el entorno laboral actual, los restaurantes enfrentan dificultades para monitorear y gestionar su inventario de manera efectiva. Esto debido a la falta de herramientas adecuadas y el trabajo tedioso que esto suele ser, para hacerlo de forma continua y detallada. Lo cual da a una falta de visibilidad y datos concretos, lo cual lleva a gastos innecesarios con el inventario y posibilidad de descomposición de alimentos.<br>

El desafío que hay actualmente es que las soluciones actuales no proveen un precio accesible, al mismo tiempo que mantienen una alta calidad de servicio.<br>

¿Cómo podemos ofrecer a los restaurantes una plataforma con un precio accesible que al mismo tiempo ofrezca la calidad que estos necesitan?

#### 1.2.2.2. Lean UX Assumptions.

<ins>**Users Assumptions:**</ins>

1. **Creo que mis clientes necesitan** una herramienta fácil de usar para la gestión de inventarios, la cual facilite sus funciones, identificando problemas tales como posible descomposición, o niveles no óptimos para la temperatura.
2. **Estas necesidades se pueden resolver con** una aplicación web como KeepItFresh, la cual ofrece una mayor facilidad para la gestión de inventarios de calidad, aun manteniendo un precio accesible.
3. **Mis clientes iniciales son** restaurantes medianos, tales como restaurantes de comida criolla y pollerías. Las cuales tengan problemas de gestión de inventarios y requieran una solución de alta calidad, pero no se pueden permitir gastos grandes.
4. **El valor #1 que un cliente quiere de mi servicio es** la capacidad de gestionar fácilmente el inventario de los restaurantes mediante sensores IoT en tiempo real.
5. **El cliente también puede obtener estos beneficios adicionales,** esto ayuda a que todos los productos del inventario sean bien utilizados a tiempo y no se malogren. Así mismo también contamos con otro IoT que consta de un botón para llamar a los meseros para mejorar la atención al cliente en los restaurantes.
6. **Voy a adquirir la mayoría de mis clientes a través de estrategias de** marketing digital y recomendaciones entre empresas que valoren la facilidad en gestión que ofrecemos.
7. **Haré dinero a través de** un modelo de suscripción mensual o anual para los diferentes IoT, lo cual le da al cliente la posibilidad de alquilar la cantidad que él requiere basado en su poder adquisitivo.
8. **Mi competencia principal en el mercado serán** otras plataformas de gestión de inventarios tales como MarketMan y OpenTable.
9. **Los venceremos debido a** que ofrecemos un servicio de alta calidad manteniendo los precios accesibles ofreciendo todas las funciones de la aplicación web desde un inicio mientras el cliente cuente con el IoT.
10. **Mi mayor riesgo de producto es** que los restaurantes no adopten fácilmente la tecnología IoT por falta de conocimientos técnicos.
11. **Resolveremos esto a través de** un proceso de onboarding intuitivo, soporte técnico constante, tutoriales interactivos y demostraciones en vivo que permitan a los usuarios entender y aprovechar los beneficios de nuestro servicio sin necesidad de conocimientos técnicos avanzados.
12. **¿Qué otras suposiciones tenemos? ¿Eso, si se prueba que es falso, causará que nuestro negocio/proyecto no funcione?**

- Los clientes están dispuestos a confiar en la certeza de nuestros IoT para gestionar los inventarios. Si los encargados creen que estos nos tienen una total certeza, podríamos tener dificultades para atraer usuarios.
- Los restaurantes asignarán presupuesto para herramientas IoT que ayuden con la gestión del restaurante. Si estos creen que este tipo de servicios es un lujo y no algo necesario, la propuesta que ofrecemos va a dejar de ser de valor para ellos.

**¿Quién es el usuario?**<br>

Dueños de restaurantes y meseros.

**¿Dónde encaja nuestro producto en su trabajo o vida?**<br>

Nuestro producto encaja en el trabajo diario de los usuarios, proporcionando herramientas útiles para la gestión de sus inventarios con el fin de facilitar su trabajo, así mismo facilita el trabajo de los meseros al recibir las llamadas de los clientes con una mayor facilidad.

**¿Qué problemas tiene nuestro producto y cómo se pueden resolver?**<br>

KeepItFresh puede enfrentar problemas tales como la falta de familiaridad de los usuarios con tecnologías IoT, desconfianza de la precisión de los sensores y la adaptación a diversos tipos de restaurantes. Para resolver estos problemas, se puede implementar un proceso de onboarding claro con tutoriales visuales y ofrecer un soporte técnico constante.

**¿Cuándo y cómo se usa el producto?**<br>

El producto se utilizará de manera diaria durante las horas operativas del restaurante, tanto en la gestión del inventario como la mejora de atención al cliente. Se accede a través de una aplicación web compatible con computadoras, tablets o smartphones, permitiendo el monitoreo en tiempo real. Además, durante el servicio, los meseros van a recibir notificaciones mediantes los botones IoT colocados en las mesas, lo que agiliza la atención al cliente y mejora su eficiencia en el trabajo.

**¿Qué características son importantes?**<br>


Entre las características más importantes de KeepItFresh se encuentra el monitoreo en tiempo real de sensores IoT, un panel de control intuitivo y visualmente claro, la integración sencilla con múltiples dispositivos y sensores, y la escalabilidad del servicio para adaptarse al crecimiento del restaurante.


**¿Cómo debe verse nuestro producto y cómo debe comportarse?**<br>
KeepItFresh debe tener un diseño visual moderno, limpio y profesional, con una paleta de colores que transmita frescura y confianza. La interfaz debe ser intuitiva, con una navegación fluida y amigable que permita al usuario encontrar con facilidad la información que necesita. Debe comportarse de forma estable y responsive, adaptándose sin dificultad a distintos tamaños de pantallas y dispositivos. La información debe de presentarse de forma clara, utilizando elementos como gráficos, iconos y colores para facilitar la interpretación de los datos.

<ins>**Business Outcomes:**</ins>
1. Al desarrollar KeepItFresh, prevemos un aumento en la cantidad de restaurantes con afinidad a nuestra plataforma, lo cual incrementará nuestras ventas y nos posicionará como una solución confiable en el mercado.
2. Generación de ingresos constantes y predecibles mediante el modelo de suscripción mensual o anual, lo cual facilita la proyección financiera a largo plazo.
3. Expansión del negocio hacia nuevos mercados y segmentos, como cadenas de restaurantes o franquicias, gracias a la escalabilidad de nuestro servicio.

<ins>**User Outcomes:**</ins>

1. Los usuarios podrán monitorear el estado de su inventario en tiempo real, lo que les permitirá tomar decisiones informadas y reducir el desperdicio de alimentos.
2. Los dueños de restaurantes tendrán una mayor tranquilidad al saber que los productos están siendo almacenados adecuadamente, minimizando pérdidas económicas.
3. La experiencia del cliente en el restaurante va a mejorar gracias al botón de llamado a meseros, agilizando la atención al cliente.

<ins>**Features:**</ins>

- Monitoreo en tiempo real de sensores IoT.
- Panel de control centralizado e intuitivo con una fácil navegación.
- Botón IoT para llamado de meseros que mejora la experiencia del cliente.
- Alertas automáticas cuando las condiciones del inventario están fuera del rango óptimo.
- Registro y consulta de inventario detallado
- Historial de alertas
- Medición del tiempo de respuesta de atencion al cliente
- Gestión de suscripcion y facturación
- Flujo de recepción y almacenamiento de inventario por el personal

#### 1.2.2.3. Lean UX Hypothesis Statements.

1. Hipótesis 1: Creemos que al implementar el monitoreo continuo y en tiempo real del estado del inventario mediante sensores IoT, los dueños de restaurantes podrán tomar decisiones más informadas sobre el inventario, lo cual reducirá el desperdicio de alimentos y las pérdidas.

2. Hipótesis 2: Creemos que al ofrecer un panel de control centralizado e intuitivo con fácil navegación para dueños y personal, la plataforma será fácil de usar y mejorará la eficiencia general en la gestión de inventario y alertas.

3. Hipótesis 3: Creemos que al facilitar la atención al cliente mediante un botón IoT de llamado a meseros, los comensales solicitarán atención más fácilmente, lo cual disminuirá los tiempos de espera y generará una mejora en la experiencia y percepción del servicio por parte de los comensales.

4. Hipótesis 4: Creemos que al enviar alertas automáticas cuando las condiciones del inventario están fuera del rango óptimo, los dueños y el personal podrán reaccionar a tiempo ante condiciones críticas, lo cual prevenirá la descomposición y reducirá las pérdidas económicas.

5. Hipótesis 5: Creemos que al permitir a los dueños registrar y consultar inventario detallado (incluyendo vencimiento y condiciones de almacenamiento), tendrán mejor control sobre su stock y facilitarán una gestión más organizada del inventario.

6. Hipótesis 6: Creemos que al proporcionar a los dueños un historial de alertas pasadas, podrán entender los incidentes ocurridos en ciertos días, lo cual les permitirá mejorar la planificación y toma de decisiones futuras para prevenir problemas recurrentes.

7. Hipótesis 7: Creemos que al permitir a los administradores medir cuánto tiempo tarda el personal en atender una solicitud, podrán evaluar la eficiencia del servicio, lo cual contribuirá al objetivo de disminuir los tiempos de espera.

8. Hipótesis 8: Creemos que al implementar un sistema de gestión de suscripción y facturación, generaremos un flujo de ingresos seguro y predecible para ClearView, mientras los dueños gestionan de forma transparente su alquiler de servicio.

9. Hipótesis 9: Creemos que al proporcionar un flujo específico para que el personal registre y almacene inventario entrante, el proceso de actualización de stock será más eficiente y preciso para los trabajadores, lo cual reducirá su carga de trabajo y asegurará registros exactos en el sistema.

#### 1.2.2.4. Lean UX Canvas.

<img src="/assets/chapter1/Lean UX canvas.png" alt="LeanUXCanvas">

## 1.3. Segmentos objetivos.



### Segmento objetivo #1: Dueños de restaurantes

**Descripción:**  
Este segmento está compuesto por propietarios de restaurantes de tamaño pequeño y mediano que buscan optimizar la gestión operativa de sus negocios, especialmente en lo relacionado al control de inventario y la reducción del desperdicio de alimentos.

**Aspectos demográficos:**  
Este grupo está compuesto mayoritariamente por hombres y mujeres de entre 30 y 55 años, con un nivel socioeconómico medio-alto (B) y medio (C). En su mayoría, cuentan con educación técnica o universitaria, especialmente en áreas de administración, negocios o gastronomía.

**Aspectos geográficos:**  
Son peruanos que operan principalmente en zonas urbanas, con un enfoque particular en Lima, Arequipa, Trujillo y otras ciudades con una fuerte actividad gastronómica.

**Aspectos psicográficos:**  
Valoran la eficiencia operativa, el control de gastos y la sostenibilidad. Son empresarios orientados a resultados, que buscan innovar y mantenerse competitivos en un mercado gastronómico cada vez más demandante.

**Necesidades:**  
Desean automatizar el control del inventario para evitar pérdidas por caducidad o mal almacenamiento, tener acceso a reportes claros en tiempo real, y recibir alertas sobre productos próximos a vencer.

**Requisitos:**  
Buscan una plataforma intuitiva, confiable y adaptable al flujo de trabajo del restaurante. Requieren acceso desde dispositivos móviles y soporte técnico constante.

**Objetivo:**  
Reducir el desperdicio de alimentos, mejorar la rentabilidad del restaurante y tomar decisiones estratégicas basadas en datos precisos.

**Sustento estadístico:**  
Según el Ministerio de la Producción del Perú (Produce, 2023), existen más de 220,000 restaurantes registrados en el país, de los cuales cerca del 85% corresponden a pequeñas y medianas empresas. Lima concentra aproximadamente el 40% del total de estos negocios. Además, estudios del Banco Interamericano de Desarrollo señalan que en América Latina, hasta el 34% de los alimentos en restaurantes se desperdician por una mala gestión de inventario.

 

### Segmento objetivo #2: Trabajadores de restaurantes

**Descripción:**  
Este segmento incluye cocineros, meseros y personal operativo de restaurantes, quienes desempeñan funciones clave en la atención al cliente y la administración diaria del inventario.

**Aspectos demográficos:**  
Está compuesto mayormente por hombres y mujeres de entre 20 y 35 años, pertenecientes a clases sociales C y D. Tienen formación técnica en gastronomía, atención al cliente o educación secundaria completa.

**Aspectos geográficos:**  
Este grupo está ubicado principalmente en zonas urbanas, específicamente en Lima, Callao y otras ciudades principales del país con una fuerte presencia de restaurantes.

**Aspectos psicográficos:**  
Valoran herramientas que faciliten su trabajo diario y les permitan brindar una mejor experiencia al cliente. Son personas prácticas que aprecian la tecnología cuando es fácil de usar y útil en su entorno laboral.

**Necesidades:**  
Necesitan una forma rápida y clara de gestionar los productos disponibles en cocina, identificar faltantes y vencimientos, y mejorar la coordinación con el equipo. También buscan mejorar la atención en sala mediante herramientas como botones IoT que agilicen el servicio.

**Requisitos:**  
Requieren una plataforma sencilla, rápida y accesible desde celulares o tablets. Valoran la facilidad de uso, el idioma claro y una curva de aprendizaje corta.

**Objetivo:**  
Facilitar su labor diaria, reducir errores humanos en el manejo de productos y mejorar la eficiencia en la atención al cliente.

**Sustento estadístico:**  
De acuerdo con el Instituto Nacional de Estadística e Informática (INE
