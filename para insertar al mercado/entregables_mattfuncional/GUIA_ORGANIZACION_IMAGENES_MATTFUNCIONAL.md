# Guia de imagenes por modulo - Mattfuncional

Objetivo: que NotebookLM entienda rapido cada bloque del producto.

## 1) Regla de nombrado

Formato:
`modulo_nombre-numero.ext`

Ejemplos:
- `panel_profesor-01.png`
- `panel_profesor-02.png`
- `pizarra_tv-01.png`
- `rutinas_asignaciones-01.png`

## 2) Modulos recomendados (carpetas)

Crear dentro de `01_imagenes_por_modulo/`:
- `panel_profesor/`
- `alumnos/`
- `rutinas_y_asignaciones/`
- `calendario_presentismo/`
- `pizarra_tv/`
- `pagina_publica/`
- `administracion_sistema/`

## 3) Cantidad sugerida por modulo

- Minimo: 3 imagenes por modulo.
- Ideal: 5 a 8 imagenes por modulo.
- Incluir al menos:
  - vista general
  - accion clave (ej: asignar rutina)
  - resultado final (ej: link de rutina o TV)

## 4) Calidad visual recomendada

- Capturas limpias, sin elementos personales sensibles.
- Misma resolucion o resoluciones cercanas.
- Evitar texto cortado y zonas borrosas.
- Si agregas imagenes generadas (Nano Banana), marcarlo en nombre:
  - `pizarra_tv_mock-01.png`

## 5) Plantilla rapida de inventario

Copiar y completar en un txt por modulo:

- Modulo:
- Objetivo visual:
- Archivos:
  - archivo 1:
  - archivo 2:
  - archivo 3:
- Mensaje clave del modulo:

## 6) Error comun a evitar

No mezclar capturas de distintos modulos con nombres genericos como
`foto1.png`, `captura2.png`. Eso complica mucho la salida de NotebookLM.
