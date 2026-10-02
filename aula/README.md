# Aula de entrenamiento — piloto Turbulencia

Primera clase integrada al inicio de EBT Manager. Ruta: `/aula/`.

- Video aprobado de 590,866667 s, sin cambios en imagen ni narración.
- Cinco pausas formativas, tres decisiones finales y transcripción por fragmentos.
- Historial de primer intento y último intento; repaso por tema.
- Avance de prueba en `localStorage` (`ebt-aula-turbulencia-v1`), solo en el navegador. No se escriben datos de aprendizaje en Supabase ni se modifican los registros del planificador.
- Los porcentajes de video visto cuentan intervalos reproducidos y no acreditan competencia operacional.

## Archivos

`contenido.js`: capítulos, tiempos de la narración y banco formativo.
`aula.js`: reproducción, pausas, rutas y persistencia local.
`aula.css`: interfaz responsive, Avianca rojo/blanco/negro.

El video original se distribuye en 30 partes binarias de hasta 900 000 bytes. `assets/video.json` describe su orden y tamaño. El reproductor descarga cuatro partes a la vez y reconstruye el MP4 exacto como Blob local, conservado mientras la página siga abierta. No hay transcodificación. La primera entrada a la clase requiere descargar unos 27 MB antes de reproducir; en una fase de operación a escala conviene sustituirlo por un servicio de streaming con acceso acorde al portal.

Antes de uso formal: validación del banco por responsables de entrenamiento y definición de identidad del participante, trazabilidad y criterios de finalización. El piloto no entrega certificaciones ni calificaciones al registro EBT.
