# UD1 - Herramientas de gestión de aprendizaje

## Introducción

En esta unidad se presenta el contexto de los entornos virtuales de aprendizaje y, especialmente, la plataforma Moodle como ejemplo de sistema de gestión de aprendizaje (LMS). El objetivo principal no es solo conocer qué es Moodle, sino comprender cómo se administra, configura y mantiene un aula virtual para que cumpla sus funciones de enseñanza, evaluación, comunicación y seguimiento del alumnado.

Moodle es una herramienta clave en educación, formación profesional y entornos corporativos, ya que permite:

- organizar cursos y materiales,
- gestionar usuarios y permisos,
- controlar acceso y matriculación,
- generar informes de actividad,
- facilitar la comunicación entre profesorado y alumnado,
- crear actividades y evaluaciones,
- mantener la plataforma actualizada y segura.

---

## 1. Conceptos fundamentales: LCMS, LMS y EVA

### 1.1 LCMS (Learning Content Management System)

Los LCMS están orientados a la gestión de contenidos educativos. Su función principal es crear, almacenar, reutilizar y recuperar módulos de aprendizaje dentro de un programa formativo más amplio.

Características principales:

- gestión de recursos didácticos,
- almacenamiento de contenidos reutilizables,
- seguimiento de actividades sobre materiales,
- uso como repositorio de recursos,
- facilidad para reutilizar contenidos en distintos cursos.

Ejemplo de uso: una biblioteca de actividades, documentos, vídeos o unidades didácticas que pueden reutilizarse en varios cursos.

### 1.2 LMS (Learning Management System)

Los LMS son sistemas diseñados específicamente para entornos formativos. Se gestionan a través de la web y permiten administrar todo lo relacionado con la formación.

Funciones típicas:

- gestión de usuarios,
- control de acceso,
- registro y organización de cursos,
- seguimiento del progreso del alumnado,
- programación de actividades por fechas,
- gestión de matriculaciones,
- informes de actividad.

Los LMS se utilizan en:

- universidades y centros educativos,
- administraciones públicas,
- empresas con formación interna,
- plataformas de e-learning.

### 1.3 EVA (Entorno Virtual de Aprendizaje)

Un EVA es un entorno virtual de aprendizaje que combina herramientas de gestión del aprendizaje con recursos de comunicación y colaboración. Es la versión más cercana al usuario final, ya que integra foros, correo, calendario, chat, videoconferencia, wikis, etc.

Moodle se considera un EVA y un LMS porque permite crear un entorno formativo completo, colaborativo y accesible.

---

## 2. Características básicas de los sistemas e-learning

El e-learning es un modelo de aprendizaje a distancia basado en el acceso a través de la web a una plataforma que funciona como aula virtual o campus educativo.

Ventajas del e-learning:

- integración entre contenidos, actividades y seguimiento,
- administración centralizada de materiales,
- ahorro de tiempo en mantenimiento,
- actualización inmediata de contenidos,
- personalización del entorno,
- aprovechamiento conjunto de funciones de LMS y LCMS.

Requisitos de un sistema e-learning:

- organizar cursos,
- gestionar actividades,
- generar informes,
- administrar la plataforma,
- asegurar accesibilidad,
- mantener compatibilidad con estándares de e-learning.

---

## 3. Qué es Moodle

Moodle es un acrónimo de Module Object-Oriented Dynamic Learning Environment, que significa “Entorno de Aprendizaje Dinámico Modular Orientado a Objetos”.

Moodle fue creado en 2002 y se ha convertido en una de las plataformas más utilizadas del mundo por su flexibilidad, potencia y comunidad abierta.

A nivel de aprendizaje, Moodle ofrece:

- colaboración y reflexión crítica,
- clases online o híbridas,
- acceso desde navegador,
- interfaz sencilla y compatible,
- instalación relativamente sencilla,
- gestión de miles de cursos en un mismo servidor,
- edición de textos con editor WYSIWYG,
- gran variedad de módulos y plugins.

Moodle se distribuye bajo licencia GNU/GPL, por lo que su código es abierto y cuenta con una comunidad internacional de desarrollo y soporte.

---

## 4. Funcionalidades clave de Moodle

