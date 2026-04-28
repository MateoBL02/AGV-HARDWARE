# AGV Hardware — Grupo 2 | Universidad de Pamplona

**Proyecto:** AS/RS Automatizado  
**Etapa:** Specification / Design  
**Grupo:** G2 — AGV Hardware  
**Integrantes:** Ivan Briceño, Carlos Adame, Andres Tolosa, Mateo Barragan, Cristian Becerra  
**Fecha:** Abril 2026

---

## Descripción del Subsistema

El AGV (Automated Guided Vehicle) implementa una arquitectura de tracción tipo oruga con control diferencial. Cada lado está conformado por dos motores DC N20 con reductor conectados en paralelo mecánico, controlados mediante puentes H TB6612FNG. El seguimiento de trayectoria se realiza con el sensor QTR-8A y la lógica de control corre en un ESP32-S3.

El sistema incluye:
- **Tracción diferencial** con 4 motores N20 (2 por lado)
- **Sistema de elevación** mediante tornillo sin fin accionado por un motor N20 adicional
- **Sensórica:** QTR-8A (seguimiento de línea), TCS34725 (color), encoders Hall magnéticos, final de carrera
- **Control:** ESP32-S3-DevKitC-1 WROOM-1 N16R8
- **Drivers:** 3x TB6612FNG
- **Alimentación:** Batería LiPo 3S (11.1V–12.6V) + regulador MP23070N (→ 5V/3.3V)
- **Comunicación:** WiFi

---

## Estructura del Repositorio

```
g2-agv-hardware/
├── 01_CAD_3D/              # Modelos 3D del AGV completo
│   ├── partes/             # Archivos CAD individuales de cada pieza
│   └── ensambles/          # Ensambles completos del AGV
├── 02_Planos_2D/           # Planos de fabricación con cotas y tolerancias (PDF)
├── 03_PCB_Electronica/     # Diseño eléctrico/electrónico
│   ├── esquematico/        # Esquemático del circuito (EasyEDA / KiCad)
│   └── layout/             # PCB Layout y ruteo
├── 04_BOM/                 # Bill of Materials definitivo
├── 05_Pruebas/             # Documentación de pruebas unitarias
│   ├── registros_escritos/ # Informes y registros escritos
│   ├── fotos/              # Registro fotográfico
│   └── videos/             # Registro en video
└── 06_Documentacion/       # Documentos del proyecto (IBD, Pflichtenheft, etc.)
```

---

## Actividades del Grupo

1. **Diseño 3D definitivo** del AGV completo — CADs de partes para manufactura y ensamble final.
2. **Ruteo PCB y Layout** eléctrico/electrónico de sensores, actuadores y componentes del subsistema.
3. **Pruebas unitarias** a las unidades existentes del AGV con documentación escrita, fotográfica y en video:
   - Sistema de traslación
   - Sistema de recolección de caja
   - Sistemas de detección de objetos
   - Sistema de control general

---

## Entregables

- Rama `g2-agv-hardware` en el repositorio central con archivos y documentos organizados.
- Planos 2D de fabricación con cotas, tolerancias y materiales — rótulo institucional (PDF).
- BOM definitivo con todos los componentes (existentes y nuevos).
- Archivos CAD completos: partes individuales y ensambles.
