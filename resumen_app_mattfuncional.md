# Resumen Mattfuncional — marketing y presentación a gimnasios

**Carpeta de trabajo mercado:** copia sincronizada y guía en `para insertar al mercado/` (leé `LEEME.md` ahí si usás solo esa carpeta en Cursor).

**Uso sugerido:** pegar este archivo en otra sesión de Cursor junto con el resumen de **MiGym Virtual**, los HTML del **manual de usuario** de ambas apps y cualquier brief de marca. Sirve como base para PDF, carpeta de presentación, folletos, guiones de video y material generado con herramientas de IA (diseño, copy, storyboard, etc.).

**Producto:** **Mattfuncional** — plataforma web para **administración integral del gimnasio** (gestión de alumnos, rutinas, contenido pedagógico, presencia en sala y **cara pública** del negocio). Complementa al ecosistema **MiGym Virtual** (app orientada al **personal trainer** y envío de rutinas); en comercialización conviene explicar cómo se combinan o cuándo conviene cada una.

**Referencia técnica interna (manual HTML):** `src/main/resources/templates/profesor/manual-usuario.html`

---

## 1. Página pública principal — la cara del gimnasio (alto valor comercial)

La **página pública** es el escaparate digital del gimnasio: primera impresión, confianza y conversión (consultas, WhatsApp, visitas). En Mattfuncional está pensada para ser **la cara de la empresa** con contenido **adaptable al cliente** sin depender del desarrollador para el día a día.

### 1.1 Personalización a medida del cliente

- **Identidad:** estética alineada al gimnasio, **logo**, textos y mensajes a la medida del negocio.
- **Imágenes y medios:** reemplazo de recursos en **carrusel**, slides con copy propio, variantes **escritorio y móvil** donde aplique (por ejemplo video hero en formatos distintos para TV de fondo vs. story en celular).
- **Rutas públicas de referencia en el sistema:** inicio (`/` o `/publica`), **Planes y promociones** (`/planes`).

### 1.2 Qué incluye hoy el paquete de página pública (para “precio actual incluye…”)

Incluir en propuestas comerciales, de forma explícita:

| Incluye | Descripción breve |
|--------|-------------------|
| **Inicio con carrusel** | Presentación del gimnasio con varios slides: mensajes, imágenes y **video de presentación** en el hero (autoplay, loop, pensado para impacto visual). |
| **Accesos rápidos** | Llamadas a la acción hacia planes, contacto, WhatsApp, etc., según la estructura de la landing. |
| **Sección de planes y promociones** | Página dedicada con **tarjetas** de planes y promos, precios, servicios, días/horarios y enlace a consulta. |
| **Imágenes descriptivas** | Slides del carrusel con fotos del espacio, equipo, clases (contenido sustituible por el gimnasio). |
| **Redes sociales** | Enlaces configurables (por ejemplo **Instagram** con URL armada desde usuario o link completo). |
| **Formulario de contacto** | Consultas que llegan al flujo administrativo del sistema. |
| **WhatsApp** | Botón / enlace con **mensaje listo** hacia el número configurado (URL de envío de WhatsApp). |
| **100 % responsive** | Misma experiencia usable en **celular, tablet y PC** (menú móvil tipo offcanvas, carrusel adaptable). |
| **Panel privado — sin desarrollador para publicar** | **Administración de la página pública** desde el panel (roles administrador): planes, promociones, textos, medios, consultas recibidas. **Publicación al instante** de promociones y cambios sin pedir deploy al equipo técnico. |

### 1.3 Mensaje clave para folletos / video

> *“Tu gimnasio se ve profesional en internet desde el primer día: carrusel, video, planes y contacto por WhatsApp, todo actualizable vos mismo desde el panel.”*

---

## 2. App de administración del gimnasio — panel del profesor (vista rápida y dinámica)

El **corazón operativo** es un **panel web unificado** para el profesor o staff: **vista rápida y dinámica** — resumen en dashboard, accesos en un clic a alumnos, series, rutinas, calendario, ejercicios, pizarra y administración. Los **alumnos no instalan nada** para ver su rutina: acceden por **enlace web** desde celular, tablet o PC.

### 2.1 Usuarios del sistema (staff)

- **Administración de usuarios** con rol (por ejemplo **ADMIN**, **AYUDANTE**; existe además rol técnico **DEVELOPER** para soporte).
- **Alta, modificación y baja** de usuarios del sistema; control de acceso a la parte privada con **correo y contraseña**.
- Los **alumnos no son “usuarios login”**: se cargan en el sistema y consumen rutinas por **enlace público** o WhatsApp, sin app obligatoria.

### 2.2 Alumnos — gestión y ficha

- **CRUD de alumnos:** carga, modificación y baja lógica (estado activo/inactivo según reglas de negocio).
- **Tipo de asistencia:** **presencial**, **virtual** o **semipresencial**.
- **Ficha del alumno** con datos a primera vista útiles para el entrenador: datos personales, contacto, horarios, **restricciones u observaciones médicas**, **objetivo del alumno**, peso, sexo, **fecha de nacimiento** (edad calculada automáticamente), etc.
- **Filtros** en listado (nombre, estado, tipo, día, horario) con **persistencia** al volver a la página.
- **Presentismo / asistencia** del día desde la lista (ciclos tipo pendiente / presente / ausente según implementación).
- **Cumpleaños del día** visible desde el panel (indicador en tarjeta de alumnos + detalle).