Algunas de las funciones más importantes de Moodle que resultan relevantes para la administración son:

- edición y diseño de temas,
- configuración de la página principal,
- administración de usuarios y roles,
- creación y organización de cursos,
- instalación de plugins y módulos,
- configuración del idioma y apariencia,
- gestión de actividades: foros, cuestionarios, tareas, wikis, chat, etc.,
- configuración de permisos y políticas de acceso,
- generación de informes y análisis,
- gestión de copias de seguridad y restauración.

### 4.1 Personalización del sitio

Desde la administración del sitio se pueden modificar:

- idioma del sitio,
- idiomas disponibles para usuarios,
- apariencia general,
- temas visuales,
- bloques de la página principal,
- configuración de edición del curso.

Ejemplos de acciones típicas:

- Administración del sitio > Idioma > Paquetes de idioma > Instalar catalán.
- Ajustes de mi perfil > Editar información para cambiar el idioma del usuario.
- Administración del sitio > Idioma > Ajustes de idioma para definir el idioma general.
- Administración del sitio > Apariencia > Temas > Selector de temas para cambiar la apariencia.
- Ajustes de la página principal > Activar edición > Agregar un bloque para añadir bloques funcionales.

### 4.2 Modo de diseño de temas

Para activar la edición visual de diseño de temas en Moodle:

- Ajustes de la página principal > Apariencia > Temas > Ajustes de temas > Activar Modo de diseño de temas.

Esto permite adaptar la interfaz y la estructura visual del campus digital.

---

## 5. Instalación de Moodle

Uno de los aspectos clave de la administración de Moodle es saber cómo instalarlo y qué requisitos necesita.

### 5.1 Requisitos básicos

Moodle normalmente se instala sobre una plataforma LAMP:

- Linux o Windows (en entornos de prueba o aula),
- Apache como servidor web,
- PHP,
- MySQL, MariaDB o PostgreSQL como base de datos,
- disco duro con espacio suficiente,
- memoria RAM suficiente para varios usuarios concurrentes.

Recomendaciones generales:

- 160 MB de espacio mínimo, aunque es mejor contar con varios GB.
- 256 MB mínimo de RAM, pero 1 GB o más es más recomendable.
- usar un navegador moderno y compatible.

### 5.2 Pasos del proceso de instalación

A continuación se resumen los pasos habituales para instalar Moodle con XAMPP, tal y como aparece en el material de apoyo:

1. Descargar XAMPP desde la web oficial.
2. Instalarlo en el directorio correspondiente y activar Apache y MySQL/MariaDB.
3. Acceder a phpMyAdmin y crear una base de datos, por ejemplo: `moodle_smrb`.
4. Descargar Moodle desde la web oficial.
5. Colocar la carpeta de Moodle dentro de `htdocs` del servidor local.
6. Abrir en el navegador la URL del sitio, por ejemplo: `http://localhost/moodle`.
7. Seguir el asistente de instalación y seleccionar:
   - tipo de base de datos: MySQL,
   - nombre de la base de datos: `moodle_smrb`,
   - usuario: `root`.

### 5.3 Estructura importante para la instalación

Moodle necesita dos elementos fundamentales:

- el directorio del código de Moodle,
- un directorio `moodledata` para almacenar archivos, caché, sesiones, temporales y recursos subidos por usuarios.

Este directorio debe estar fuera del árbol web y no accesible directamente por navegación web, ya que sería un grave problema de seguridad.

### 5.4 Errores frecuentes en la instalación y soluciones

Los apuntes del curso destacan varios problemas habituales y sus soluciones:

#### Error 1: extensión PHP faltante

Si aparece un error de extensión PHP, revisar `php.ini` y activar la extensión:

- `extension=php_zip.dll`

Se guarda el archivo, se reinicia Apache y se vuelve a instalar.

#### Error 2: base de datos MySQL/MariaDB

Si la instalación identifica un problema con la base de datos, revisar `config.php` y cambiar:

- `mysql` por `mariadb` en `$CFG->dbtype`

#### Error 3: límite de variables de entrada

En `php.ini` se puede modificar:

- `max_input_vars = 6000`

quitando el punto y coma de delante.

#### Error 4: extensiones necesarias no activadas

