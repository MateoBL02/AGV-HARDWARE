# 05 — Pruebas Unitarias

Documentación de las pruebas realizadas a las unidades existentes del AGV. Incluye registros escritos, fotográficos y de video.

## Sistemas a probar

| Sistema | Descripción |
|---------|-------------|
| Sistema de traslación | Prueba de movimiento recto, giro, velocidad y seguimiento de línea |
| Sistema de elevación | Prueba de subida/bajada de plataforma, final de carrera, carga máxima |
| Detección de objetos | Prueba del sensor de color TCS34725 y sensor QTR-8A |
| Sistema de control general | Prueba de comunicación WiFi, latencia, respuesta PWM |

## Estructura de cada registro de prueba

Cada prueba debe documentarse con:

1. **Nombre de la prueba**
2. **Fecha y responsable**
3. **Objetivo**
4. **Procedimiento paso a paso**
5. **Resultados obtenidos** (valores medidos, comportamiento observado)
6. **Criterio de aceptación / fallo**
7. **Conclusión**
8. **Evidencia:** fotos y video referenciados

## Subcarpetas

### `registros_escritos/`
Informes en PDF o DOCX de cada prueba realizada.
- Ejemplo: `prueba_traccion_01.pdf`, `prueba_elevacion_01.pdf`

### `fotos/`
Fotos organizadas por sistema y fecha.
- Ejemplo: `traccion_prueba1_01.jpg`

### `videos/`
Videos de las pruebas. Pueden ser enlaces a Drive o archivos directos.
- Ejemplo: `prueba_seguimiento_linea_v1.mp4`
- O un archivo `links_videos.md` con los enlaces de YouTube/Drive.
