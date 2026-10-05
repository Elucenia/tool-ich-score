<!-- ELUCENIA technical documentation · ich-score · es · no clinical/professional/rights approval -->

# Puntuación ICH

[condiciones, fuentes y permisos](https://elucenia.org/es/herramientas/ich-score)

## Cómo usar

Utilice la herramienta en el portal o abra index.html mediante un servidor HTTP local. Seleccione el idioma, complete los campos y calcule.

## Entradas y unidades

### Escala de coma de Glasgow

`gcs`

- `0` — 13 a 15
- `1` — 5 a 12
- `2` — 3 a 4

### Volumen del hematoma ≥ 30 mL (fórmula ABC/2)

`vol`

### Hemorragia intraventricular

`ivh`

### Origen infratentorial

`infra`

### Edad ≥ 80 años

`idade`

## Edición del método

ICH/Hemphill 2001: 5 factores, total 0–6; volumen ABC/2; sin decisión terapéutica automática

## Fórmula documentada

Glasgow 3 a 4 = 2 · 5 a 12 = 1 · 13 a 15 = 0; volumen ≥ 30 mL = 1; extensión ventricular = 1; origen infratentorial = 1; edad ≥ 80 años = 1. Total: 0 a 6.

Volumen por ABC/2: A = mayor diámetro en corte de mayor área; B = perpendicular a A; C = número de cortes con hematoma × grosor (cm). Resultado mL.

## Límites y población

Estimación de gravedad en la presentación de hemorragia intracerebral, asociada a mortalidad a 30 días en la cohorte original. La edad y el volumen son componentes de la puntuación. El resumen no demuestra que una puntuación aislada justifique una decisión terapéutica ni un pronóstico individual definitivo.

## Referencias

- [Hemphill JC 3rd et al. The ICH score: a simple, reliable grading scale for intracerebral hemorrhage. Stroke, 2001.](https://doi.org/10.1161/01.STR.32.4.891)

## Reproducir las pruebas técnicas

Ejecute node test.cjs en el directorio raíz de este repositorio para repetir los casos sintéticos registrados. Se conservan las entradas, los resultados esperados y las tolerancias originales. Las pruebas técnicas no constituyen validación clínica.

```sh
node test.cjs
```

tool.json contiene las fuentes, la edición y el alcance de la revisión. examples.json conserva las entradas y los resultados esperados de los casos sintéticos; results.json registra los resultados obtenidos.

[Ficha y referencias](../tool.json) · [Código JavaScript](../calculator.js) · [Casos de referencia](../examples.json) · [results.json](../results.json)

## Revisión y condiciones de uso

No se ha realizado una revisión clínica independiente.

Esta interfaz es una traducción de elaboración propia, no una edición oficial o certificada. No se han realizado la revisión clínica independiente, la revisión lingüística profesional ni la autorización de derechos de los instrumentos.

Resultado de la fórmula o clasificación. La interpretación, la conducta y la aplicabilidad dependen de la evaluación profesional y de la fuente seleccionada.

## Licencia y atribución

Apache-2.0 se aplica únicamente al código de ELUCENIA. Los derechos de los instrumentos, publicaciones, traducciones y datos permanecen en manos de sus respectivos titulares. Conserve LICENSE y NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026
