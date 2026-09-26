# RefinIA

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.22215864.svg)](https://doi.org/10.5281/zenodo.22215864)

**Aplicación:** https://fborrasumh.github.io/refinia/

Revisa un **manuscrito académico** (artículo, tesis o TFM) como lo haría un evaluador exigente, y comprueba con cálculos y fuentes reales la **exactitud de sus afirmaciones**. Aplicación de un solo fichero, sin servidor.

## Novedades de la versión 2.0

- Interfaz guiada con el estilo de Forja y un manuscrito de ejemplo con 14 errores sembrados.
- **Módulo de exactitud**, con comprobaciones que no dependen de la IA:
  - **Estadística recalculada**, al estilo de statcheck: recalcula el valor p a partir de t, F, χ², r y z con sus grados de libertad, teniendo en cuenta el redondeo. Distingue los errores que cambian la conclusión.
  - **Coherencia numérica**: porcentajes que no cuadran con su recuento, estimaciones fuera de su IC 95 % e IC que contradicen al valor p.
  - **Citas y referencias**: cada referencia se busca en OpenAlex y Crossref para detectar las inexistentes, las retractadas y los errores de año, autor o DOI. También marca citas sin referencia y referencias no citadas.
- **Afirmación frente a fuente**: un agente compara lo que se atribuye a un trabajo con su resumen real y, si el resumen no basta, lo declara.
- **Modo «Solo exactitud»**: funciona sin clave y sin coste.
- Panel «Exactitud» con un índice de 0 a 100. Si una lente y el cálculo exacto señalan lo mismo, prevalece el cálculo.
- **Corregido**: el segmentador no reconocía los títulos pegados a su párrafo, y la sección asignada a cada comentario era la del pasaje entero en lugar de la de su frase.

## Motor de lectura

Seis lentes en paralelo (exactitud y datos, razonamiento matemático, método y estadística, consistencia, referencias y argumentación), una pasada de consistencia entre secciones y un verificador anti-ruido. Cada comentario se ancla a su cita literal. Incluye resolución en el documento con evidencia de OpenAlex, chat de seguimiento, comparación con la versión revisada y exportación a Markdown, Word y JSON, además de una carta de respuesta a los revisores.

## Privacidad

El texto va del navegador a OpenAI; las referencias se consultan en OpenAlex y Crossref. No hay servidor intermedio. La clave se guarda en `localStorage` (`ia_openai_key`) y las revisiones en IndexedDB.

## Cómo citar

Borrás Rocher, F. (2026). *RefinIA* (versión 2.0.0) [Software]. Universidad Miguel Hernández de Elche. https://doi.org/10.5281/zenodo.22215864

El DOI anterior es el de concepto: apunta siempre a la última versión. El DOI de cada versión concreta está en [Zenodo](https://doi.org/10.5281/zenodo.22215864). GitHub ofrece la cita en formato APA y BibTeX con el botón *Cite this repository*, a partir de `CITATION.cff`.

Forma parte del catálogo [Herramientas IA para la academia](https://fborrasumh.github.io/ia/).

## Licencia

MIT © 2026 Fernando Borrás Rocher · Universidad Miguel Hernández de Elche.
