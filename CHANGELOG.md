# Cambios

## v1.0.0 — 2026-08-31

Primera versión pública de RefinIA.

- Ingesta de manuscritos en PDF (pdf.js), DOCX (mammoth) o texto pegado, con
  reconstrucción de párrafos y detección de secciones.
- Revisión por seis lentes independientes en paralelo: exactitud y datos,
  razonamiento matemático, método y estadística, consistencia interna,
  referencias y atribución, argumentación y claridad.
- Pasada de consistencia entre secciones sobre el esqueleto factual del
  documento (afirmaciones, cifras y definiciones con cita literal).
- Verificador que descarta hallazgos no sostenidos, genéricos o duplicados.
- Anclaje de cada comentario a su posición exacta en el texto, con espina
  lateral de densidad de problemas.
- Gestión de comentarios (resuelto / descartado), chat de seguimiento y
  comprobación de la versión revisada comentario a comentario.
- Exportación a Markdown, Word, JSON y borrador de carta de respuesta.
- Persistencia local en IndexedDB. Clave de OpenAI en localStorage.
