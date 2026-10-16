# Fase 3 · Objetivos y alcance · <estudio>
## Introducción
## 1. Objetivos
### Objetivo general
Desarrollar una aplicación web accesible, visual e intuitiva para facilitar a los niños con diabetes el seguimiento de su enfermedad y el aprendizaje de hábitos de autocuidado, favoreciendo su autonomía y permitiendo a sus padres o tutores supervisar su evolución.

### Objetivos específicos

| ID | Objetivo SMART | Qué se mide | Valor de éxito | Cómo se comprueba |
|---|---|---|---|---|
| OE1 | Conseguir que, antes de la defensa final, al menos el 75 % de los niños participantes registre correctamente un nivel de glucosa en menos de dos minutos y sin ayuda de un adulto. | Porcentaje de participantes que completan correctamente el registro y tiempo empleado. | Al menos el 75 % completa la tarea en menos de 120 segundos sin ayuda. | Prueba de usabilidad con un mínimo de cuatro participantes del perfil infantil, utilizando datos ficticios. Se registrarán los tiempos y la necesidad de ayuda antes de la defensa final. |
| OE2 | Conseguir que, antes de la defensa final, al menos el 75 % de los niños participantes obtenga una puntuación mínima del 60 % en un cuestionario sobre los contenidos educativos de la aplicación. | Porcentaje de participantes que alcanza la puntuación mínima en el cuestionario. | Al menos el 75 % de los participantes responde correctamente a un mínimo de 3 de las 5 preguntas. | Se realizará un cuestionario de cinco preguntas sobre los contenidos educativos de la aplicación, como la glucosa, la alimentación, la insulina o el ejercicio físico. Se comprobarán los resultados antes de la defensa final. |
| OE3 | Conseguir que, antes de la defensa final, al menos el 75 % de los adultos participantes consulte los últimos registros de glucosa de su hijo e identifique correctamente la información mostrada en menos de 90 segundos. | Porcentaje de adultos que localiza e interpreta correctamente la información y tiempo empleado. | Al menos el 75 % completa la tarea correctamente en menos de 90 segundos. | Prueba de usabilidad con un mínimo de cuatro adultos que representen el perfil de padres o tutores, utilizando registros ficticios. Se registrarán los tiempos, los aciertos y la necesidad de ayuda. |
| OE4 | Conseguir que, antes de la defensa final, al menos el 75 % de los niños participantes complete de forma autónoma una actividad de seguimiento y una actividad educativa, obteniendo las recompensas correspondientes. | Porcentaje de participantes que completa ambas actividades sin ayuda y recibe correctamente los puntos o la experiencia. | Al menos el 75 % completa las dos actividades sin ayuda y obtiene las recompensas previstas. | Se pedirá a los participantes que registren un dato ficticio de glucosa y completen un cuestionario educativo. Se comprobará que ambas acciones quedan registradas y que las recompensas se actualizan correctamente. |
| OE5 | Conseguir que, antes de la defensa final, todas las pruebas funcionales de permisos confirmen que los niños no pueden modificar los parámetros de la calculadora de insulina y que los tutores autorizados sí pueden gestionarlos. | Funcionamiento de los permisos y existencia de accesos o modificaciones no autorizados. | El 100 % de los casos de prueba definidos se resuelve correctamente. | Se realizarán pruebas funcionales con cuentas de niño y de tutor, intentando acceder y modificar los parámetros desde ambos perfiles. Se comprobará que las restricciones se aplican también en el servidor, cuando corresponda. Las pruebas se completarán antes de la defensa final. |

Las pruebas de usabilidad se realizarán con datos ficticios y tendrán como finalidad evaluar la facilidad de uso, la comprensión de los contenidos y el funcionamiento técnico de la aplicación. No se utilizarán sus resultados para tomar decisiones médicas reales.

## 2. Alcance