En `php.ini`, activar:

- `extension=gd`
- `extension=intl`
- `extension=sodium`
- `extension=soap`

#### Error 5: conflicto con MariaDB y MySQL

Cuando el sistema falla por incompatibilidades de base de datos, se puede descargar la versión correcta de MariaDB, cambiar la carpeta `mysql` por una nueva versión y conservar los archivos de datos y scripts. Luego se actualiza con la herramienta correspondiente.

Este tipo de incidencia es muy habitual en entornos locales con XAMPP y requiere cuidado con los archivos de la base de datos y la configuración.

---

## 6. Administración del sitio Moodle

La administración del sitio es la parte esencial para que la plataforma funcione bien. Desde este panel se configuran los aspectos globales de la plataforma.

### 6.1 Acceso al panel de administración

Desde el rol de administrador se puede acceder a:

- Administración del sitio,
- configuración general,
- usuarios,
- cursos,
- apariencia,
- seguridad,
- informes,
- mantenimiento.

### 6.2 Gestión de usuarios

Una de las tareas principales del administrador es crear y gestionar cuentas de usuario.

Acción recomendada:

- Administración del sitio > Usuarios > Cuentas > Agregar usuario.

Se suele crear una estructura simple con varios perfiles:

- `admin2` como administrador secundario,
- `profesor1` como docente,
- `alumno1` como estudiante.

Es importante definir bien los roles para asegurar que cada usuario tenga las capacidades correctas.

### 6.3 Roles y permisos

Moodle usa roles para controlar el acceso y las acciones permitidas en cada contexto.

Se puede acceder a:

- Administración del sitio > Usuarios > Permisos > Asignar roles globales.

Si los roles no aparecen en todos los contextos, también puede revisarse:

- Permisos > Definir roles > seleccionar el rol > tipos de contexto en que puede asignarse este rol > Sistema.

Principales roles:

- administrador,
- docente,
- estudiante,
- invitado,
- profesor no editor,
- gestor de curso, etc.

Esto es fundamental para evitar errores de seguridad y garantizar una buena organización del curso.

### 6.4 Gestión de cursos y categorías

Moodle permite organizar los cursos por categorías para facilitar la navegación y búsqueda.

Acciones habituales:

- Cursos > Agregar/Editar cursos > Agregar una nueva categoría.
- Cursos > Agregar/Editar cursos > Agregar una sub-categoría.

Esto es muy útil cuando la institución tiene muchos cursos, por ejemplo:

- Formación dual,
- FP Básica,
- CFGS,
- cursos de idiomas,
- cursos de actualización docente.

### 6.5 Configuración de cursos

Cuando se crea un curso, el administrador o el docente debe definir:

- nombre del curso,
- categoría,
- descripción,
- formato del curso,
- fechas de disponibilidad,
- método de matriculación,
- permisos del alumnado,
- actividades y recursos necesarios.

Moodle admite varios formatos de curso según la estrategia didáctica: semanal, por temas, social, etc.

---

## 7. Administración de la apariencia y del sitio

Moodle permite adaptar la experiencia visual del entorno educativo.

### 7.1 Idiomas

Es posible instalar paquetes de idioma y adaptar la plataforma al contexto del alumnado.

Ejemplo:

- Administración del sitio > Idioma > Paquetes de idioma > Instalar catalán.

También cada usuario puede cambiar su lenguaje desde:

- Ajustes de mi perfil > Editar información.

### 7.2 Temas visuales

Para cambiar la apariencia general del sitio:

- Administración del sitio > Apariencia > Temas > Selector de temas.

También se puede activar el modo de diseño para trabajar visualmente la composición del sitio y la página principal.

### 7.3 Bloques

Los bloques son elementos añadidos a la interfaz que aportan funcionalidades útiles como:

- calendario,
- actividades recientes,
- buscador,
- administración rápida,
- validación de usuarios,
- enlaces a recursos.

Ejemplo:

- Ajustes de la página principal > Activar edición > Agregar un bloque.

---

## 8. Instalación de plugins y módulos

Moodle dispone de una gran comunidad de desarrollo y puede ampliarse con plugins y módulos.

Se accede a:

- Página de Moodle > Descargas > Módulos y plugins.

