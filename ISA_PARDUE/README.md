## ISA 95 vs Modelo de Pardue

El **Modelo Purdue** (oficialmente **Purdue Enterprise Reference Architecture** o PERA) y el **estándar ISA-95** (también conocido como IEC 62264) son dos referencias fundamentales en la automatización industrial y la integración entre sistemas de planta (OT) y sistemas empresariales (IT). Aunque se usan casi como sinónimos en la práctica diaria, **no son exactamente lo mismo**.

### Similitudes principales

- Ambos definen una **estructura jerárquica** (normalmente representada como una pirámide) con **niveles** (levels) que van desde los procesos físicos hasta los sistemas de negocio.
- Comparten **prácticamente los mismos niveles** (0 a 4 o 0 a 5 según la versión):
  - **Nivel 0** — Procesos físicos reales (máquinas, materiales, energía)
  - **Nivel 1** — Sensores, actuadores e instrumentación de campo
  - **Nivel 2** — Control supervisado (SCADA, HMI, sistemas de control de procesos)
  - **Nivel 3** — Sistemas de ejecución de manufactura (MES), gestión de operaciones de planta
  - **Nivel 4** — Sistemas empresariales (ERP, planificación logística, finanzas)
  - (A veces se menciona **Nivel 5** — Sistemas externos / nube / partners)
- Ambos sirven para:
  - Estandarizar el lenguaje entre proveedores, integradores y usuarios finales.
  - Facilitar la **segmentación de redes** y la **ciberseguridad** (defensa en profundidad).
  - Guiar la integración entre sistemas de producción y sistemas de negocio.
- El **estándar ISA-95 tomó al Modelo Purdue como base** y lo formalizó/estandarizó.

### Diferencias clave

| Aspecto                  | Modelo Purdue (PERA)                              | Estándar ISA-95 (IEC 62264)                              |
|--------------------------|----------------------------------------------------|------------------------------------------------------------------|
| **Origen**               | Desarrollado en los 90 en la Universidad Purdue (proyecto PERA) | Estándar oficial de ISA (luego adoptado como IEC 62264)         |
| **Enfoque principal**    | Arquitectura de referencia para **Computer Integrated Manufacturing (CIM)** y segmentación física/funcional de redes | **Interfaz y modelos de información** entre sistemas empresariales (Nivel 4) y sistemas de control de manufactura (Nivel 3) |
| **Propósito central**    | Estructura jerárquica de sistemas y **seguridad por segmentación** (muy usado en ciberseguridad OT – ISA-99 / IEC 62443) | Definir **qué información** fluye entre niveles (especialmente Nivel 3 ↔ Nivel 4), modelos de datos, actividades y transacciones |
| **Nivel de detalle**     | Más conceptual y orientado a arquitectura de red y zonas | Mucho más detallado: modelos de objetos, atributos, verbos (production request, segment requirement, etc.) |
| **Aplicación típica**    | Diseño de redes OT, firewalls entre niveles, DMZ, Purdue segmentation | Implementación de interfaces MES-ERP, integración vertical, estandarización de datos de producción |
| **Uso en ciberseguridad**| Base principal del modelo de segmentación (Purdue levels + zonas/conduit) | Indirecto (se usa junto con Purdue para justificar flujos permitidos) |
| **Flexibilidad tecnológica** | No prescribe protocolos específicos | Independiente de tecnología, pero define flujos y semántica de datos |

### Resumen práctico (cómo se usan en la vida real)

- Cuando hablas de **"segmentar la red según Purdue"**, **firewalls entre niveles**, **DMZ en nivel 3.5**, **no permitir tráfico directo de IT a PLC** → estás hablando del **Modelo Purdue** (aplicado a seguridad y arquitectura de red).
- Cuando hablas de **"implementar ISA-95 para conectar MES con ERP"**, **modelos de producción**, **órdenes de trabajo**, **datos de desempeño**, **categorías de información estandarizadas** → estás hablando del **estándar ISA-95**.

En la mayoría de diagramas y conversaciones cotidianas en la industria se dice simplemente **"pirámide ISA-95"** o **"Modelo Purdue/ISA-95"**, pero técnicamente:

- **Purdue** → más arquitectura y seguridad (cómo se conectan físicamente/lógicamente)
- **ISA-95** → más integración funcional y semántica (qué datos se intercambian y cómo se estructuran)
