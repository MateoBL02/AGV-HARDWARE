# 04 — BOM (Bill of Materials) Definitivo

Listado completo de materiales y componentes necesarios para la siguiente etapa de fabricación del AGV. Incluye tanto los componentes ya existentes como los nuevos.

## Archivo BOM

El BOM definitivo debe entregarse en formato `.xlsx` o `.pdf` con la siguiente estructura:

| # | Componente | Referencia | Cantidad | Función | Especificación clave | Estado |
|---|-----------|-----------|---------|---------|---------------------|--------|
| 1 | Microcontrolador | ESP32-S3-DevKitC-1 WROOM-1 N16R8 | 1 | Control general | WiFi, 3.3V, ADC, PWM | Existente |
| 2 | Driver motor | TB6612FNG | 3 | Control de motores | 15V / 1.2A continuo/canal | Existente |
| 3 | Motor DC con encoder | N20 Hall 12VDC 200RPM | 5 | Tracción (x4) + Elevación (x1) | Torque bloqueado >1.2 kg·cm | Existente |
| 4 | Sensor línea | QTR-8A | 1 | Seguimiento de trayectoria | 8 IR analógico, 5V | Existente |
| 5 | Sensor color | TCS34725 | 1 | Detección de color | I2C, 3.3V | Existente |
| 6 | Regulador voltaje | MP23070N | 1 | 12V → 5V/3.3V | Hasta 3A salida | Existente |
| 7 | Batería | LiPo 3S 2500mAh | 1 | Alimentación principal | 11.1V–12.6V, ~40 min autonomía | Existente |
| 8 | Conector batería | XT60 | 1 | Conexión batería | — | Existente |
| 9 | Final de carrera | Microswitch COM/NO/NC | 1 | Límite elevación | — | Existente |
| 10 | Conectores I2C | Male Header 4 pines | 2 | Expansión I2C | GND/VCC/SCL/SDA | Existente |

> Este BOM es preliminar. Actualizar con cantidades exactas, referencias de proveedor y precios para la entrega final.
