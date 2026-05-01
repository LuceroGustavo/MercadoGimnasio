# Plan maestro — versión liviana (personal trainers / online)

**Producto técnico de referencia:** MiGym Virtual (misma base que la app de gimnasio, sin módulos de sala).

**Nombre comercial:** definir nombre corto para venta (ej. “MiGym Virtual”, “Tu app de rutinas”, etc.). En documentación interna seguir usando `resumen_app_migym_virtual.md` y `manual-usuario_MiGymvirtual.html`.

**Contraste con “App administración de gimnasio”:** esta versión es para **entrenador personal / negocio online**: rutinas, seguimiento y web propia; **no** se promete calendario tipo grilla de gimnasio, **ni** pizarra en TV, **ni** narrativa fuerte de presentismo de sala.

## 1) Objetivo comercial

- Vender una solución **simple y clara**: web + panel + rutinas por enlace + WhatsApp.
- Público: **personal trainers**, coaches online, estudios sin operación de sala tipo gym.

## 2) Entregables mínimos (igual que el otro producto, pero más cortos)

1. PDF principal (8–12 páginas o equivalente).
2. Presentación corta (PowerPoint / NotebookLM).
3. 3–6 reels o microvideos (un beneficio por pieza).
4. Opcional: audio resumen corto (NotebookLM).

## 3) Materia prima en esta carpeta

- `00_fuente_texto/` — un `.txt` por bloque del índice; imágenes con el **mismo número** de bloque.
- `02_prompts_notebooklm/` — prompts para PDF / diapositivas / audio.
- Cuando exista: `01_imagenes_por_modulo/` y `03_exportables/` (versiones finales).

## 4) Checklist

- [ ] Completar textos en `00_fuente_texto/` según `0- indice de bloques.txt`.
- [ ] Capturas reales **solo** de pantallas que existen en MiGym Virtual (sin calendario gym ni pizarra).
- [ ] Revisar que el copy no mencione módulos excluidos (ver tabla en `resumen_app_migym_virtual.md`).
- [ ] Generar PDF + presentación en NotebookLM.
- [ ] Exportar reels y dejar copia en `03_exportables/`.
- [ ] Actualizar `CONTINUIDAD_PC_CASA_TRABAJO.md` y `git push`.

## 5) Reglas de calidad

- No inventar funciones ni precios.
- No prometer **calendario semanal tipo gimnasio**, **pizarra en TV** ni **modalidad presencial/semipresencial** como en la app de gimnasio completa.
- Enfatizar **página pública** + **redes** + **rutina por enlace** + **seguimiento**.
