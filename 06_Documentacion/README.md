# 06 — Documentación del Proyecto

Documentos técnicos y de gestión del subsistema AGV Hardware.

## Documentos incluidos

| Archivo | Descripción |
|---------|-------------|
| `IBD_Hardware.pdf` | Internal Block Diagram — arquitectura del hardware del AGV |
| `Especificacion_Tecnica_Pflichtenheft.pdf` | Especificación técnica (Pflichtenheft) — descripción funcional, análisis técnico y BOM preliminar |
| `Esquematico_Diseno2.pdf` | Esquemático eléctrico completo del sistema |

## Información del proyecto

- **Proyecto:** AS/RS Automatizado
- **Grupo:** G2 — AGV Hardware
- **Universidad:** Universidad de Pamplona
- **Integrantes:**
  - Ivan Briceño
  - Carlos Adame
  - Andres Tolosa
  - Mateo Barragan
  - Cristian Becerra

## Resumen técnico

- **Microcontrolador:** ESP32-S3-DevKitC-1 WROOM-1 N16R8
- **Tracción:** 4x Motor N20 12VDC 200RPM con encoder Hall — control diferencial tipo oruga
- **Elevación:** 1x Motor N20 + tornillo sin fin
- **Drivers:** 3x TB6612FNG (izquierdo, derecho, plataforma)
- **Sensores:** QTR-8A (línea), TCS34725 (color), encoders, final de carrera
- **Alimentación:** LiPo 3S → MP23070N (5V) → regulador 3.3V interno ESP32
- **Comunicación:** WiFi (ESP32 integrado)
- **Corriente total estimada:** ~3.4A (operación continua)
- **Autonomía estimada:** ~40 minutos con batería 2500 mAh
