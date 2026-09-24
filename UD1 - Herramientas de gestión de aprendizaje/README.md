# UD1 - Herramientas de gestión de aprendizaje

## Objetivos de la unidad

En esta unidad se estudian los sistemas de gestión de aprendizaje y los entornos virtuales de aprendizaje (EVA), con un enfoque especial en Moodle como herramienta de administración y gestión docente.

Se pretende que el alumnado comprenda:

- qué es un LMS, un LCMS y un EVA,
- cómo se integran en la enseñanza digital,
- qué elementos forman parte de un entorno virtual de aprendizaje,
- cómo se administra y personaliza Moodle,
- qué tareas realiza un administrador de la plataforma.

---

## 1. Contexto: software libre, web 2.0 y aprendizaje digital

El desarrollo del software libre y la aparición de la web 2.0 han impulsado la creación de aplicaciones específicas para el aprendizaje permanente. Estas herramientas permiten que los estudiantes accedan a los cursos en cualquier momento, desde cualquier lugar y con diversos dispositivos.

Las plataformas actuales no solo permiten subir materiales, sino también:

- gestionar usuarios,
- registrar actividades,
- seguir el progreso del alumnado,
- crear comunidades de aprendizaje,
- coordinar procesos de evaluación,
- facilitar la comunicación entre docentes y estudiantes.

---

## 2. LCMS, LMS y EVA

### 2.1 LCMS

Los LCMS (Learning Content Management Systems) están orientados a la gestión de contenidos educativos. Su finalidad es crear, almacenar, recuperar y reutilizar pequeños módulos o unidades de aprendizaje dentro de un programa de formación más amplio.

También permiten controlar la actividad del usuario y, al actuar como repositorio de contenidos, se pueden integrar en otros sistemas.

### 2.2 LMS

Los LMS (Learning Management Systems) son sistemas web especializados en entornos formativos. Además de las funciones típicas de un CMS, ofrecen:

- gestión de usuarios,
- control de acceso,
- gestión de informes,
- registro y administración de cursos,
- arreglos por fechas,
- seguimiento del alumnado,
- procesos de matriculación.

Se suelen usar en universidades, administraciones públicas y empresas para formación interna.

### 2.3 EVA

Los EVA (Entornos Virtuales de Aprendizaje) integran herramientas de comunicación y colaboración con la gestión de contenidos y actividades. En ellos aparecen recursos como:

- foros,
- correo,
- calendarios,
- videoconferencia,
- chat,
- blogs,
- wikis.

Moodle es un ejemplo claro de EVA y LMS.

---

## 3. Moodle como sistema de gestión de aprendizaje

Moodle es una plataforma de aprendizaje diseñada para apoyar la enseñanza y la colaboración. Su gran valor es que combina:

- administración de cursos,
- gestión de estudiantes,
- herramientas de interacción,
- recursos educativos,
- evaluaciones,
- informes de actividad,
- personalización del entorno.

Gracias a su potencia y versatilidad, Moodle se ha convertido en una de las plataformas más usadas del mundo.

### 3.1 Características principales

- soporte a la colaboración y la reflexión crítica,
- aprendizaje en línea y presencial complementario,
- interfaz sencilla y ligera,
- compatibilidad con navegadores web,
- bajo coste de uso por su licencia GPL,
- posibilidad de alojar miles de cursos en la misma instalación,
- facilidad para trabajar con textos y contenidos multimedia.

---

## 4. Administración de Moodle: tareas del administrador

La administración de Moodle es esencial para asegurar el correcto funcionamiento del entorno virtual. Las labores principales del administrador incluyen:

- instalar y mantener la plataforma,
- gestionar usuarios y roles,
- configurar la apariencia y el idioma,
- crear y organizar cursos,
- instalar plugins y módulos,
- revisar accesos, permisos y seguridad,
- preparar copias de seguridad,
- revisar estadísticas e informes,
- mantener la plataforma actualizada.

---

## 5. Requisitos técnicos de instalación

Las referencias del curso indican que Moodle puede instalarse sobre un entorno LAMP:

- sistema operativo compatible,
- servidor web Apache,
- PHP,
- base de datos MySQL/MariaDB/PostgreSQL,
- memoria y espacio suficientes.

### 5.1 Recomendaciones básicas

- espacio mínimo: 160 MB para el software, aunque lo recomendable es más espacio para contenido y archivos,
- memoria RAM: 256 MB mínimo, 1 GB o más recomendado,
- uso de navegador moderno,
- cuidado con permisos de archivos y carpetas.

---

## 6. Proceso de instalación de Moodle con XAMPP

### 6.1 Pasos básicos

