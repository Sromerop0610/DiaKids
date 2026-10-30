# Propuesta de proyecto · DiaKids (Estudio Optativa)

**Integrantes:** Dayron Torres Yegua, Abel Suazo Cabeza de Vaca, Jesús Gallardo Domínguez, Sara Romero Pérez  
**Fecha de entrega:** 25 de octubre de 2026  

## Índice

0. [Introducción](#introducción)
1. [El problema](#1.-el-problema)
2. [Viabilidad técnica](#2-viabilidad-técnica)
3. [Objetivos y alcance](#3-objetivos-y-alcance)
4. [Recursos](#4-recursos)

## Introducción

La idea de proyecto es una aplicación para la diabetes adaptada para niños.


Las aplicaciones para la gestión de la diabetes (el calculo de bolos y el registro de la azucar) es muy rudimentaria, es una aplicación muy básica y mecánica, y con una forma de manejar los datos que los niños más pequeños tardan en entender.


Mi propuesta es una aplicación de gestión de la diabetes adaptada a niños, que permita registrar los niveles de glucosa, consultar información y realizar cálculos relacionados con la administración de insulina mediante una interfaz visual, sencilla y comprensible.


La aplicación estaría vinculada a la cuenta, en la misma, de un adulto. Donde el adulto pudiese comprobar los datos e introducirlos también.

---

## 1. El problema

#### Necesidad:

El problema a resolver es la robustez y falta de accesibilidad de las aplicaciones ya existentes para el seguimiento del estado de la diabetes en niños pequeños.

Afecta tanto a los niños como a los padres, ya que además de ser algo realmente importante para la salud, también es un suplicio para los padres el estar constantemente atentos a dichas aplicaciones sin siquiera dar oportunidad a sus hijos de ayudarles o enseñarles cómo utilizarlas.

La frecuencia de este problema es diaria, ya que es una enfermedad crónica que necesita un seguimiento y una atención diaria.

El impacto sería clave para que los pequeños empiecen a entender cómo gestionar y seguir sus datos, de manera que cuando se vayan haciendo mayores no se les haga un mundo aprender a utilizar dichas aplicaciones tan robustas. Además de que para los padres sería un gran alivio ver cómo sus hijos evolucionan y cada vez son más capaces de lidiar con dicho problema por cuenta propia.


#### Users persona:
Tendremos dos perfiles de distintas edades.
##### El primero: Hermana de Sara - 12 años
- Necesidades: Tener un registro de sus niveles de glucosa, una calculadora de bolos que le diga la insulina que necesita administrarse y desarrollar un habito de autocuidado porque tiende a desantenderse del problema.
- Frustraciones: Dificultad de entendimiento de las aplicaciones actuales del mercado, información no accesible para personas mas pequeñas.
- Objetivos: Poder sobrellevar la enfermedad de una forma mas sencilla y asequible para alguien de su edad.
- Caso de uso:
  - Registra su glucosa y gana recompensas: Introduce su nivel de azúcar (manualmente o por conexión con el glucómetro) y la app lo premia con puntos o avances en su avatar para que no sea una tarea aburrida.
  - Calcula su insulina con dibujos: Usa una calculadora visual donde selecciona qué va a comer mediante iconos (ej. una manzana, un bocadillo) en lugar de lidiar con fórmulas matemáticas o gramos complejos, obteniendo la dosis exacta para su pluma.
  - Responde a recordatorios lúdicos: Recibe avisos amigables de la app (como si fuera una mascota o un amigo) cuando le toca medirse, lo que le ayuda a acordarse sin sentir que la están regañando.

##### Segunda: Madre de Sara - 47 años 
- Necesidad: Controlar el nivel de glucosa de su hija y tener registro de ello diario, asegurarse que su hija aprenda a sobrellevar la enfermedad sin un control constante.
- Frustraciones: Su hija no es constante con el seguimiento de la enfermedad y ademas al ser pequeña se le olvida calcular ciertas cosas, tener que estar pendiente las 24 horas del día (desatendiendo responsabilidades propias), al no ser una persona que entienda las nuevas tecnologías y no saber nada de la diabetes previamente, le cuesta ayudar a su hija.
- Objetivos: Seguimiento mas fácil para la enfermedad de su hija y que aprenda de una forma mas didácticas.
- Caso de uso:
  - Visualiza el estado de su hija de un vistazo: Abre su panel de control y ve mediante colores sencillos (verde, amarillo, rojo) si su hija está bien en ese momento, sin necesidad de entender gráficos médicos complicados.
  - Recibe avisos con "instrucciones de emergencia": Si la glucosa de la niña se descontrola o se salta un registro, recibe una alerta acompañada de una guía rápida y clara sobre qué pasos dar en ese preciso instante.
  - Consulta informes de autonomía: Revisa un resumen semanal en formato infografía para comprobar si su hija va aprendiendo a cuidarse sola, lo que le permite soltar el control poco a poco con tranquilidad.

#### Competencia:

- Mysugr
    - Tiene tanto calculadora como interfaz para gestion, la calculadora usa datos como la glucosa actual, carbohidratos, ratio insulina/carbohidratos, factor de correccion e insulina activa. Esta tambien permite configurar parametros dependientes del horario y un registro de glucosa.

- Diabetes-m
    - Permite calcular la insulina utilizando carbohidratos, grasas, proteinas y glucosa medida tambien contemplando insulina activca, bolus extendido, correcion por actividad física, correcion por enfermedad, objetivo de glucosa, ratio insulina/carbohidratos y base de datos de alimentos

- One touch
    - Es una calculadora que lo que hace es automatizar el cálculo de bolos utilizando factores como pueden ser la glusoca actual, glucosa objetivo, carbohidratos, ratio insulina/carbohidratos, sensibilidad a la insulina, duracion de la accion de la insulina e insulina que permanece activa

- El problema principal de las tres es que estan pensadas para un enfoque mas adulto por lo que los niños tienen mayor dificultad para usarlas

#### Propuesta de valor:
Nuestra propuesta consiste en desarrollar una aplicación para la gestión de la diabetes específicamente adaptada a niños, que facilite la comprensión y el manejo de la enfermedad mediante una interfaz sencilla, visual e intuitiva.

La aplicación contará con **dos tipos de perfiles: niños y padres o tutores**, cada uno con diferentes permisos y funcionalidades.

El **perfil del niño** estará diseñado para que pueda utilizar la aplicación de forma sencilla y segura. Podrá introducir sus niveles de glucosa, registrar información relacionada con sus comidas y utilizar la calculadora de bolos introduciendo los datos necesarios para realizar el cálculo. Sin embargo, **no tendrá permisos para modificar los parámetros de la calculadora**, evitando que pueda cambiar accidentalmente valores establecidos previamente.

El **perfil de padres o tutores** tendrá mayores permisos de gestión. Desde este perfil podrán **configurar y modificar los parámetros utilizados por la calculadora**, supervisar los registros de glucosa y otros datos introducidos por el niño, consultar su evolución y gestionar la información de su perfil. De esta forma, los adultos podrán mantener el control sobre aquellos aspectos que requieren una mayor responsabilidad, mientras que el niño podrá participar progresivamente en su propia gestión de una manera adaptada a su edad.

La aplicación también contará con un **apartado de información dividido en diferentes temas**, para que el niño pueda aprender sobre la diabetes de forma progresiva y organizada. Estos temas podrán abordar aspectos como la glucosa, la insulina, la alimentación, el ejercicio físico o diferentes situaciones relacionadas con la diabetes.

Para hacer que el aprendizaje sea más atractivo, cada tema incluirá un **juego o cuestionario interactivo** relacionado con los contenidos aprendidos. Al completarlos, el niño podrá obtener puntos y experiencia para hacer progresar a su personaje dentro de la aplicación.

La gamificación también estará integrada en las tareas habituales de gestión de la diabetes. El niño podrá conseguir puntos por **registrar sus niveles de glucosa, introducir sus comidas, utilizar las diferentes funciones de la aplicación y mantener sus registros actualizados**. Estos puntos permitirán que su personaje gane experiencia y **suba de nivel**, pudiendo desbloquear progresivamente nuevos elementos o recompensas.

El objetivo de este sistema no será premiar al niño por tener determinados niveles de glucosa, sino **incentivar aquellas acciones que sí puede controlar**, como registrar sus datos, aprender sobre su enfermedad y mantener un seguimiento constante. De esta manera, se pretende que la aplicación no solo facilite la gestión diaria de la diabetes, sino que también motive al niño a **seguir aprendiendo sobre su condición y desarrollar progresivamente un hábito de autocuidado y seguimiento**.

En conjunto, la aplicación busca transformar una herramienta de gestión de la diabetes que puede resultar técnica, repetitiva y poco intuitiva en una experiencia **más accesible, educativa, interactiva y adaptada a los niños**, proporcionando al mismo tiempo a los padres o tutores las herramientas necesarias para supervisar y configurar aquellos aspectos que requieren una mayor responsabilidad.

---

## 2. Viabilidad técnica

### REQUISITOS FUNCIONALES

#### MUST:
- El niño podrá iniciar sesión en su perfil.
- El padre, madre o tutor podrá iniciar sesión en su perfil.
- El adulto podrá crear y configurar el perfil del niño.
- El padre, madre o tutor podrá enlazar su perfil con el del niño.
- El padre/madre/tutor podrá modificar los parámetros usados por la calculadora.
- El niño puede registrar sus niveles de glucosa.
- El niño podrá registrar sus comidas y los datos nutricionales necesarios para el cálculo.
- El niño puede calcular su insulina.
- El padre/madre/tutor podrá enlazar su perfil con el de su hijo/a.

#### SHOULD:
- El niño recibe alertas para medir su glucosa.
- El niño podrá consultar su historial de registros de glucosa.
- El padre/madre/tutor podrá personalizar las horas habituales de recordatorio.
- El padre/madre/tutor podrá revisar los registros de glucosa del niño.
- El padre/madre/tutor recibe alertas para registrar la glucosa de su hijo/a.
- El padre/madre/tutor recibe informes semanales de autonomía de su hijo/a.

#### COULD:
- El niño/a tendrá contenido didáctico para aumentar sus conocimientos sobre su condición concreta (aprendizaje progresivo y organizado).
- Cada tema tendrá un juego o cuestionario interactivo para que el niño/a pueda aprender sobre la diabetes de forma progresiva y organizada.

#### WON'T:
- El niño/a tendrá un personaje con podrá ir subiendo de nivel con el tiempo si va realizando las tareas de gestión de la diabetes.

#### RECORRIDO MÍNIMO DEL USUARIO:

| PADRE | HIJO/A |
| :--- | :--- |
| Registro/inicio de sesión | Registro/inicio de sesión |
| Vincular perfiles | Vincular perfiles |
| Dashboard principal (opciones de nuevo registro / calculadora) | Dashboard principal (opciones de nuevo registro / calculadora) |
| Configuración de parámetros | |
| | Registro de glucosa |
| | Calculadora Visual |
| | Resultado de bolus (Muestra la dosis exacta) |
| | Confirmación (Guardar registro en el historial) |
| Consulta del historial y registros guardados del menor | |


### REQUISITOS TÉCNICOS
#### FRONTEND (React)

El frontend será la parte de la aplicación con la que interactuarán los niños y sus padres o tutores. Se desarrollará con React y se añadirán bibliotecas que faciliten la navegación, la comunicación con el backend y el diseño de la interfaz.

Hemos pensado en usar:

| Biblioteca | ¿Para qué la usaremos? | ¿Qué hace? |
| --- | --- | --- |
| **React Router** | Gestionar las páginas de la aplicación: inicio de sesión, perfil infantil, panel de padres y registros. | Permite navegar entre páginas sin recargar toda la aplicación. |
| **TanStack Query** | Consultar, guardar y actualizar datos obtenidos del backend, como los registros de glucosa. | Facilita la gestión de las peticiones, los estados de carga y los errores. |
| **Tailwind CSS** | Diseñar botones, formularios, paneles y tarjetas adaptables a distintos tamaños de pantalla. | Permite crear una interfaz visual y personalizable sin escribir demasiado CSS repetitivo. |
| **Recharts** | Representar gráficamente el historial de glucosa y su evolución. | Facilita la creación de gráficos para que los padres puedan interpretar los registros de forma visual. |

#### INFRAESTRUCTURA

Proponemos separar el frontend, el backend y la base de datos. De esta manera, cada parte podrá desplegarse y actualizarse de forma independiente.

##### Servicios elegidos y sus condiciones gratuitas

| **Servicio** | **Uso** | **Condiciones del plan gratuito** |
| --- | --- | --- |
| **Vercel Hobby** | Desplegar el frontend de React. | Incluye alojamiento para proyectos personales, con límites de uso. Entre sus cuotas publicadas están 1 millón de invocaciones de funciones y 100.000 lecturas de Edge Config por periodo de facturación, si se utilizan esas funciones. |
| **Render Free** | Ejecutar la API de Express. | Dispone de 750 horas de instancia gratuitas por espacio de trabajo y mes. El servicio se suspende tras 15 minutos sin tráfico entrante y tarda aproximadamente un minuto en volver a arrancar al recibir una petición. |
| **MongoDB Atlas Free** | Alojar la base de datos MongoDB. | Ofrece 512 MB de almacenamiento. El clúster gratuito tiene límites de rendimiento y no incluye las copias de seguridad gestionadas disponibles en planes superiores. |

Los planes y sus condiciones pueden cambiar, así que conviene volver a comprobarlos antes de desplegar el proyecto.

No necesitamos contratar un servidor propio para la primera versión. Vercel, Render y MongoDB Atlas cubren el alojamiento de la interfaz, la ejecución del backend y el almacenamiento de los datos.

Sí necesitaremos configurar algunas medidas adicionales:

* Variables de entorno para guardar la cadena de conexión de MongoDB y las claves secretas del backend.
* Conexiones HTTPS para proteger la comunicación.
* Restricciones de acceso a MongoDB para que solo los servicios autorizados puedan conectarse.
* Validación de las peticiones y comprobación de permisos en el backend.
* Una política de copias de seguridad y recuperación antes de considerar el uso de datos reales.

El principal inconveniente de Render Free es que el backend puede tardar en responder cuando vuelve a arrancar tras un periodo de inactividad. Para una demostración en clase es asumible, pero debe tenerse en cuenta.

### Requisitos técnicos: backend y base de datos
#### Backend(Node.js + express)
##### 1. Autenticación y Roles

La aplicación implementa un sistema de autenticación con control de acceso basado en roles (**RBAC**):

* **Niño:** Puede registrar sus datos diarios (glucosa, comidas), consultar su historial y acceder al contenido didáctico.
* **Adulto (Padre / Tutor):** Puede crear o vincular perfiles infantiles, consultar los registros del menor y configurar los parámetros médicos de la calculadora.

El backend verifica la autenticación, el rol del usuario y su relación con el perfil infantil antes de procesar cada petición protegida.

##### Stack de Seguridad
* **JWT (JSON Web Token):** Gestión de sesiones sin estado.
* **bcrypt:** Encriptación de contraseñas mediante hashing.
* **Express Middlewares:** Validación de token, roles y permisos en cada endpoint.
* **Seguridad en Tokens:** En el caso de usar cookies, se configurarán con las directivas `HttpOnly`, `Secure` y `SameSite`.

---

##### 2. APIs Principales (Endpoints)

| Grupo | Ruta (Ejemplo) | Función |
| :--- | :--- | :--- |
| **Autenticación** | `POST /api/auth/register`<br>`POST /api/auth/login` | Registro de adultos e inicio de sesión. |
| **Perfiles** | `GET /api/profiles/me`<br>`POST /api/profiles/children` | Consulta de perfil propio y creación de perfiles infantiles. |
| **Vinculación** | `POST /api/guardians/link` | Enlace entre un perfil adulto y un perfil infantil. |
| **Glucosa** | `POST /api/glucose`<br>`GET /api/glucose` | Registro y consulta del historial de glucosa según permisos. |
| **Comidas** | `POST /api/meals`<br>`GET /api/meals` | Registro y consulta de comidas e hidratos. |
| **Calculadora** | `GET /api/calculator/settings`<br>`PUT /api/calculator/settings` | Consulta (Niño/Adulto) o modificación (Solo Adulto) de parámetros. |
| **Recordatorios** | `GET /api/reminders`<br>`PUT /api/reminders` | Consulta y configuración de horarios de alertas. |

---

##### 3. APIs y Servicios Externos

Para acotar el alcance de la versión inicial y reducir la complejidad, se limita la dependencia de servicios de terceros:

| Servicio Externo | Uso Previsto | Límite Gratuito |
| :--- | :--- | :--- |
| **Sensores / Bombas de insulina** | **No se integra.** Registro 100% manual. | N/A |
| **Servicio de Email / Push / SMS** | **No se utiliza inicialmente.** Alertas in-app. | N/A |
| **Base de Datos (MongoDB Atlas)** | Persistencia de usuarios, registros y configuraciones. | Según plan M0 (512 MB gratis). |

#### Base de datos (MongoDB)
Utilizaremos **MongoDB Atlas** (NoSQL) para almacenar los usuarios, perfiles infantiles, registros y configuraciones de la aplicación en documentos BSON organizados en colecciones.

---

##### Colecciones Principales

###### 1. `users`
Almacena los datos de autenticación y el rol de cada usuario registrado.

| Campo | Tipo | Descripción |
| :--- | :--- | :--- |
| `_id` | `ObjectId` | Identificador único del usuario. |
| `name` | `String` | Nombre del usuario. |
| `email` | `String` | Correo electrónico para iniciar sesión (único). |
| `passwordHash` | `String` | Hash de la contraseña (generado con `bcrypt`). |
| `role` | `String` | Rol del usuario (`child` o `guardian`). |
| `createdAt` | `Date` | Fecha de creación de la cuenta. |

---

###### 2. `childProfiles`
Contiene la información específica del perfil infantil, separada de las credenciales de acceso.

| Campo | Tipo | Descripción |
| :--- | :--- | :--- |
| `_id` | `ObjectId` | Identificador del perfil infantil. |
| `userId` | `ObjectId` | Referencia al usuario correspondiente en `users`. |
| `guardianIds` | `Array<ObjectId>` | Referencias a los usuarios adultos autorizados (`users`). |
| `nickname` | `String` | Nombre o apodo mostrado dentro de la app. |
| `birthDate` | `Date` | Fecha de nacimiento. |
| `createdAt` | `Date` | Fecha de creación del perfil. |

---

###### 3. `glucoseRecords`
Registra las lecturas de glucosa introducidas por el niño.

| Campo | Tipo | Descripción |
| :--- | :--- | :--- |
| `_id` | `ObjectId` | Identificador único del registro. |
| `childId` | `ObjectId` | Referencia al perfil infantil en `childProfiles`. |
| `value` | `Number` | Valor de la glucosa medida (ej. 110). |
| `unit` | `String` | Unidad de medida (ej. `mg/dL`). |
| `measuredAt` | `Date` | Fecha y hora en que se realizó la medición. |
| `createdAt` | `Date` | Fecha de creación del registro en el sistema. |

---

###### 4. `meals`
Almacena las comidas e hidratos de carbono registrados por el menor.

| Campo | Tipo | Descripción |
| :--- | :--- | :--- |
| `_id` | `ObjectId` | Identificador de la comida. |
| `childId` | `ObjectId` | Referencia al perfil infantil en `childProfiles`. |
| `description` | `String` | Descripción de la comida (ej. manzana, bocadillo). |
| `carbohydrates` | `Number` | Cantidad estimada de carbohidratos (en gramos). |
| `consumedAt` | `Date` | Fecha y hora de consumo. |
| `createdAt` | `Date` | Fecha de registro en el sistema. |

---

###### 5. `calculatorSettings`
Guarda los parámetros de la calculadora configurados exclusivamente por los tutores.

| Campo | Tipo | Descripción |
| :--- | :--- | :--- |
| `_id` | `ObjectId` | Identificador de la configuración. |
| `childId` | `ObjectId` | Referencia al perfil infantil en `childProfiles`. |
| `parameters` | `Object` | Objeto con parámetros educativos para la simulación (ratios, FCF, etc.). |
| `updatedBy` | `ObjectId` | Referencia al usuario adulto (`users`) que hizo la modificación. |
| `updatedAt` | `Date` | Fecha de la última actualización. |

---

###### 6. `reminders`
Almacena las preferencias y alertas de recordatorio personalizadas.

| Campo | Tipo | Descripción |
| :--- | :--- | :--- |
| `_id` | `ObjectId` | Identificador del recordatorio. |
| `childId` | `ObjectId` | Referencia al perfil infantil en `childProfiles`. |
| `createdBy` | `ObjectId` | Referencia al usuario adulto (`users`) que lo creó. |
| `time` | `String` | Hora programada (ej. `"08:00"`, `"14:30"`). |
| `daysOfWeek` | `Array<Number>` | Días activos (`1` = Lunes, `7` = Domingo). |
| `enabled` | `Boolean` | Estado del recordatorio (`true` / `false`). |

### 3- Evaluación de capacidades del equipo

#### Inventario de habilidades
* **O** Sí
* **X** No
* **-** Más o menos

| Nombres | React | Node + express | MongoDB | Git |
| :--- | :---: | :---: | :---: | :---: |
| Dayron | X | - | O | O |
| Abel | X | X | - | O |
| Jesús | X | X | - | O |
| Sara | - | - | - | O |

#### ¿Qué necesitaréis aprender?
Tras valorar en conjunto las habilidades de cada miembro, notamos la falta de habilidad en el ámbito de React y de Node + express a nivel general. Vamos a necesitar nutrirnos más en ese área para hacer un mejor proyecto.

---

### 4- Identificación de riesgos técnicos

1. **Falta de tiempo y disponibilidad por sobrecarga académica/laboral.**
   * **Estrategia de mitigación:** Encontrar una manera óptima de mantener al equipo informado sobre la disponibilidad que tendremos cada integrante semanalmente, con la finalidad de encontrar un equilibrio entre todos acorde al tiempo disponible de cada uno. En nuestro caso, creamos un canal en nuestro servidor de Discord `#disponibilidad` para informar al equipo en caso de encontrar algún inconveniente.

2. **Curva de aprendizaje y falta de conocimiento en las tecnologías aplicadas.**
   * **Estrategia de mitigación:** En nuestro caso, ninguno de los integrantes del equipo está realmente familiarizado ni tiene una base contundente en ninguna de las tecnologías que se nos exige utilizar, por lo que una buena estrategia de mitigación sería poner un esfuerzo extra individualmente para aprender lo más rápido posible a utilizar las tecnologías exigidas y disminuir dicho riesgo/miedo lo máximo posible.

3. **Sobreestima del alcance del proyecto en relación al tiempo disponible.**
   * **Estrategia de mitigación:** De primera mano y a la hora de proponer la idea, es fácil proponer ideas y funcionalidades para el proyecto, pero no siempre es posible llevarlo todo a cabo. Para que esto no ocurra, lo que podríamos hacer es un ajuste cada cierto tiempo para evaluar qué funcionalidades creemos que sí que podremos implementar y cuáles no, basándonos en el sistema de prioridad propuesto.

4. **Mala comunicación y cuellos de botella en la toma de decisiones.**
   * **Estrategia de mitigación:** Designar un portavoz/líder de proyecto por sprint que centralice la toma de decisiones técnicas rápidas cuando haya desacuerdos, y mantener el tablero del proyecto actualizado.

5. **Desigualdad en la carga de trabajo o desmotivación de algún integrante.**
   * **Estrategia de mitigación:** Descomponer el trabajo en tareas acordes al tiempo disponible de cada uno según la semana (estimadas en un máximo de 2 a 4 horas de desarrollo cada una). Se realizará una revisión breve de estado por semana para detectar bloqueos a tiempo y poder reasignar o ayudar con ciertas tareas de forma equilibrada entre los miembros del equipo.

6. **Exposición accidental de credenciales o datos sensibles de salud.**
   * **Estrategia de mitigación:** Proteger todas las rutas del servidor mediante token/sesión desde su creación y utilizar archivos de variables de entorno (`.env`), los cuales se incluirán obligatoriamente en el archivo `.gitignore` desde el primer commit para evitar subir contraseñas o claves secretas a GitHub.

---

## 3. Objetivos y alcance

### Introducción

Este documento detalla los objetivos, el alcance y las líneas maestras de desarrollo para una aplicación web orientada al seguimiento y aprendizaje de la diabetes tipo 1 en niños, facilitando su autocuidado y la supervisión por parte de sus tutores.

El proyecto se estructura en torno a los siguientes puntos clave:

* **Objetivos SMART y validación:** Medición de la usabilidad y la seguridad mediante pruebas con un grupo de 8 usuarios (4 niños y 4 tutores). Se evaluará la autonomía del menor al registrar la glucosa, su aprendizaje educativo, la agilidad del tutor para consultar el historial y el control estricto de permisos.
* **Estrategia de plataforma (*Mobile-First*):** Diseño optimizado para smartphones para el uso cotidiano de niños y tutores, con soporte secundario en escritorio/tablet para la revisión detallada de gráficos y configuración.
* **Alcance del MVP y límites:** Centrado en el registro manual, la visualización de alimentos y el cálculo seguro de bolus. Se excluyen la integración con sensores de glucosa (CGM), las notificaciones push externas, las apps nativas y la emisión de diagnósticos médicos.
* **Evolución futura:** Planificación de mejoras posteriores como soporte *offline* (PWA), alertas en tiempo real, gamificación con avatar y minijuegos educativos.

### 1. Objetivos
#### Objetivo general
Desarrollar una aplicación web accesible, visual e intuitiva para facilitar a los niños con diabetes el seguimiento de su enfermedad y el aprendizaje de hábitos de autocuidado, favoreciendo su autonomía y permitiendo a sus padres o tutores supervisar su evolución.

#### Objetivos específicos

| ID | Objetivo SMART | Qué se mide | Valor de éxito | Cómo se comprueba |
|---|---|---|---|---|
| OE1 | Conseguir que, antes de la defensa final, al menos el 75 % de los niños participantes registre correctamente un nivel de glucosa en menos de dos minutos y sin ayuda de un adulto. | Porcentaje de participantes que completan correctamente el registro y tiempo empleado. | Al menos el 75 % completa la tarea en menos de 120 segundos sin ayuda. | Prueba de usabilidad con un mínimo de cuatro participantes del perfil infantil, utilizando datos ficticios. Se registrarán los tiempos y la necesidad de ayuda antes de la defensa final. |
| OE2 | Conseguir que, antes de la defensa final, al menos el 75 % de los niños participantes obtenga una puntuación mínima del 60 % en un cuestionario sobre los contenidos educativos de la aplicación. | Porcentaje de participantes que alcanza la puntuación mínima en el cuestionario. | Al menos el 75 % de los participantes responde correctamente a un mínimo de 3 de las 5 preguntas. | Se realizará un cuestionario de cinco preguntas sobre los contenidos educativos de la aplicación, como la glucosa, la alimentación, la insulina o el ejercicio físico. Se comprobarán los resultados antes de la defensa final. |
| OE3 | Conseguir que, antes de la defensa final, al menos el 75 % de los adultos participantes consulte los últimos registros de glucosa de su hijo e identifique correctamente la información mostrada en menos de 90 segundos. | Porcentaje de adultos que localiza e interpreta correctamente la información y tiempo empleado. | Al menos el 75 % completa la tarea correctamente en menos de 90 segundos. | Prueba de usabilidad con un mínimo de cuatro adultos que representen el perfil de padres o tutores, utilizando registros ficticios. Se registrarán los tiempos, los aciertos y la necesidad de ayuda. |
| OE4 | Conseguir que, antes de la defensa final, todas las pruebas funcionales de permisos confirmen que los niños no pueden modificar los parámetros de la calculadora de insulina y que los tutores autorizados sí pueden gestionarlos. | Funcionamiento de los permisos y existencia de accesos o modificaciones no autorizados. | El 100 % de los casos de prueba definidos se resuelve correctamente. | Se realizarán pruebas funcionales con cuentas de niño y de tutor, intentando acceder y modificar los parámetros desde ambos perfiles. Se comprobará que las restricciones se aplican también en el servidor, cuando corresponda. Las pruebas se completarán antes de la defensa final. |

Las pruebas de usabilidad se realizarán con datos ficticios y tendrán como finalidad evaluar la facilidad de uso, la comprensión de los contenidos y el funcionamiento técnico de la aplicación. No se utilizarán sus resultados para tomar decisiones médicas reales.

### 2. Alcance

#### El MVP
El recorrido del MVP y los requisitos indispensables (Must) están definidos en el documento de viabilidad técnica:  
 [Ver MVP en 02-viabilidad-tecnica.md](./02-viabilidad-tecnica.md#requisitos-funcionales)

#### Plataforma

El proyecto se desarrollará como una aplicación web responsive con un enfoque **Mobile-First**:

- **Móvil (dispositivo principal):** Es el entorno clave para el uso cotidiano de la aplicación. Tanto el niño (para introducir lecturas de glucosa o usar la calculadora visual en el colegio o fuera de casa) como el tutor necesitarán acceder de forma rápida desde sus smartphones. La interfaz se diseñará pensando en pantallas táctiles pequeñas, botones grandes y accesibles, y una navegación muy intuitiva.

- **Escritorio / Tablet (dispositivo secundario):** Accesible a través de cualquier navegador web moderno (Chrome, Firefox, Safari, Edge). Este formato está pensado especialmente para que los tutores o padres puedan consultar el historial detallado, revisar gráficos de evolución y configurar los parámetros médicos de la calculadora con mayor comodidad y amplitud de pantalla.

#### Usuarios y datos

Para las pruebas y la validación del proyecto se trabajará con un grupo controlado de **8 usuarios en total**, distribuidos equitativamente entre los dos roles del sistema:

##### Usuarios infantiles (4 niños/as)

- **2 usuarios reales:** Niños con diabetes tipo 1 del entorno cercano del equipo (incluyendo el caso de referencia familiar utilizado para definir las necesidades del proyecto). Permitirán evaluar la usabilidad real, si la interfaz resulta atractiva, si la calculadora visual se entiende de manera autónoma y si el lenguaje es adecuado a su edad.

- **2 usuarios de prueba (ficticios):** Cuentas destinadas a pruebas internas del equipo de desarrollo para testear casos límite (valores extremos de glucosa, errores al introducir datos, navegación rápida) sin condicionar registros reales.

##### Usuarios adultos (4 padres, madres o tutores)

- **2 usuarios reales:** Tutores legales vinculados directamente a los menores reales. Probarán la configuración de parámetros médicos (ratios de insulina, objetivos de glucosa), la vinculación de cuentas y la supervisión del historial desde un punto de vista cotidiano.

- **2 usuarios de prueba (ficticios):** Cuentas gestionadas por el equipo técnico para verificar la respuesta del backend, la persistencia en MongoDB y las validaciones de seguridad de roles y permisos.

#### Lo que no haremos

| Qué | Por qué |
| :--- | :--- |
| **Integración automática con sensores de glucosa continuos (CGM) o bombas de insulina (Dexcom, FreeStyle Libre, etc.)** | Los fabricantes de dispositivos médicos utilizan APIs cerradas, protocolos Bluetooth propietarios o requieren certificaciones sanitarias y acuerdos comerciales muy restrictivos. Desarrollar estas integraciones consumiría la mayor parte del tiempo del proyecto y añadiría una complejidad técnica inasumible. La versión actual se basará exclusivamente en el registro manual. |
| **Sistema de alertas push externas, SMS o avisos por correo electrónico en tiempo real** | Requiere integrar y configurar servicios de mensajería de terceros (como Twilio o Firebase Cloud Messaging), muchos de los cuales tienen costes asociados, límites estrictos en planes gratuitos o añaden dependencias externas innecesarias para un MVP. Las alertas y recordatorios se gestionarán de forma interna dentro de la propia aplicación (in-app). |
| **Aplicación móvil nativa compilada para tiendas (Google Play Store / Apple App Store)** | Desarrollar para plataformas nativas (mediante React Native, Swift o Kotlin) obligaría al equipo a lidiar con cuentas de desarrollador de pago, procesos de revisión de apps y una curva de aprendizaje mucho más elevada. Una web responsive optimizada para móviles cumple el mismo propósito con un único código base y despliegue inmediato. |
| **Sustitución o diagnóstico médico autónomo (recomendación clínica prescriptiva)** | Por motivos éticos y de responsabilidad legal, la aplicación se limita a actuar como una herramienta de apoyo al cálculo y registro basada estrictamente en los parámetros introducidos por los tutores. No emitirá diagnósticos, recomendaciones de cambio de tratamiento ni decisiones automatizadas no supervisadas. |
| **Sistema de gamificación complejo (subida de nivel de avatar, desbloqueo de accesorios, animaciones)** | Aunque es una idea atractiva para el público infantil, diseñar y programar la lógica de progresión, estados de avatar, ilustraciones y mecánicas de juego desviaría el esfuerzo del equipo del núcleo crítico del proyecto: la fiabilidad del cálculo de bolus, la correcta visualización de alimentos y la sincronización segura entre perfiles de tutor y menor. |

#### Ampliaciones futuras
1. **Sistema de notificaciones push y alertas en tiempo real:** Implementar notificaciones automáticas en el dispositivo del menor y del tutor mediante un servicio de mensajería (como Firebase Cloud Messaging). Permitiría avisar al niño de sus horas de medición sin depender de alarmas externas y alertaría inmediatamente al tutor si transcurre un periodo prolongado sin registros tras una comida.

2. **Soporte PWA (Progressive Web App) y funcionamiento offline:** Configurar Service Workers y almacenamiento local (IndexedDB) para que la aplicación web pueda instalarse como un icono en la pantalla de inicio del móvil y permita registrar datos sin conexión a internet. Clave para situaciones escolares o excursiones donde el niño pueda tener mala cobertura; los registros se guardan localmente y se sincronizan con MongoDB de forma automática al recuperar la conexión.

3. **Sistema de gamificación y avatar interactivo:** Un avatar o personaje virtual que acompaña al niño en la interfaz. El personaje ganará experiencia y subirá de nivel mediante acciones de autocuidado constantes (registrar la glucosa a tiempo, anotar las comidas, consultar la calculadora), permitiendo desbloquear accesorios visuales y elementos cosméticos. Transforma una rutina médica repetitiva en un hábito positivo y motivador.

4. **Módulo educativo interactivo (minijuegos y cuestionarios):** Crear una sección de aprendizaje dividida por temas (qué es la insulina, cómo contar raciones de hidratos, manejo durante el deporte) acompañada de cuestionarios tipo test y pequeños juegos interactivos. Fomenta la comprensión progresiva de su condición, permitiendo que el menor adquiera criterio propio a medida que crece.

---

## 4. Recursos

### Introducción

Este documento define la estructura de recursos, herramientas técnicas y metodologías de gestión necesarias para llevar a cabo el desarrollo del proyecto. Su propósito es garantizar una distribución clara de responsabilidades en el equipo, asegurar la viabilidad del desarrollo y coordinar el flujo de trabajo colaborativo.

El contenido se articula en torno a tres pilares organizativos:

* **Gestión del talento y roles (Las personas):** Asignación de liderazgos técnicos individuales (Frontend, Backend, Base de datos y QA/Despliegue) y organización modular de tareas en parejas (responsable y apoyo) para cubrir la autenticación, los registros de glucosa/comidas, la calculadora de bolus y las alertas. Se establecen canales de comunicación centralizados a través de Discord y acuerdos de equipo mediante contrato.
* **Infraestructura y herramientas (La tecnología):** Referencia al *stack* técnico detallado en la fase de viabilidad (React, Node.js, Express y MongoDB Atlas) y selección de herramientas estándar para control de versiones (Git/GitHub), prototipado (Figma), desarrollo (VS Code) y pruebas de API (Postman).
* **Flujo de trabajo y repositorio (La gestión):** Metodología ágil apoyada en GitHub Projects (tablero Kanban *To Do / In Progress / Done*), estrategia de ramificación basada en `main`, `develop` y ramas por *issue*, junto con la estructura física de carpetas para el control de la documentación, cliente frontend y servidor backend.

### 1. Las personas
#### Roles técnicos
Hemos asignado un rol técnico a cada integrante del equipo. Realmente cada persona asignada a cada rol no programa ni se encarga de todo el contenido de su área concreta, sino que será el responsable de dicha capa y de su funcionamiento.

**Frontend Lead** → Sara: Gestiona la interfaz, su diseño y la revisión del código frontend.

**Backend Lead** → Dayron: Gestiona el servidor, las APIs, la lógica del proyecto y el código backend.

**Database Manager** → Abel: diseña el esquema de la base de datos, gestiona las migraciones, asegura la integridad de los datos, optimiza las consultas y crea los scripts de datos iniciales.

**QA + despliegue** → Jesús: Comprueba la calidad del software mediante pruebas y se encarga del despliegue y la integración continua (CI/CD).

#### Responsables por módulo
Para desarrollar el MVP, hemos dividido los requisitos en módulos funcionales, cada uno con un responsable principal y una persona de apoyo, que se encargan de desarrollarlo.

| Módulo/funcionalidad | Descripción | Responsable principal | Persona de apoyo |
| :--- | :--- | :--- | :--- |
| Autenticación, Roles y Vinculación | Registro e inicio de sesión, gestión de perfiles y vinculación entre el menor y su tutor, con control de acceso según el rol (niño/adulto). | Abel | Jesús |
| Registro de Glucosa y Comidas | Formulario visual e historial para que el niño registre lecturas de glucosa y alimentos/carbohidratos, y panel para que el tutor consulte los datos. | Dayron | Sara |
| Calculadora de Insulina (Bolus) | Interfaz interactiva de cálculo para el niño y panel de configuración exclusiva de parámetros médicos (ratios, FCF) para el tutor. | Sara | Dayron |
| Recordatorios y Sistema de Alertas | Configuración de horarios habituales por el tutor y recepción de alertas in-app para mediciones del niño. | Jesús | Abel |
 
#### Comunicación (enlace al contrato)

El canal de comunicación principal que utilizará el equipo será Discord. De esta manera, el equipo realizará llamadas para la puesta en común y seguimiento del proyecto, además de utilizar sus diferentes canales de texto para aclarar dudas y para la mayor coordinación posible.

[Ir al contrato.](https://github.com/Sromerop0610/ProyectoOptativa/blob/main/docs/CONTRATO.md)

### 2. La tecnología
#### Stack, servicios y APIs (enlace a la fase 2)
[Enlace a fase 2](https://github.com/Sromerop0610/ProyectoOptativa/blob/develop/docs/propuesta/02-viabilidad-tecnica.md#requisitos-t%C3%A9cnicos)

#### Herramientas de desarrollo
| Para qué | Herramienta |
| :--- | :--- |
| **Control de versiones** | Git / GitHub |
| **Diseño UI/UX y prototipado** | Figma |
| **Entorno de desarrollo (IDE)** | Visual Studio Code |
| **Pruebas de APIs y endpoints** | Postman |
| **Gestión de base de datos** | MongoDB Atlas |
| **Comunicación del equipo** | Discord |

### 3. La gestión
#### Tablero
La organización del proyecto se gestionará mediante una metodología ágil utilizando **GitHub Projects**.

El trabajo se estructurará en las siguientes columnas principales:
* **To Do:** Tareas planificadas para el sprint o hito actual.
* **In Progress:** Tareas en desarrollo activo.
* **Done:** Tareas completadas, probadas e integradas en la rama principal.

#### Ramas

La rama main contiene el codigo principal de la aplicacion, despues tenemos una rama develop en la cual vamos implementando los diferentes cambios para que cuando esten revisados sean integrados en main, para trabajar creamos ramas para cada issue que salen de develop y una vez terminadas se integran en esta.

#### Estructura de carpetas

La estructura actual del proyecto es la siguiente

```text
proyecto-diabetes/
├── .github/ISSUE_TEMPLATE
│   └── tarea.md                
├── client/                     
│   └── README.md
├── docs/
│   ├── docs/
│       ├── 00-brainstorming.md              
│       ├── 01-problema.md         
│       ├── 02-viabilidad-tecnica.md             
│       ├── 03-objetivos-y-alcance.md              
│       └── 04-recursos.md
│   └── CONTRATO.md              
├── server/                      
│   └── README.md
├── .gitignore                   
└── README.md                    
```