### 2.3 Seguimiento de avance

- Relacionado con las **anotaciones y seguimiento** que el profesor registra en cada visita o revisión (módulo de **progreso** en ficha del alumno: observaciones, grupos trabajados, control por fecha, etc.).
- Complementa la **asistencia** y el historial para ver evolución en el tiempo.

### 2.4 Calendario semanal

- **Calendario semanal** del profesor en **nueva pestaña**; vista de grilla con **rango de fechas** y opción de semana **lun–sáb** o **lun–dom**.
- Sirve para visualizar **ocupación / planificación** de la semana (detalle según cómo lo expliques en el pitch: citas, bloques, alumnos — alinear con lo que muestra la pantalla en demo).

### 2.5 Ejercicios — biblioteca y creación propia

- Listado tipo **tarjetas / lista rica** con búsqueda y filtro por **grupo muscular**.
- **Ejercicios predeterminados del sistema:** el producto incluye una **biblioteca inicial** para empezar a trabajar de inmediato (en código la referencia operativa es **60 ejercicios predeterminados**; en comercial podés decir “decenas de ejercicios listos” o “60+ predeterminados” según política de versión).
- **Creación de ejercicios propios:** nombre, descripción, tipo, grupos musculares, **imagen o video** (contenido visual propio del gimnasio / marca).
- **Grupos musculares:** grupos del sistema (no editables) más **grupos propios** del profesor.

### 2.6 Series y rutinas

- **Series:** agrupan ejercicios en secuencia con datos de trabajo (**repeticiones, peso, orden** en la serie; el manual describe subir/bajar orden).
- **Rutinas:** plantillas armadas con **una o más series** en orden definido.
- **Asignación de rutinas al alumno** genera la **hoja pública** con **enlace único**; el alumno **no instala** nada.
- **Administración total de asignaciones:** **activar / desactivar** (enlace muestra rutina o mensaje de inactiva), modificar, copiar enlace, envío por **WhatsApp** si hay celular cargado, **inactivar todas** desde ficha cuando haga falta.

### 2.7 Datos en series, bloques y rutinas (peso, reps, tiempo)

- En **series** y flujo hacia **rutinas / hoja pública**, el sistema contempla información de entreno: **peso, repeticiones, vueltas/series**, y en ejercicios **peso o tiempo** según tipo — útil para comunicar “planilla digital” frente a planillas en papel.

### 2.8 Pizarra virtual en sala (TV)

- **Reemplazo conceptual de la pizarra física** del gym: una **TV o monitor** muestra en **vivo** lo que el profesor va cargando o seleccionando desde el sistema.
- **Administración de esquemas reutilizables** (bloques o estructuras que se pueden reutilizar y **modificar en el acto**).
- **Nombres personalizables** de esquemas o bloques para que el lenguaje coincida con el gimnasio (clase WOD, circuito, bloque A/B, etc.).
- Mensaje comercial: *“El alumno en sala ve lo mismo que el profesor controla desde la notebook o tablet.”*

### 2.9 Administrar el sistema (módulo consolidado)

Incluir en el pitch como bloque **“Administración del sistema”**:

| Tema | Qué comunicar |
|------|----------------|
| **Página pública** | Mismo bloque que la sección 1: todo centralizado. |
| **Backup** | Existencia de flujo de **respaldo de datos** (detalle técnico según contrato: frecuencia, almacenamiento, restauración). |
| **Usuarios y contraseñas** | Gestión de staff, recuperación / cambio de claves según roles y políticas. |
| **Depuración / limpieza de datos** | Herramientas o procedimientos para entornos de prueba o mantenimiento (ajustar según producto final comercializado). |
| **Manual de usuario** | Documentación integrada (**HTML del manual**) para capacitación interna del gimnasio y reducción de soporte. |

### 2.10 Dominio, servidor y propiedad (mensaje comercial + qué va en el precio)

**Quién paga el recurrente (claridad):** el **abono del servidor** (hosting, VPS, etc.) y la **renovación del dominio** los contrata y paga **el cliente**, a su nombre, con el proveedor que elija. Vos **no** actuás como intermediario que factura hosting y lo repaga a un tercero (transparencia, sin margen opaco en infra).

**Incluido en el precio del proyecto (oferta comercial acordada):**

| Incluye | Detalle |
|--------|--------|
| **Asesoramiento** | Ayuda para **elegir y comprar** el servidor adecuado al volumen esperado y al presupuesto. |
| **Configuración del servidor** | Dejar el entorno listo para la aplicación (según stack acordado). |
| **Subida de la app y despliegue** | Publicación en producción y verificación de que el sistema queda operativo. |
| **Configuración del dominio** | Enlace del dominio al servidor (DNS, certificados SSL si aplica, etc.). |
| **Soporte post–puesta en marcha** | **1 mes de soporte** desde “**en producción**”: **limar y verificar** el funcionamiento de lo ya entregado (bugs, ajustes finos de pantalla, dudas de uso del alcance acordado). |