Ejemplos mencionados en el material:

- Standard Slideshow: descargar y descomprimir en la carpeta `moodle/mod`.
- User_contact: añadir funcionalidades de contacto entre usuarios.

Los plugins pueden ampliar:

- actividades,
- informes,
- bloque de contenido,
- integración con servicios externos,
- nuevas opciones de notificación.

El administrador debe verificar compatibilidad y versiones antes de instalarlos para evitar problemas de funcionamiento.

---

## 9. Administración de seguridad y mantenimiento

La administración de Moodle no termina con la instalación. La seguridad y el mantenimiento continuo son fundamentales.

### 9.1 Copias de seguridad

Es imprescindible realizar copias de seguridad periódicas para evitar pérdida de información. Moodle permite:

- backups del sitio,
- backups de cursos,
- restauración de contenidos.

Se recomienda:

- guardar backups externos,
- controlar fechas y frecuencia,
- mantener la base de datos y los archivos del sitio protegidos.

### 9.2 Cron

Moodle usa tareas programadas o cron para ejecutar procesos en segundo plano, como:

- envío de correos,
- programación de actividades,
- copias de seguridad automatizadas,
- tareas de mantenimiento.

Es una herramienta muy importante para el correcto funcionamiento de la plataforma.

### 9.3 Correo y mensajes

El administrador debe comprobar que el sistema de correo funciona correctamente, ya que el email se usa para:

- recuperar contraseñas,
- notificar actividades,
- enviar mensajes del sistema,
- confirmaciones de registro.

Configuración recomendada:

- Administración del sitio > Plugins > Salidas de mensajes > Email.
- Definir servidor SMTP y autenticación.

### 9.4 Permisos de archivos y directorios

La seguridad del sitio depende en gran medida de los permisos del sistema. Es muy importante:

- que los archivos del núcleo de Moodle no sean escribibles por el servidor web,
- que `moodledata` tenga permisos adecuados para escritura,
- que no sea accesible públicamente,
- que se comprueben los permisos tras cada actualización o migración.

---

## 10. Administración de la base de datos

Moodle depende de una base de datos para almacenar:

- usuarios,
- cursos,
- actividades,
- archivos,
- logs,
- configuraciones,
- calificaciones.

El administrador debe:

- crear la base de datos adecuadamente,
- asignar un usuario específico con permisos mínimos,
- proteger la credencial de acceso,
- planificar copias de seguridad y restauraciones,
- no usar la cuenta `root` para la conexión de producción.

---

## 11. Reportes, seguimiento y analítica

Uno de los puntos fuertes de Moodle es la posibilidad de generar informes para evaluar:

- actividad del alumnado,
- participación en foros,
- entregas de tareas,
- resultados de cuestionarios,
- progreso general por curso.

Desde la administración se pueden revisar:

- usuarios activos,
- estado del curso,
- accesos y tiempos,
- actividades completadas,
- rendimiento por módulo.

Esto es clave para la toma de decisiones de mejora del proceso de enseñanza.

---

## 12. Buenas prácticas de administración en Moodle

Para un uso eficiente y seguro de Moodle, se recomienda:

- mantener actualizada la versión de Moodle,
- revisar los plugins y compatibilidades antes de instalarlos,
- crear roles bien definidos,
- coordinar la creación de cursos con categorías,
- activar copias de seguridad periódicas,
- documentar los cambios realizados en la plataforma,
- comprobar que el correo y los permisos funcionan,
- revisar periódicamente la seguridad del sitio,
- preparar un plan de mantenimiento para cada curso.

---

### 12.1 Guía práctica de administración de Moodle

Estas actividades están pensadas para que el alumno practique la administración básica de Moodle desde la vista del administrador. Es importante seguir cada paso con atención, comprobar los resultados y documentar lo que se va configurando para entender cómo funciona la plataforma en la práctica.

#### Ejercicio 1: Configuración inicial del sitio

Pautas:

1. Accede a la administración del sitio.
2. Cambia el nombre del sitio, la descripción y la zona horaria.
3. Comprueba el idioma principal del sitio y la apariencia general.
4. Revisa la página principal y activa o desactiva bloques útiles.
5. Comprueba que la interfaz es clara y que el acceso a la administración es sencillo.