### El MVP
El recorrido del MVP y los requisitos indispensables (Must) están definidos en el documento de viabilidad técnica:  
 [Ver MVP en 02-viabilidad-tecnica.md](./02-viabilidad-tecnica.md#requisitos-funcionales)

### Plataforma

El proyecto se desarrollará como una aplicación web responsive con un enfoque **Mobile-First**:

- **Móvil (dispositivo principal):** Es el entorno clave para el uso cotidiano de la aplicación. Tanto el niño (para introducir lecturas de glucosa o usar la calculadora visual en el colegio o fuera de casa) como el tutor necesitarán acceder de forma rápida desde sus smartphones. La interfaz se diseñará pensando en pantallas táctiles pequeñas, botones grandes y accesibles, y una navegación muy intuitiva.

- **Escritorio / Tablet (dispositivo secundario):** Accesible a través de cualquier navegador web moderno (Chrome, Firefox, Safari, Edge). Este formato está pensado especialmente para que los tutores o padres puedan consultar el historial detallado, revisar gráficos de evolución y configurar los parámetros médicos de la calculadora con mayor comodidad y amplitud de pantalla.

### Usuarios y datos

Para las pruebas y la validación del proyecto se trabajará con un grupo controlado de **8 usuarios en total**, distribuidos equitativamente entre los dos roles del sistema:

#### Usuarios infantiles (4 niños/as)

- **2 usuarios reales:** Niños con diabetes tipo 1 del entorno cercano del equipo (incluyendo el caso de referencia familiar utilizado para definir las necesidades del proyecto). Permitirán evaluar la usabilidad real, si la interfaz resulta atractiva, si la calculadora visual se entiende de manera autónoma y si el lenguaje es adecuado a su edad.

- **2 usuarios de prueba (ficticios):** Cuentas destinadas a pruebas internas del equipo de desarrollo para testear casos límite (valores extremos de glucosa, errores al introducir datos, navegación rápida) sin condicionar registros reales.

#### Usuarios adultos (4 padres, madres o tutores)

- **2 usuarios reales:** Tutores legales vinculados directamente a los menores reales. Probarán la configuración de parámetros médicos (ratios de insulina, objetivos de glucosa), la vinculación de cuentas y la supervisión del historial desde un punto de vista cotidiano.

- **2 usuarios de prueba (ficticios):** Cuentas gestionadas por el equipo técnico para verificar la respuesta del backend, la persistencia en MongoDB y las validaciones de seguridad de roles y permisos.

### Lo que no haremos

| Qué | Por qué |
| :--- | :--- |
| **Integración automática con sensores de glucosa continuos (CGM) o bombas de insulina (Dexcom, FreeStyle Libre, etc.)** | Los fabricantes de dispositivos médicos utilizan APIs cerradas, protocolos Bluetooth propietarios o requieren certificaciones sanitarias y acuerdos comerciales muy restrictivos. Desarrollar estas integraciones consumiría la mayor parte del tiempo del proyecto y añadiría una complejidad técnica inasumible. La versión actual se basará exclusivamente en el registro manual. |
| **Sistema de alertas push externas, SMS o avisos por correo electrónico en tiempo real** | Requiere integrar y configurar servicios de mensajería de terceros (como Twilio o Firebase Cloud Messaging), muchos de los cuales tienen costes asociados, límites estrictos en planes gratuitos o añaden dependencias externas innecesarias para un MVP. Las alertas y recordatorios se gestionarán de forma interna dentro de la propia aplicación (in-app). |
| **Aplicación móvil nativa compilada para tiendas (Google Play Store / Apple App Store)** | Desarrollar para plataformas nativas (mediante React Native, Swift o Kotlin) obligaría al equipo a lidiar con cuentas de desarrollador de pago, procesos de revisión de apps y una curva de aprendizaje mucho más elevada. Una web responsive optimizada para móviles cumple el mismo propósito con un único código base y despliegue inmediato. |
| **Sustitución o diagnóstico médico autónomo (recomendación clínica prescriptiva)** | Por motivos éticos y de responsabilidad legal, la aplicación se limita a actuar como una herramienta de apoyo al cálculo y registro basada estrictamente en los parámetros introducidos por los tutores. No emitirá diagnósticos, recomendaciones de cambio de tratamiento ni decisiones automatizadas no supervisadas. |
| **Sistema de gamificación complejo (subida de nivel de avatar, desbloqueo de accesorios, animaciones)** | Aunque es una idea atractiva para el público infantil, diseñar y programar la lógica de progresión, estados de avatar, ilustraciones y mecánicas de juego desviaría el esfuerzo del equipo del núcleo crítico del proyecto: la fiabilidad del cálculo de bolus, la correcta visualización de alimentos y la sincronización segura entre perfiles de tutor y menor. |

### Ampliaciones futuras
1. **Sistema de notificaciones push y alertas en tiempo real:** Implementar notificaciones automáticas en el dispositivo del menor y del tutor mediante un servicio de mensajería (como Firebase Cloud Messaging). Permitiría avisar al niño de sus horas de medición sin depender de alarmas externas y alertaría inmediatamente al tutor si transcurre un periodo prolongado sin registros tras una comida.

2. **Soporte PWA (Progressive Web App) y funcionamiento offline:** Configurar Service Workers y almacenamiento local (IndexedDB) para que la aplicación web pueda instalarse como un icono en la pantalla de inicio del móvil y permita registrar datos sin conexión a internet. Clave para situaciones escolares o excursiones donde el niño pueda tener mala cobertura; los registros se guardan localmente y se sincronizan con MongoDB de forma automática al recuperar la conexión.

3. **Sistema de gamificación y avatar interactivo:** Un avatar o personaje virtual que acompaña al niño en la interfaz. El personaje ganará experiencia y subirá de nivel mediante acciones de autocuidado constantes (registrar la glucosa a tiempo, anotar las comidas, consultar la calculadora), permitiendo desbloquear accesorios visuales y elementos cosméticos. Transforma una rutina médica repetitiva en un hábito positivo y motivador.

4. **Módulo educativo interactivo (minijuegos y cuestionarios):** Crear una sección de aprendizaje dividida por temas (qué es la insulina, cómo contar raciones de hidratos, manejo durante el deporte) acompañada de cuestionarios tipo test y pequeños juegos interactivos. Fomenta la comprensión progresiva de su condición, permitiendo que el menor adquiera criterio propio a medida que crece.
