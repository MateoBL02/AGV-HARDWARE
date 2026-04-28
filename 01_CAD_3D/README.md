# 01 — Diseño CAD 3D

Contiene los archivos de diseño tridimensional del AGV completo para manufactura y ensamble final.

## Subcarpetas

### `partes/`
Archivos CAD individuales de cada componente diseñado o adaptado:
- Chasis principal
- Soportes de motores
- Mecanismo de elevación (tornillo sin fin + plataforma)
- Ruedas / orugas
- Soportes de sensores (QTR-8A, TCS34725)
- Soporte de la PCB y electrónica
- Otros elementos estructurales

### `ensambles/`
Ensambles completos del AGV:
- Ensamble general del vehículo
- Subensamble del sistema de tracción
- Subensamble del sistema de elevación

## Formatos aceptados
- `.STEP` / `.STP` — intercambio entre herramientas CAD (preferido)
- `.STL` — para impresión 3D
- `.f3d` — Fusion 360
- `.SLDPRT` / `.SLDASM` — SolidWorks

## Notas
- Todos los archivos deben incluir el nombre del componente y versión en el nombre del archivo.
- Ejemplo: `chasis_principal_v1.step`, `ensamble_general_v2.step`
