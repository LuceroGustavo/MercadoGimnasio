# Carpeta «para insertar al mercado»

**Propósito:** un solo lugar para que Cursor (este repo o el del trabajo) lea **contexto comercial** + manuales y para ir guardando **prompts**, **bocetos**, **imágenes** y entregables (PDF, copy, guiones) sin mezclar con el código fuente.

## Contenido fijo de referencia

| Archivo | Uso |
|--------|-----|
| `resumen_app_mattfuncional.md` | Pitch y puntos para **gimnasio / administración completa**. |
| `resumen_app_migym_virtual.md` | Pitch para **personal trainer / solo rutinas online** (sin calendario ni pizarra). |
| `manual-usuario-Mattfuncional.html` | Manual embebible / pegable en otras herramientas. |
| `manual-usuario_MiGymvirtual.html` | Igual para MiGym Virtual. |

**Sincronización:** si editás los resúmenes en la **raíz** del repo (`resumen_app_*.md`), copiá también acá para que quien lea solo esta carpeta vea la última versión.

## Cómo seguimos trabajando (vos + Cursor)

1. **En el trabajo:** abrí el proyecto (o esta carpeta) en Cursor y pedí que use como contexto **`para insertar al mercado/`**.  
2. **Acá (Mattfuncional):** seguís el mismo flujo: pegás prompts, pedís textos para folleto, tablas para PDF, etc.  
3. **Cuando tengas imágenes:** subilas a esta carpeta (por ejemplo `imagenes/mattfuncional/`, `imagenes/migym/`) o indicá la ruta en el mensaje; en el prompt decís qué archivo tocar o qué pieza generar (caption, slide, etc.).  
4. **Dos carpetas de app (recomendado):** dentro de esta misma carpeta podés crear, cuando quieras:  
   - `entregables_mattfuncional/` — PDF, guiones, listas de precios, borradores.  
   - `entregables_migym_virtual/` — lo mismo para el segundo producto.  

No hace falta crearlas hasta que tengas material; Cursor puede crearlas al primer archivo que guardemos.

## Prompt útil para pegar en Cursor (trabajo u hogar)

```
Usá como contexto principal la carpeta: para insertar al mercado/
Incluí los resúmenes .md y los manual-usuario*.html al razonar.
Objetivo: [ej. guion video 90s Mattfuncional / folleto A4 MiGym Virtual].
Tono: [formal / cercano]. No inventes precios ni funciones que no figuren en esos archivos.
```

---

*Última idea: si un día esta carpeta crece mucho, considerá `.gitignore` parcial solo para binarios pesados; los `.md` y HTML suelen conviene versionarlos.*
