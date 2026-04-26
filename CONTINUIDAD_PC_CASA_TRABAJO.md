# Continuidad entre PC (casa) y trabajo — Cursor y GitHub

**Propósito:** este archivo es el **puente** entre dos máquinas y dos **chats distintos** de Cursor. Lo que se haga en **PC de casa** queda registrado aquí (y en el resto del repo) para que el chat de **Cursor en el trabajo** pueda seguir sin perder contexto.

---

## Acuerdo de trabajo

| Dónde | Rol |
|--------|-----|
| **Este repositorio en la PC de casa** | Desarrollo / redacción / material comercial que hagamos desde casa. **Actualizar este documento** cuando cierre una sesión importante o antes de cambiar de máquina. |
| **PC del trabajo + otro chat de Cursor** | Continuar leyendo **este archivo primero**, luego `LEEME.md` y los resúmenes/manuales indicados abajo. |
| **GitHub** | Fuente de verdad compartida. **Al terminar una sesión** (casa o trabajo): `git pull` al abrir, trabajo local, **`git push`** al cerrar para que la otra PC vea todo actualizado. |

---

## Contexto del proyecto (una línea)

Plan comercial y práctica para **insertar en el mercado dos productos**: **Mattfuncional** (gimnasio / administración completa + página pública + pizarra TV + calendario, etc.) y **MiGym Virtual** (personal trainer / rutinas online, sin calendario tipo gym ni pizarra). Misma base técnica en gran medida; el marketing los diferencia según `resumen_app_*.md`.

---

## Archivos de contexto fijos en la raíz (léelos en Cursor en cualquier PC)

- `LEEME.md` — propósito de la carpeta, flujo con Cursor, prompt sugerido.
- `resumen_app_mattfuncional.md` — pitch y detalle comercial Mattfuncional.
- `resumen_app_migym_virtual.md` — pitch MiGym Virtual y diferencias vs Mattfuncional.
- `manual-usuario-Mattfuncional.html` — manual usuario (referencia / pegable).
- `manual-usuario_MiGymvirtual.html` — idem MiGym Virtual.
- `para insertar al mercado/` — carpeta viva: entregables Mattfuncional (plan maestro, `00_fuente_texto/`, guías, prompts NotebookLM, etc.); leé `LEEME.md` dentro o en la raíz según dónde abras el repo.

**Nota:** los **resúmenes** y **manuales** siguen en la **raíz**; el **kit de salida al mercado** (textos por bloque, imágenes, prompts) vive bajo `para insertar al mercado/entregables_mattfuncional/`. Si movés rutas, actualizá una línea aquí o en `LEEME.md`.

---

## Prompt corto para pegar en Cursor (trabajo u hogar)

```
Leé primero CONTINUIDAD_PC_CASA_TRABAJO.md y LEEME.md.
Usá como contexto: resumen_app_*.md, manual-usuario*.html y, si el trabajo es Mattfuncional comercial, para insertar al mercado/entregables_mattfuncional/ (PLAN_MAESTRO, 00_fuente_texto, prompts).
Objetivo: [describir la tarea del día].
No inventes precios ni funciones que no figuren en esos documentos.
```

---

## Bitácora (rellenar al cerrar sesión en casa o en trabajo)

_Escribí aquí una línea por sesión: fecha, PC (casa/trabajo), qué quedó hecho y qué sigue._

| Fecha | PC | Hecho | Siguiente paso |
|--------|-----|--------|-----------------|
| 2026-04-23 | casa | Creado este archivo de continuidad; lectura de toda la documentación de raíz | Completar filas siguientes en cada sesión; push a GitHub |
| 2026-04-24 | trabajo | Relectura completa de documentación (`LEEME`, resúmenes y manuales) para plan de inserción al mercado; confirmado flujo de trabajo entre dos PCs con GitHub como puente. Además se creó `para insertar al mercado/entregables_mattfuncional/` con plan maestro, guía de imágenes y prompts base para NotebookLM | Completar materiales reales (capturas por módulo + texto fuente) y generar PDF v1/video v1; cerrar sesión con `git push` para continuidad en PC casa |
| 2026-04-24 | casa | Sincronización: lectura de toda la documentación y entregables desde trabajo; ajuste de `CONTINUIDAD` para alinear rutas con `para insertar al mercado/` | Completar materiales (capturas por módulo, PDF v1 en NotebookLM) según `PLAN_MAESTRO_MATTFUNCIONAL.md` |
| 2026-04-25 | casa | NotebookLM: generación de 4 PDF y 1 presentación tipo PowerPoint usando `00_fuente_texto/` + imágenes por bloque | Refinar versión final del instructivo/presentación y exportables definitivos |

---

*Última actualización relevante: 2026-04-25 (PC casa).*
