# Resumen MiGym Virtual — marketing y presentación (personal trainer / envío de rutinas)

**Carpeta de trabajo mercado:** `para insertar al mercado/` — ver `LEEME.md` para coordinar prompts e imágenes entre este repo y Cursor en el trabajo.

**Uso sugerido:** pegar en otra sesión de Cursor junto con **`resumen_app_mattfuncional.md`**, el **manual de usuario HTML** de MiGym Virtual (y el de Mattfuncional si comparás productos) y el brief de marca. Sirve para PDF, folletos, videos y material con IA.

**Producto:** **MiGym Virtual** — misma **base técnica y de experiencia** que **Mattfuncional**, pero **enfocada solo en el envío y la gestión de rutinas** para **entrenador personal** o negocios **100 % virtuales** (sin operación de sala tipo gimnasio con pizarra ni planificación semanal tipo grilla de gym).

**Relación con Mattfuncional:** quien ya conoce Mattfuncional entiende MiGym Virtual en minutos: **se quitan módulos** que no aplican al trainer online; **el resto del flujo es el mismo** (ejercicios, series, rutinas, asignaciones, hoja pública por enlace, WhatsApp, panel, administración del sistema, manual).

**Manual de usuario (ruta típica en el repo MiGym Virtual):** `src/main/resources/templates/profesor/manual-usuario.html` — *ajustar si tu copia del proyecto usa otra ruta.*

---

## 1. Página pública — misma base, perfil “trainer / online”

La landing sigue siendo la **cara del negocio**: carrusel, video, planes, contacto, WhatsApp, responsive y contenido administrable. **Diferencia clave frente a Mattfuncional “gimnasio”:**

### 1.1 Sin dirección física obligatoria desde administración

En muchos casos el **personal trainer** o el **studio online** no necesita mostrar **dirección del local** como eje central (no hay “sala” o se trabaja remoto). Al **no depender** de un bloque fuerte de “dirección del gimnasio” desde el panel, la página pública puede **destinar más espacio visual y de configuración a redes y presencia digital**.

### 1.2 Redes sociales ampliadas (mensaje comercial)

Más margen para enlazar las redes **más usadas por el trainer** para captar leads:

- **Instagram**, **TikTok**, **YouTube**, **Facebook**, y otras que definan en la implementación (enlaces configurables en la misma lógica de “marca + contacto” que la app de referencia).

**Pitch:** *“Tu web vende tu método y te lleva a Instagram, TikTok o YouTube desde un solo lugar, sin que tengas que ser diseñador web.”*

### 1.3 Resto del paquete público (igual que la referencia)

- Carrusel, video hero (desktop/móvil), planes y promociones, imágenes, formulario de consulta, WhatsApp, **100 % responsive**, **administración desde el panel** sin desarrollador para el día a día de promos y textos.

---

## 2. Panel de administración — lo mismo que Mattfuncional, salvo lo que no lleva

**Misma idea:** panel **rápido y dinámico**; alumnos consumen rutina por **enlace web** (sin instalar app). Staff con usuarios propios (ADMIN / AYUDANTE / DEVELOPER según implementación).

### 2.1 Lo que **no** incluye MiGym Virtual (diferencias explícitas)

| No incluye | Motivo comercial |
|------------|------------------|
| **Calendario semanal** | El foco es **rutina y seguimiento**, no la grilla de ocupación de sala de un gimnasio. |
| **Pizarra digital en TV** | No hay narrativa de “clase en sala”; el alumno entrena **con su enlace** donde esté. |
| **Modalidad presencial / semipresencial del alumno** | El producto se plantea con alumnos en modalidad **virtual** (entrenamiento a distancia / seguimiento online). *No prometer turnos de piso ni presentismo de gym como en Mattfuncional completo.* |

### 2.2 Lo que **sí** se mantiene (igual que la app de referencia)

- **Usuarios del sistema** (alta, edición, roles, contraseñas).
- **Alumnos:** carga, ficha, edición, estado; datos útiles (objetivo, observaciones, fecha de nacimiento / edad, contacto, etc.) — **enfoque virtual** en el discurso comercial.
- **Seguimiento de progreso** (anotaciones, evolución en ficha).
- **Ejercicios** (predeterminados + propios, imágenes/video, grupos musculares).
- **Series** y **rutinas** (plantillas, orden, peso/reps/tiempo según diseño actual).
- **Asignaciones** con **enlace público**, ACTIVA/INACTIVA, WhatsApp, **sin instalación** para el alumno.
- **Dashboard** con resumen (alumnos, series, rutinas — *sin tarjeta de calendario semanal ni acceso a pizarra*).
- **Administrar el sistema:** página pública, backups, usuarios, depuración según alcance, **manual de usuario**.

### 2.3 Mensaje para folleto / comparativa con Mattfuncional

> *“MiGym Virtual es tu versión online: misma potencia en rutinas y contenido, sin lo que solo usa un gimnasio con sala (calendario de piso y pizarra en TV).”*

---

## 3. Dominio, servidor y propiedad (misma política que Mattfuncional)

**Recurrente:** hosting + dominio **a nombre y cargo del cliente**; sin intermediación opaca del desarrollador.

**Incluido en el precio del proyecto (si mantenés el mismo paquete que Mattfuncional):** asesoramiento compra servidor, configuración, deploy, dominio/DNS, **1 mes de soporte** post–producción para **limar y verificar** lo entregado.

**Alcance del mes de soporte:** igual que Mattfuncional — **sí** bugs y ajustes finos de lo pactado; **no** módulos nuevos, **no** codificación extensa, **no** features fuera de alcance (presupuesto aparte).

**Propiedad:** aplicación y entorno bajo **control del cliente**; mensaje **sin lock-in**.

---

## 4. Sugerencias de marketing específicas para MiGym Virtual

1. **Cliente ideal:** trainer independiente, nutricionista–coach, box online, rehabilitación a distancia.  
2. **Demo corta:** landing → login → crear/editar rutina → asignar → abrir enlace en el celular (sin pasos de pizarra ni calendario).  
3. **Bundle comercial:** “Mattfuncional en el gym + MiGym Virtual para tus clientes online” si vendés ambos.  
4. **Contenido social:** el copy de la landing puede insistir en **TikTok / Reels / Shorts** como canal de captación enlazado desde la web.

---

## 5. Checklist para la otra sesión de Cursor

- [ ] Este archivo: `resumen_app_migym_virtual.md`  
- [ ] `resumen_app_mattfuncional.md` (para comparativas)  
- [ ] Manual HTML **MiGym Virtual** (ruta real del repo)  
- [ ] Objetivo del entregable (PDF, video, folleto, etc.)  
- [ ] Confirmar en código qué redes están cableadas en la página pública (no inventar iconos o campos que aún no existan)

---

## 6. Para el otro chat — revisión rápida

- Contrastar “**solo virtual**” y ausencia de **calendario / pizarra** con el manual real del repo MiGym Virtual.  
- Si en el código aún figuran filtros o textos de “presencial”, unificar **wording comercial** con lo que muestra la app.  
- Listar **URLs exactas** de redes que el panel permita guardar (Instagram, TikTok, etc.) según la plantilla `index-publica` / admin de ese proyecto.

---

*Documento orientado a marketing y briefs. Alinear siempre con el manual y el código del repo **MiGym Virtual** que subas.*