1. Descargar XAMPP.
2. Instalarlo y activar Apache y MySQL/MariaDB.
3. Entrar en phpMyAdmin.
4. Crear una base de datos, por ejemplo: `moodle_smrb`.
5. Descargar Moodle desde la web oficial.
6. Colocar la carpeta dentro de `htdocs`.
7. Abrir la URL del sitio en el navegador.
8. Completar el asistente de instalación.

### 6.2 Configuración recomendada

Durante la instalación suele ser necesario indicar:

- tipo de base de datos: MySQL,
- nombre de la base de datos: `moodle_smrb`,
- usuario: `root` en entornos locales,
- crear la estructura de la aplicación.

### 6.3 Directorio `moodledata`

Moodle necesita un espacio para almacenar:

- archivos subidos,
- caché,
- sesiones,
- datos temporales,
- contenido generado por usuarios.

Este directorio no debe ser accesible directamente desde la web y se recomienda ubicarlo fuera del árbol principal del sitio.

---

## 7. Problemas habituales en la instalación

### Error de extensión PHP

Se puede corregir activando en `php.ini`:

- `extension=php_zip.dll`

### Problema con la base de datos

En algunos casos es necesario cambiar:

- `mysql` por `mariadb` en `config.php`

### límite de variables de entrada

Modificar:

- `max_input_vars = 6000`

### extensiones necesarias no activadas

Activar en el archivo de configuración:

- `gd`
- `intl`
- `sodium`
- `soap`

### incompatibilidades con MariaDB

Cuando XAMPP o la versión local de bases de datos falla, puede ser necesario actualizar MariaDB y mover la carpeta de datos con cuidado para evitar perder la instalación.

---

## 8. Administración del sitio

El sitio Moodle dispone de un panel de administración que permite configurar aspectos globales de la plataforma.

### 8.1 Gestión de usuarios

Para crear usuarios:

- Administración del sitio > Usuarios > Cuentas > Agregar usuario.

Se recomienda crear perfiles tipo:

- administrador,
- profesor,
- estudiante.

### 8.2 Roles y permisos

Los roles determinan qué puede hacer cada usuario.

Se pueden administrar desde:

- Administración del sitio > Usuarios > Permisos > Asignar roles globales.

Es importante definir bien los permisos para no comprometer la seguridad ni la estructura del curso.

### 8.3 Cursos y categorías

La organización de los cursos es clave en una plataforma de formación.

Se puede acceder a:

- Cursos > Agregar/Editar cursos > Agregar una nueva categoría.

Esto facilita:

- la búsqueda,
- la navegación,
- la organización por niveles,
- la gestión de grandes cantidades de cursos.

---

## 9. Personalización y apariencia

Moodle permite adaptar la interfaz a la identidad del centro o institución.

### 9.1 Cambiar idioma

- Administración del sitio > Idioma > Paquetes de idioma > Instalar catalán.
- Ajustes de mi perfil > Editar información.
- Administración del sitio > Idioma > Ajustes de idioma.

### 9.2 Cambiar apariencia

- Administración del sitio > Apariencia > Temas > Selector de temas.

### 9.3 Activar edición visual del tema

- Ajustes de la página principal > Apariencia > Temas > Ajustes de temas > Activar Modo de diseño de temas.

---

## 10. Plugins y módulos

Moodle se puede ampliar con módulos y plugins. Entre los ejemplos mencionados en la documentación aparecen:

- Standard Slideshow,
- User_contact.

Estos complementos permiten crear contenidos más visuales o mejorar la interacción entre usuarios.

La instalación debe hacerse con cuidado, verificando compatibilidad con la versión instalada.

---

## 11. Seguridad y mantenimiento

La administración de Moodle no se limita a crear cursos: también incluye seguridad y continuidad.

### 11.1 Copias de seguridad

Se recomienda realizar copias periódicas para preservar:

- cursos,
- usuarios,
- actividades,
- contenidos,
- credenciales y configuraciones.

### 11.2 Cron

El cron permite que Moodle ejecute tareas en segundo plano, como:

- enviar correos,
- realizar procesos automáticos,
- ejecutar tareas de mantenimiento o backups.

### 11.3 Correos y mensajes

El sistema de correo es crucial para:

- restablecer contraseñas,
- enviar avisos,
- notificar actividades,
- comunicar cambios relevantes.

Se recomienda comprobar el envío de mensajes desde la configuración del sitio.

### 11.4 Permisos y archivo de configuración

Mantener bien configurados los permisos del sistema es una buena práctica para evitar:

- accesos no autorizados,
- pérdida de archivos,
- errores en la instalación,
- conflictos entre actualización y entorno local.

---

## 12. Informes y seguimiento del alumnado

