# 03 — PCB y Electrónica

Diseño eléctrico y electrónico del AGV: esquemático, ruteo de PCB y layout de conexiones.

## Componentes principales del sistema

| Componente | Función | Especificación |
|---|---|---|
| ESP32-S3-DevKitC-1 WROOM-1 N16R8 | Microcontrolador principal | WiFi, 3.3V, múltiples GPIO/ADC |
| TB6612FNG (x3) | Drivers puente H | Hasta 15V / 1.2A continuo por canal |
| Motor N20 con encoder Hall (x5) | Tracción (x4) + Elevación (x1) | 12VDC, 200 RPM |
| QTR-8A | Sensor seguidor de línea | 8 IR analógicos, 5V |
| TCS34725 | Sensor de color | I2C, 3.3V |
| MP23070N | Regulador buck 12V→5V | Alta eficiencia |
| Final de carrera (FC1) | Límite de elevación | COM/NO/NC |
| Batería LiPo 3S | Alimentación principal | 11.1V–12.6V / conector XT60 |

## Subcarpetas

### `esquematico/`
- Archivo fuente del esquemático (EasyEDA, KiCad, etc.)
- Exportación en PDF del esquemático completo
- Archivo fuente: `Esquematico_Diseño2` (EasyEDA)

### `layout/`
- Archivo de PCB con ruteo completo
- Gerbers para fabricación
- Imagen de la PCB (top y bottom layer)

## Asignación de pines ESP32-S3

| GPIO | Señal |
|------|-------|
| IO1 | enc1a |
| IO2 | enc1b |
| IO39 | enc2a |
| IO40 | enc2b |
| IO41 | enc3a |
| IO42 | enc3b |
| IO35 | enc4a |
| IO38 | enc4b |
| IO36 | enc5a |
| IO33 | enc5b |
| IO3 | enc1a (QTR) |
| IO8 | pwmplataforma |
| IO18 | in2plataforma |
| IO3 | in1plataforma |
| IO9 | pwmizquierdo |
| IO10 | in2izquierdo |
| IO11 | in1izquierdo |
| IO12 | pwmderecho |
| IO13 | in2derecho |
| IO14 | in1derecho |
| IO4 | SDASC (TCS34725) |
| IO5 | SCLSC (TCS34725) |
| IO15 | FC1 (final de carrera) |
| IO16 | SCL (I2C general) |
| IO17 | SDA (I2C general) |