Qué debes comprobar:

- La apariencia del sitio es ordenada.
- El idioma está bien configurado.
- La navegación del portal resulta clara.

#### Ejercicio 2: Crear usuarios y perfiles de prueba

Pautas:

1. Entra en Administración del sitio > Usuarios > Cuentas > Agregar usuario.
2. Crea cuentas de prueba del tipo administrador, profesor y alumno.
3. Asigna una contraseña inicial y revisa los datos básicos del perfil.
4. Inicia sesión con las distintas cuentas para comprobar que funcionan.
5. Verifica que cada usuario tiene acceso distinto según su perfil.

Qué debes comprobar:

- Las cuentas se crean correctamente.
- El inicio de sesión funciona.
- Los permisos son distintos según el perfil.

#### Ejercicio 3: Roles y permisos

Pautas:

1. Entra en Administración del sitio > Usuarios > Permisos > Asignar roles globales.
2. Asigna roles para administrador, profesor y estudiante.
3. Comprueba qué acciones puede hacer cada perfil.
4. Verifica que un alumno no puede modificar parámetros del sitio.
5. Anota las diferencias entre roles.

Qué debes comprobar:

- Los permisos están bien definidos.
- El alumnado no tiene acceso a funciones administrativas.
- El profesorado puede gestionar su curso sin alterar la configuración global.

#### Ejercicio 4: Crear una categoría y un curso

Pautas:

1. Ve a Cursos > Agregar/Editar cursos > Agregar una nueva categoría.
2. Crea una categoría y, si procede, una subcategoría.
3. Añade un curso nuevo dentro de la categoría.
4. Completa los datos principales del curso: nombre, descripción, formato, fechas y nivel.
5. Guarda los cambios y revisa la vista desde el perfil de alumno.

Qué debes comprobar:

- El curso está bien organizado.
- La estructura es clara para el alumnado.
- La información del curso está completa.

#### Ejercicio 5: Matriculación y grupos

Pautas:

1. Accede al curso que has creado.
2. Entra en la sección de usuarios y matriculación.
3. Añade usuarios al curso manualmente o mediante archivo CSV.
4. Crea grupos de trabajo si se consideran necesarios.
5. Asigna alumnos a cada grupo.
6. Comprueba la diferencia entre usuarios matriculados y usuarios con acceso de invitado.

Qué debes comprobar:

- Los alumnos están dentro del curso.
- Los grupos están bien definidos.
- El acceso del alumnado es correcto.

#### Ejercicio 6: Añadir recursos y actividades

Pautas:

1. Añade un recurso como un PDF, un enlace o un archivo.
2. Crea un foro para dudas y debates.
3. Añade una tarea con fecha de entrega.
4. Crea un cuestionario breve para comprobar aprendizaje.
5. Revisa el curso desde la perspectiva del estudiante.

Qué debes comprobar:

- El curso incluye materiales y actividades.
- La evaluación y la comunicación están integradas.
- El alumnado puede interactuar con los contenidos fácilmente.

#### Ejercicio 7: Configuración del correo y notificaciones

Pautas:

1. Ve a Administración del sitio > Plugins > Salidas de mensajes > Email.
2. Revisa la configuración del servidor SMTP o del correo del sistema.
3. Envía un mensaje de prueba.
4. Comprueba que el correo puede usarse para avisos y recuperación de contraseñas.
5. Revisa la configuración de notificaciones del curso.

Qué debes comprobar:

- Los mensajes llegan correctamente.
- Se gestionan avisos del sistema y de recuperación de acceso.
- La comunicación no queda bloqueada.

#### Ejercicio 8: Copias de seguridad y restauración

Pautas:

1. Accede a la administración del curso o del sitio.
2. Realiza una copia de seguridad del curso.
3. Guarda la copia en un lugar seguro.
4. Restaura la copia en un curso de prueba.
5. Verifica que materiales, actividades y usuarios se mantienen intactos.

Qué debes comprobar:

- La copia de seguridad funciona.
- La restauración conserva el contenido.
- La plataforma puede recuperarse si ocurre un problema.

#### Ejercicio 9: Analizar informes y progreso

Pautas:

1. Revisa los informes del curso y del sitio.
2. Consulta accesos, actividades recientes y participación en foros.
3. Comprueba entregas, calificaciones y uso del contenido.
4. Identifica alumnos con baja participación.
5. Anota qué datos podrían servir para mejorar la enseñanza.

Qué debes comprobar:

- Puedes seguir la actividad del alumnado.
- Las estadísticas ayudan a detectar dificultades.
- La intervención educativa puede basarse en evidencias.

#### Ejercicio 10: Seguridad y mantenimiento

Pautas:

1. Revisa los permisos de archivos y carpetas del sistema.
2. Comprueba que la carpeta `moodledata` está protegida.
3. Actualiza módulos y plugins con compatibilidad comprobada.
4. Verifica que el cron funciona correctamente.
5. Revisa registros del sistema para detectar incidencias.

Qué debes comprobar:

- La plataforma está protegida frente a accesos indebidos.
- Los módulos están actualizados.
- El mantenimiento se realiza de manera regular.

#### Ejercicio 11: Caso práctico final

Pautas:

1. Crea una estructura de categorías por departamento o asignatura.
2. Registra usuarios de tipo administrador, profesor y estudiante.
3. Crea un curso con recursos, un foro y un cuestionario.
4. Matricula a los alumnos en ese curso.
5. Asigna permisos según el rol de cada usuario.
6. Realiza una copia de seguridad del curso.
7. Revisa los informes de actividad y documenta los resultados.

Qué debes comprobar:

- La estructura del sitio es clara.
- Los usuarios tienen acceso correcto.
- El curso funciona como entorno de aprendizaje.
- La seguridad y la recuperación del contenido están aseguradas.

#### Criterios de evaluación de la práctica

La práctica será correcta si:

- se ha configurado adecuadamente el sitio,
- se han creado usuarios con roles correctos,
- el curso está organizado por categorías,
- se han añadido recursos y actividades,
- la matriculación funciona correctamente,
- los permisos están bien definidos,
- se han revisado seguridad y copias de seguridad,
- se ha comprobado la actividad del alumnado.

---

## 13. Resumen final

Moodle no es solo una herramienta para subir materiales: es una plataforma completa de administración educativa. Su valor real radica en que un administrador puede:

- instalar y mantener la infraestructura tecnológica,
- organizar el entorno virtual,
- gestionar a usuarios y roles,
- configurar cursos y actividades,
- mantener la seguridad y la disponibilidad,
- analizar la participación y resultados,
- facilitar la enseñanza y el aprendizaje digital.

Por eso, desde el punto de vista de la administración, Moodle es una solución poderosa y flexible, especialmente útil para centros educativos, entornos de formación y proyectos de e-learning.

---

## 14. Checklist de administración Moodle

Antes de dar por finalizado un Moodle en un centro o aula virtual, conviene comprobar:

- [ ] la base de datos está creada y funciona,
- [ ] el directorio `moodledata` está bien configurado,
- [ ] el sitio responde correctamente en el navegador,
- [ ] hay un administrador principal y roles definidos,
- [ ] existen cursos organizados por categorías,
- [ ] los usuarios están creados con sus permisos correctos,
- [ ] están activados los plugins y módulos necesarios,
- [ ] el correo y cron funcionan,
- [ ] hay copias de seguridad periódicas,
- [ ] se ha revisado la seguridad del sitio.

---

## 15. Actividades sugeridas

1. Crear una base de datos y preparar la instalación de Moodle.
2. Identificar los requisitos de software y hardware.
3. Crear usuarios del tipo administrador, profesor y alumno.
4. Organizar cursos por categorías.
5. Configurar idioma y apariencia del sitio.
6. Asignar roles y permisos.
7. Explorar la administración de plugins y copias de seguridad.
8. Analizar un caso práctico de aula virtual en Moodle.

---

## Bibliografía recomendada

- MoodleDocs. Installation.
- MoodleDocs. Site Administration.
- Material docente del curso “Herramientas de gestión de aprendizaje”.
- Apuntes del profesor sobre LMS, LCMS y EVA.

Se recomienda revisar también la documentación oficial de Moodle para profundizar en funciones y configuraciones específicas.