Moodle ofrece herramientas para analizar el progreso del alumnado. Estas herramientas sirven para:

- revisar la participación,
- detectar alumnos con bajo rendimiento,
- valorar el uso de actividades,
- comprobar entregas y resultados,
- tomar decisiones pedagógicas.

El administrador y el docente deben saber interpretar estas métricas para mejorar la calidad de la enseñanza.

---

## 13. Buenas prácticas para la administración de una plataforma Moodle

- documentar la configuración del sitio,
- mantener un plan de copias de seguridad,
- revisar actualizaciones de Moodle y plugins,
- crear roles claros y coherentes,
- cuidar la organización de cursos y categorías,
- fomentar una estructura clara de contenidos,
- revisar periódicamente la seguridad y los permisos,
- asegurar que el correo y la matrícula funcionen correctamente.

---

### 13.1 Guía práctica de administración de Moodle

Estas actividades están pensadas para que el alumno practique la administración básica de Moodle desde la vista del administrador. La idea es seguir una secuencia clara, comprobar cada paso y documentar los resultados para entender cómo funciona la plataforma en la práctica.

#### Ejercicio 1: Configuración inicial del sitio

Pautas:

1. Accede a la administración del sitio.
2. Cambia el nombre del sitio, la descripción y la zona horaria.
3. Instala o revisa el idioma principal del curso y del sitio.
4. Comprueba si el tema visual es adecuado para la navegación del alumnado.
5. Activa o desactiva bloques útiles en la página principal.
6. Comprueba que la página principal se muestra correctamente y que el acceso a la administración es sencillo.

Qué debes comprobar:

- La interfaz es clara.
- El idioma está configurado correctamente.
- El sitio presenta una apariencia ordenada y accesible.

#### Ejercicio 2: Crear usuarios y perfiles de prueba

Pautas:

1. Entra en Administración del sitio > Usuarios > Cuentas > Agregar usuario.
2. Crea al menos tres cuentas de prueba: administrador, profesor y alumno.
3. Asigna una contraseña inicial y revisa los datos básicos del perfil.
4. Inicia sesión con cada cuenta para comprobar que funciona.
5. Comprueba que cada usuario tiene acceso a las funciones que corresponden a su rol.

Qué debes comprobar:

- Las credenciales permiten iniciar sesión.
- El perfil del usuario se ha creado correctamente.
- Los accesos difieren según el tipo de perfil.

#### Ejercicio 3: Roles y permisos

Pautas:

1. Accede a Administración del sitio > Usuarios > Permisos > Asignar roles globales.
2. Asigna el rol de administrador a un usuario con responsabilidad de gestión.
3. Asigna el rol de profesor a un docente de prueba.
4. Comprueba qué permisos tiene cada rol.
5. Verifica que un alumno no puede modificar la configuración general del sitio.

Qué debes comprobar:

- Cada usuario tiene permisos adecuados para su función.
- La seguridad del sitio no queda comprometida.
- El profesor puede gestionar el curso sin acceder a la administración global.

#### Ejercicio 4: Crear una categoría y un curso

Pautas:

1. Entra en Cursos > Agregar/Editar cursos > Agregar una nueva categoría.
2. Crea una categoría y, si procede, una subcategoría.
3. Añade un curso nuevo dentro de la categoría correspondiente.
4. Completa los datos básicos del curso: nombre, descripción, formato, fechas y nivel.
5. Guarda la información y comprueba la vista del curso como alumno.

Qué debes comprobar:

- El curso está visible y organizado correctamente.
- La navegación es clara para el alumnado.
- La estructura de cursos es lógica y ordenada.

#### Ejercicio 5: Matriculación y grupos

Pautas:

1. Accede al curso que has creado.
2. Entra en la sección de usuarios y matriculación.
3. Añade usuarios manualmente o mediante un archivo CSV.
4. Crea grupos de trabajo si el curso lo requiere.
5. Asigna usuarios a cada grupo.
6. Comprueba la diferencia entre usuarios matriculados y usuarios de invitado.

Qué debes comprobar:

- Los alumnos aparecen dentro del curso correctamente.
- Los grupos están organizados.
- El proceso de matriculación es claro y funcional.

#### Ejercicio 6: Añadir recursos y actividades

Pautas:

1. Añade un recurso del curso, como un PDF, un enlace o un archivo.
2. Crea un foro para dudas o debates.
3. Añade una tarea con fecha de entrega.
4. Crea un cuestionario breve para comprobar conocimientos.
5. Revisa cómo se ven los contenidos desde el punto de vista del alumno.

Qué debes comprobar:

- El curso contiene materiales y actividades.
- La comunicación y la evaluación están integradas.
- El alumnado puede interactuar con los recursos de forma sencilla.