**Alcance del mes de soporte (dejar explícito en contrato y presupuesto):**

- **Sí incluye:** corrección de errores de lo desplegado, pequeños ajustes para que lo pactado funcione bien en producción, aclaraciones sobre el uso del sistema entregado.
- **No incluye:** **módulos nuevos**, funcionalidades que no estaban en el alcance del proyecto, integraciones nuevas, rediseños grandes ni **codificación extensa**. Eso se cotiza aparte como **nuevo desarrollo** o **pack de horas**.

**Propiedad y autonomía (marketing):** al cerrar la entrega, **aplicación, dominio y entorno** quedan **bajo control del cliente** (cuentas a su nombre). El gimnasio **no depende** del desarrollador para que el sitio siga online en el día a día: renueva dominio y servidor con sus proveedores; si quiere, otro técnico puede tomar el relevo con el código y documentación acordados — **cero lock-in**, **soberanía de marca y datos**.

**Nota interna:** seguís sin ser el **dueño del contrato de hosting** ni el que cobra el recurrente al gym; sí incluís el **trabajo** de asesorar, configurar, desplegar y **un mes** de **pulido y verificación** (no es backlog de features). Después del mes, todo fuera de ese alcance es **presupuesto aparte**.

---

## 3. Sugerencias extra para tu plan de marketing (PDF, folletos, videos)

1. **Propuesta de valor en una frase:** “Gimnasio ordenado: web que vende + panel que entrena y hace seguimiento.”  
2. **Dolor que resuelve:** menos Excel, menos PDFs perdidos, menos “te paso la rutina por WhatsApp” sin control de versión.  
3. **Prueba social / casos:** espacio para logo de gimnasios piloto o testimonios (rellenar cuando los tengas).  
4. **Demo en vivo:** 15 minutos: landing → login → alumno → asignar rutina → abrir enlace en celular → pizarra en TV.  
5. **Roles claros:** quién es ADMIN vs ayudante en el día a día del gym.  
6. **Privacidad y datos médicos:** mensaje prudente (“campos para observaciones; el gym es responsable del uso conforme ley local”).  
7. **Paquetes comerciales:** “Solo Mattfuncional” vs “Mattfuncional + MiGym Virtual” para trainers independientes que también llevan gimnasio.  
8. **Onboarding:** checklist “primera semana”: cargar logo, 3 fotos, WhatsApp, 2 planes, 5 alumnos, primera rutina.  
9. **Soporte:** canal de contacto (correo del desarrollador ya documentado en login/manual para incidencias).  
10. **Roadmap suave (opcional):** integraciones futuras, app nativa, pagos online — solo si son reales para no comprometer ventas.  
11. **Propiedad y hosting (§2.10):** en presupuestos el **pack incluido** vs **recurrente** cliente; y **límites del mes de soporte** (limar/verificar lo entregado; **sin** módulos nuevos ni codificación extensa).

---

## 4. Checklist para pegar en la otra sesión de Cursor

- [ ] Este archivo: `resumen_app_mattfuncional.md`  
- [ ] Resumen equivalente de **MiGym Virtual**  
- [ ] HTML manual Mattfuncional: `src/main/resources/templates/profesor/manual-usuario.html`  
- [ ] HTML manual MiGym Virtual (ruta según ese repo)  
- [ ] Objetivo del entregable: **PDF**, **carpeta de presentación**, **guion de video 60s / 3 min**, **folleto A4 triptych**, etc.  
- [ ] Tono de marca: formal / cercano / técnico  
- [ ] Precio o rangos (si ya los definís) para que la IA no invente números  
- [ ] Texto explícito §2.10: recurrente cliente; pack incluido + **1 mes soporte** = solo **limar/verificar** app en producción (**no** módulos nuevos ni código extenso); **propiedad / sin lock-in**

---

## 5. Para el otro chat — qué revisar o completar (opcional)

Con las secciones 1–4 y **§2.10 (dominio/servidor/propiedad)** **alcanza** para armar material serio. Si el otro chat quiere **profundizar sin inventar**, puede:

- **Contrastar** cada bullet con el HTML del manual y corregir wording si el producto cambió.
- **Definir audiencias:** solo dueño de gimnasio vs decisor + encargado operativo (copy distinto para PDF vs folleto).
- **Afinar límites** (§2.10 ya delimita soporte: no módulos nuevos / no código extenso; revisar horarios de respuesta y cantidad de usuarios si aplica).
- **Glosario de una página:** alumno vs usuario del sistema, asignación vs rutina plantilla, ACTIVA/INACTIVA — reduce confusiones en videos.
- **SEO y redes:** título/meta descripción sugeridos para la landing pública (si vendés implementación).
- **Comparativa breve** con “hacerlo a mano” (Excel/WhatsApp) sin nombrar competidores SaaS, si el canal es conservador.

Si nada de eso aplica, **no hace falta agregar nada más** al resumen.

---

*Documento generado para uso interno de marketing y briefs. Ajustar cifras y textos legales según la oferta comercial final.*