#### Ejercicio 7: Configuración del correo y notificaciones

Pautas:

1. Ve a Administración del sitio > Plugins > Salidas de mensajes > Email.
2. Configura un servidor SMTP o comprueba la configuración disponible.
3. Envía un mensaje de prueba.
4. Verifica que el correo puede usarse para recuperar contraseñas y enviar avisos.
5. Revisa la configuración de avisos del curso.

Qué debes comprobar:

- Los mensajes se reciben correctamente.
- Los avisos del sistema funcionan.
- La comunicación institucional no queda bloqueada.

#### Ejercicio 8: Copias de seguridad y restauración

Pautas:

1. Accede a la administración del curso o del sitio para realizar una copia de seguridad.
2. Crea una copia de seguridad del curso con todos sus recursos.
3. Guarda la copia en un lugar seguro.
4. Restáurala en un curso de prueba.
5. Comprueba que se mantienen los recursos, actividades y usuarios.

Qué debes comprobar:

- La copia de seguridad se realiza correctamente.
- La restauración funciona sin perder contenidos.
- El curso puede recuperarse en caso de problema.

#### Ejercicio 9: Monitorización de la actividad

Pautas:

1. Revisa los informes del curso y del sitio.
2. Consulta accesos, actividades recientes y participación en foros.
3. Comprueba entregas, calificaciones y uso del contenido.
4. Identifica alumnos con poca participación.
5. Anota qué datos serían útiles para orientar la intervención educativa.

Qué debes comprobar:

- Puedes seguir la actividad del alumnado.
- Las estadísticas permiten identificar dificultades.
- La toma de decisiones se basa en evidencias.

#### Ejercicio 10: Seguridad y mantenimiento básico

Pautas:

1. Revisa los permisos de archivos y carpetas del sistema.
2. Comprueba que la carpeta `moodledata` está protegida.
3. Actualiza módulos y plugins con compatibilidad comprobada.
4. Verifica que el cron está funcionando correctamente.
5. Revisa los registros del sistema para detectar incidencias.

Qué debes comprobar:

- La plataforma está protegida frente a accesos indebidos.
- Los módulos están actualizados y compatibles.
- El mantenimiento se realiza de forma regular.

#### Ejercicio 11: Caso práctico de administración Moodle

Pautas:

1. Crea una estructura de categorías por departamento o asignatura.
2. Registra usuarios del tipo administrador, profesor y alumno.
3. Crea un curso con una presentación inicial, recursos de apoyo, un foro y un cuestionario.
4. Matricula a los estudiantes en el curso.
5. Asigna permisos de acuerdo con el perfil de cada usuario.
6. Realiza una copia de seguridad del curso.
7. Comprueba los informes de actividad y documenta el resultado final.

Qué debes comprobar:

- La estructura del sitio es clara.
- Los usuarios tienen acceso correcto.
- El curso es funcional en términos de contenidos y actividades.
- La seguridad y la recuperación del curso están aseguradas.

#### Criterios de evaluación de la práctica

La práctica se considera correcta si se cumple lo siguiente:

- se ha configurado correctamente el sitio,
- se han creado usuarios con roles adecuados,
- el curso está organizado por categorías,
- se han añadido recursos y actividades,
- la matriculación funciona correctamente,
- los permisos están bien definidos,
- se han revisado seguridad y backups,
- se ha comprobado la actividad del alumnado.

---
---

## 14. Conclusión

Moodle es más que una plataforma de cursos; es un entorno completo de administración educativa. Desde el punto de vista del administrador, se debe conocer tanto la parte técnica como la pedagógica, porque una buena gestión de Moodle influye directamente en la experiencia de aprendizaje y en la eficiencia del proceso formativo.

El alumnado debe ser capaz de entender no solo cómo usar la plataforma, sino también cómo se configura, se mantiene y se organiza para que sea segura, útil y funcional.

---

## 15. Cuestionario de repaso

1. ¿Qué es un LMS y qué diferencia tiene con un LCMS?
2. ¿Qué caracteriza a un EVA?
3. ¿Qué significa Moodle y qué tipo de herramienta es?
4. ¿Qué elementos son necesarios para instalar Moodle?
5. ¿Qué tareas realiza un administrador de Moodle?
6. ¿Por qué es importante la gestión de roles y permisos?
7. ¿Qué papel tienen el cron y los backups en la plataforma?
8. ¿Qué aspectos deben revisarse para mantener Moodle seguro?

---

## Bibliografía

- Material de la unidad “Herramientas de gestión de aprendizaje”.
- Documentación oficial de Moodle.
- Apuntes del profesor sobre EVA, LMS y LCMS.
- Guías prácticas de instalación y configuración de Moodle.

