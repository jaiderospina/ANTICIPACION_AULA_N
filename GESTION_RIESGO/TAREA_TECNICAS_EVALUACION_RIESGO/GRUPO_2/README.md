# 🛡️ 30 Técnicas de Evaluación de Riesgo — ISO 31000:2018

<div align="center">

![Banner](images/banner.svg)

</div>

<div align="center">

![ISO 31000](https://img.shields.io/badge/ISO%2031000-2018-1F4E79?style=for-the-badge&logo=buffer&logoColor=white)
![ISO 27001](https://img.shields.io/badge/ISO%2FIEC%2027001-2022-2E75B6?style=for-the-badge&logo=shield&logoColor=white)
![ISO 27032](https://img.shields.io/badge/ISO%2FIEC%2027032-2023-0F6E56?style=for-the-badge&logo=security&logoColor=white)
![CEM 2026](https://img.shields.io/badge/CEM-2026-BA7517?style=for-the-badge&logo=graduation-cap&logoColor=white)

**Curso de Estado Mayor **  
MY. SALEK VARGAS SAMIR ALFONSO
MY. URIBE RUEDA ANDRES RODRIGO
MYCIM. GALLO PIMIENTO REINEL
MY. MARTINEZ RINCON DAVID FERNANDO
MY. BAEZ LIZARAZO JAVIER HERNANDO

*Módulo: Ciberseguridad y Gestión de Riesgos*

[Ver técnicas preventivas](#-técnicas-de-identificación-preventivas) · [Ver técnicas analíticas](#-técnicas-analíticas-cuantitativas) · [Ver técnicas de apoyo](#-técnicas-de-apoyo-a-la-decisión)

</div>

---

## 📋 Tabla de Contenidos

- [Contexto y Fuente](#-contexto-y-fuente)
- [Mapa Visual de Técnicas](#-mapa-visual-de-técnicas)
- [Grupo 1 — Identificación y Diagnóstico](#grupo-1--identificación-y-diagnóstico)
- [Grupo 2 — Análisis Causal y de Fallas](#grupo-2--análisis-causal-y-de-fallas)
- [Grupo 3 — Análisis Cuantitativo y Probabilístico](#grupo-3--análisis-cuantitativo-y-probabilístico)
- [Grupo 4 — Apoyo a la Decisión](#grupo-4--apoyo-a-la-decisión)
- [Referencia Rápida — Las 30 Técnicas](#-referencia-rápida--las-30-técnicas)

---

## 🎯 Contexto y Fuente

Este repositorio documenta las **30 Técnicas de Evaluación de Riesgo** identificadas en las páginas 29 y 30 del material de estudio del **Curso de Estado Mayor (CEM) 2026**, bajo el marco normativo de la **ISO 31000:2018** y aplicadas al contexto de **ciberseguridad e infraestructura crítica de defensa**.

> **Nota:** Cada técnica incluye definición técnica formal y ejemplo práctico orientado a operaciones de la Fuerza Aérea Colombiana (FAC) y seguridad de infraestructura crítica nacional.

---

## 🗺️ Mapa Visual de Técnicas

![Mapa de Técnicas](images/mapa_tecnicas.svg)

```
                    ISO 31000:2018 — TÉCNICAS DE EVALUACIÓN DE RIESGO
                    ══════════════════════════════════════════════════

  ┌─────────────────────┐   ┌──────────────────────┐   ┌─────────────────────┐
  │  🔍 IDENTIFICACIÓN  │   │  🔬 ANÁLISIS CAUSAL   │   │  📊 CUANTITATIVO    │
  │  Y DIAGNÓSTICO      │   │  Y DE FALLAS          │   │  Y PROBABILÍSTICO   │
  ├─────────────────────┤   ├──────────────────────┤   ├─────────────────────┤
  │ 01. Lluvia de ideas │   │ 11. Causa/Consecuencia│   │ 17. Monte Carlo     │
  │ 02. Checklist       │   │ 12. Ishikawa          │   │ 18. Redes Bayesian. │
  │ 03. HACCP           │   │ 14. HRA               │   │ 21. Markov          │
  │ 04. Escenarios      │   │ 15. RCM               │   │ 22. Matriz Riesgo   │
  │ 05. AMEF            │   │ 16. Circ. Furtivo     │   │ 29. Índices Riesgo  │
  │ 06. Entrevista      │   │ 27. Causa Raíz (RCA)  │   └─────────────────────┘
  │ 07. PHA             │   └──────────────────────┘
  │ 08. Riesgo Ambient. │   ┌──────────────────────┐   ┌─────────────────────┐
  │ 09. BIA             │   │  🧩 ANÁLISIS DE       │   │  ⚖️ APOYO A LA      │
  │ 25. HAZOP           │   │  SISTEMAS COMPLEJOS   │   │  DECISIÓN           │
  │ 26. SWIFT           │   ├──────────────────────┤   ├─────────────────────┤
  └─────────────────────┘   │ 10. Árbol de Fallas   │   │ 13. Árbol Decisión  │
                            │ 19. LOPA              │   │ 23. Costo/Beneficio │
                            │ 20. Bow Tie           │   │ 24. MCDM            │
                            │ 28. Árbol de Eventos  │   │ 30. Delphi          │
                            └──────────────────────┘   └─────────────────────┘
```

---

## Grupo 1 — Identificación y Diagnóstico

### 01. 💡 Lluvia de Ideas *(Brainstorming)*

![Tipo](https://img.shields.io/badge/Tipo-Cualitativo-1D9E75?style=flat-square) ![Fase](https://img.shields.io/badge/Fase-Identificación-7F77DD?style=flat-square) ![Norma](https://img.shields.io/badge/IEC%2031010-A.3-1F4E79?style=flat-square)

**Definición técnica:**  
Técnica creativa de identificación de riesgos en la que un grupo de expertos genera de manera libre e iterativa ideas sobre posibles amenazas, vulnerabilidades y eventos no deseados. Se fundamenta en la estimulación del pensamiento colectivo sin restricciones críticas en la fase inicial.

**🎖️ Ejemplo — Infraestructura Crítica FAC:**  
Un equipo interdisciplinario (operaciones, TI, inteligencia, logística) realiza sesiones para identificar posibles vectores de ataque cibernético a los sistemas de control de tráfico aéreo (ATC) o redes de comunicaciones tácticas, antes de actualizar el plan de seguridad operacional.

---

### 02. ✅ Lista de Verificación *(Checklist)*

![Tipo](https://img.shields.io/badge/Tipo-Cualitativo-1D9E75?style=flat-square) ![Fase](https://img.shields.io/badge/Fase-Identificación-7F77DD?style=flat-square)

**Definición técnica:**  
Instrumento de evaluación sistemática que consiste en una relación predefinida de ítems, condiciones o controles que deben verificarse frente a un sistema, proceso o activo. Su fortaleza radica en la sistematización de la experiencia acumulada y la reducción del error humano por omisión.

**🎖️ Ejemplo — Infraestructura Crítica FAC:**  
Antes de una misión aérea o activación de un centro de mando, se aplica una lista de verificación de ciberseguridad: actualización de firmas antivirus, verificación de integridad de sistemas SCADA, validación de accesos autorizados y confirmación de protocolos de cifrado en comunicaciones.

---

### 03. 🏭 Análisis de Peligros y Puntos Críticos de Control *(HACCP)*

![Tipo](https://img.shields.io/badge/Tipo-Cualitativo-1D9E75?style=flat-square) ![Fase](https://img.shields.io/badge/Fase-Identificación-7F77DD?style=flat-square)

**Definición técnica:**  
Metodología proactiva que identifica peligros significativos en cada etapa de un proceso y establece Puntos de Control Crítico (PCC) con límites, monitoreo y acciones correctivas predefinidas. Aplicable a cadenas de suministro tecnológico.

**🎖️ Ejemplo — Infraestructura Crítica FAC:**  
Aplicado a la cadena de suministro de software y hardware militar: puntos críticos identificados incluyen la adquisición de componentes electrónicos (riesgo de hardware troyanizado), integración de sistemas (riesgo de backdoors) y actualización de firmware (riesgo de inyección de malware).

---

### 04. 🌐 Análisis de Escenarios

![Tipo](https://img.shields.io/badge/Tipo-Cualitativo-1D9E75?style=flat-square) ![Fase](https://img.shields.io/badge/Fase-Identificación-7F77DD?style=flat-square)

**Definición técnica:**  
Método de evaluación prospectiva que construye descripciones detalladas y plausibles de posibles estados futuros adversos, considerando combinaciones de amenazas, vulnerabilidades y contextos. Especialmente útil para eventos de baja probabilidad y alto impacto.

**🎖️ Ejemplo — Infraestructura Crítica FAC:**  
La FAC desarrolla tres escenarios: **A)** Denegación de servicio a comunicaciones durante operación activa; **B)** Compromiso de sistemas de navegación por actor estatal; **C)** Infiltración de red interna por amenaza interna (*insider threat*). Cada escenario se evalúa en impacto operacional y capacidad de respuesta.

---

### 05. ⚙️ Análisis de Modo y Efecto de Falla *(AMEF / FMEA)*

![Tipo](https://img.shields.io/badge/Tipo-Cuantitativo-378ADD?style=flat-square) ![Fase](https://img.shields.io/badge/Fase-Análisis-D85A30?style=flat-square) ![Índice](https://img.shields.io/badge/NPR-S×O×D-BA7517?style=flat-square)

**Definición técnica:**  
Técnica sistemática y cuantitativa que examina cada componente o función de un sistema para identificar los modos en que puede fallar, los efectos de esa falla y su criticidad mediante el **Número de Prioridad de Riesgo:**

```
NPR = Severidad × Ocurrencia × Detectabilidad
```

**🎖️ Ejemplo — Infraestructura Crítica FAC:**  
Aplicado al sistema IAM de la red militar: la falla en la revocación de accesos a personal desvinculado obtiene NPR alto (S=5, O=3, D=4 → NPR=60), priorizando controles como revisiones periódicas automatizadas de permisos.

---

### 06. 🎤 Entrevista Estructurada

![Tipo](https://img.shields.io/badge/Tipo-Cualitativo-1D9E75?style=flat-square) ![Fase](https://img.shields.io/badge/Fase-Identificación-7F77DD?style=flat-square)

**Definición técnica:**  
Metodología de recopilación de información basada en sesiones individuales con expertos o actores clave, utilizando un guion preestablecido de preguntas abiertas y cerradas. Permite obtener conocimiento tácito y perspectivas especializadas no documentadas formalmente.

**🎖️ Ejemplo — Infraestructura Crítica FAC:**  
Se entrevista estructuradamente al oficial de seguridad, administrador de sistemas, oficial de inteligencia y encargado de operaciones. Se obtiene información sobre prácticas informales de seguridad, incidentes no reportados y percepción de amenazas, complementando la información documental.

---

### 07. 🔭 Análisis Primario de Peligros *(PHA)*

![Tipo](https://img.shields.io/badge/Tipo-Cualitativo-1D9E75?style=flat-square) ![Fase](https://img.shields.io/badge/Fase-Diseño-534AB7?style=flat-square)

**Definición técnica:**  
Técnica inductiva de evaluación temprana de riesgos, aplicada en fases de diseño o conceptualización, que identifica peligros de manera estructurada usando palabras guía para evaluar qué puede salir mal **antes** de la implementación completa del sistema.

**🎖️ Ejemplo — Infraestructura Crítica FAC:**  
Durante el diseño de una red de comunicaciones tácticas clasificadas, se identifican peligros: interceptación de señales, jamming electromagnético, acceso no autorizado a nodos y falla en protocolos de cifrado. Los peligros se incorporan al diseño de seguridad desde el inicio.

---

### 08. 🌍 Valoración del Riesgo Ambiental

![Tipo](https://img.shields.io/badge/Tipo-Cualitativo-1D9E75?style=flat-square) ![Fase](https://img.shields.io/badge/Fase-Contexto-888780?style=flat-square)

**Definición técnica:**  
Evaluación de los riesgos derivados del entorno físico, geográfico, geopolítico y contextual en el que opera una organización. Considera factores externos como desastres naturales, inestabilidad política, conflictos armados y factores sociales que pueden materializar amenazas.

**🎖️ Ejemplo — Infraestructura Crítica FAC:**  
Para una base aérea estratégica se evalúan: proximidad a zonas de conflicto (mayor exposición a ataques), condiciones climáticas que afectan centros de datos (inundaciones) e inestabilidad en la cadena de suministro de componentes tecnológicos críticos por tensiones geopolíticas regionales.

---

### 09. 💼 Análisis de Impacto al Negocio *(BIA)*

![Tipo](https://img.shields.io/badge/Tipo-Cuantitativo-378ADD?style=flat-square) ![Fase](https://img.shields.io/badge/Fase-Continuidad-1D9E75?style=flat-square) ![Métricas](https://img.shields.io/badge/RTO%20|%20RPO%20|%20MTPD-key-BA7517?style=flat-square)

**Definición técnica:**  
Proceso formal de identificación y cuantificación del impacto que tendría la interrupción de procesos o sistemas críticos. Establece:
- **MTPD** — Tiempo Máximo de Interrupción Tolerable
- **RTO** — Objetivo de Tiempo de Recuperación
- **RPO** — Objetivo de Punto de Recuperación

**🎖️ Ejemplo — Infraestructura Crítica FAC:**  
El BIA de sistemas de mando y control determina: MTPD = 4 horas antes de comprometer misiones activas; RTO = 2 horas; RPO = 15 minutos. Esto justifica sistemas redundantes y copias de seguridad en tiempo casi real en ubicaciones geográficamente separadas.

---

### 25. ⚠️ Estudio de Peligros y Operatividad *(HAZOP)*

![Tipo](https://img.shields.io/badge/Tipo-Cualitativo-1D9E75?style=flat-square) ![Fase](https://img.shields.io/badge/Fase-Análisis-D85A30?style=flat-square) ![Palabras Guía](https://img.shields.io/badge/No%20|%20Más%20|%20Menos%20|%20Reverso-guías-534AB7?style=flat-square)

**Definición técnica:**  
Técnica sistemática y cualitativa que examina un sistema usando **palabras guía** (No, Más, Menos, Reverso, Otro que, Antes, Después) aplicadas a parámetros del proceso para identificar desviaciones y sus posibles causas y consecuencias.

**🎖️ Ejemplo — Infraestructura Crítica FAC:**  
Revisión de flujos de datos de sistemas de inteligencia: Parámetro *"flujo de información clasificada"*, Palabra guía *"MÁS"* → Desviación: más datos de los autorizados fluyendo hacia zona desmilitarizada → Causa identificada: exfiltración de datos. Se documentan salvaguardas requeridas.

---

### 26. 🔄 Estructura que Pasa Si *(SWIFT)*

![Tipo](https://img.shields.io/badge/Tipo-Cualitativo-1D9E75?style=flat-square) ![Fase](https://img.shields.io/badge/Fase-Identificación-7F77DD?style=flat-square)

**Definición técnica:**  
Técnica de identificación de riesgos facilitada en grupo que utiliza preguntas estructuradas **"¿Qué pasaría si...?"** para explorar sistemáticamente posibles desviaciones, fallas o situaciones no planificadas. Más estructurada que brainstorming, más ágil que HAZOP.

**🎖️ Ejemplo — Infraestructura Crítica FAC:**  
> *"¿Qué pasaría si el enlace satelital de respaldo falla simultáneamente con la red primaria?"*  
> *"¿Qué pasaría si el administrador de red único está incapacitado durante un incidente cibernético?"*  
> *"¿Qué pasaría si el proveedor cloud clasifica erróneamente datos secretos?"*

---

## Grupo 2 — Análisis Causal y de Fallas

### 10. 🌳 Análisis de Árbol de Fallas *(FTA)*

![Tipo](https://img.shields.io/badge/Tipo-Cuantitativo-378ADD?style=flat-square) ![Dirección](https://img.shields.io/badge/Deductivo-Top--Down-D85A30?style=flat-square)

**Definición técnica:**  
Técnica deductiva *top-down* que parte de un **evento tope** (no deseado) y descompone lógicamente las causas que podrían generarlo usando compuertas lógicas AND/OR. Permite calcular la probabilidad del evento tope mediante álgebra booleana.

![Árbol de Fallas FAC](images/fta_diagram.svg)

```
        [Evento Tope: Compromiso Sistema Defensa]
                          ↑
                      [AND Gate]
               ┌──────────┴──────────┐
         [Falla Radar]          [Falla Comunicac.]
              ↑                       ↑
          [OR Gate]               [OR Gate]
        ┌────┴────┐           ┌────────┴────────┐
   [Ataque  [Falla     [Jamming    [Ciberataque
   Cyber]   HW]        EM]         C2]
```

**🎖️ Ejemplo — Infraestructura Crítica FAC:**  
Árbol de fallas para el compromiso del sistema de defensa aérea: se identifican los **cortes mínimos** más críticos que requieren tratamiento prioritario, como la combinación ataque cibernético al software de procesamiento + falla de comunicaciones de respaldo.

---

### 11. 🔀 Análisis de Causa y Consecuencia

![Tipo](https://img.shields.io/badge/Tipo-Semicuantitativo-BA7517?style=flat-square) ![Dirección](https://img.shields.io/badge/Híbrido-FTA%20+%20ETA-534AB7?style=flat-square)

**Definición técnica:**  
Técnica híbrida que combina árbol de fallas (deductivo) y árbol de eventos (inductivo). Parte de un evento iniciador y se desarrolla simultáneamente hacia atrás (causas) y hacia adelante (consecuencias), proporcionando visión completa de cadenas causales.

**🎖️ Ejemplo — Infraestructura Crítica FAC:**  
Para un incidente de ransomware en sistemas de planificación: **← Causas** (phishing, falta de segmentación, parches desactualizados) | **→ Consecuencias** (cifrado de datos operacionales, interrupción de misiones, exposición de información clasificada, pérdida de credibilidad institucional).

---

### 12. 🐟 Análisis de Causa/Efecto *(Diagrama de Ishikawa)*

![Tipo](https://img.shields.io/badge/Tipo-Cualitativo-1D9E75?style=flat-square) ![Fase](https://img.shields.io/badge/Fase-Diagnóstico-D85A30?style=flat-square)

**Definición técnica:**  
Técnica de análisis causal que representa gráficamente (espina de pescado) las categorías de causas raíz que contribuyen a un efecto. Las categorías incluyen: **Personas, Procesos, Tecnología, Entorno, Gestión y Materiales.**

**🎖️ Ejemplo — Infraestructura Crítica FAC:**

```
Personas ──────────────────────────────────────┐
  (falta concienciación, error humano)          │
Procesos ──────────────────────────────────────┤
  (controles acceso insuficientes, sin DLP)     ├──► FUGA DE INFORMACIÓN CLASIFICADA
Tecnología ─────────────────────────────────────┤
  (sistemas desactualizados, sin cifrado)        │
Gestión ─────────────────────────────────────── ┘
  (ausencia de política de seguridad)
```

---

### 14. 👤 Análisis de Confiabilidad Humana *(HRA)*

![Tipo](https://img.shields.io/badge/Tipo-Cuantitativo-378ADD?style=flat-square) ![Factor](https://img.shields.io/badge/Factor-Humano-D85A30?style=flat-square)

**Definición técnica:**  
Metodología que evalúa la probabilidad de **error humano** en tareas críticas, identificando Factores de Desempeño que pueden aumentar o reducir dicha probabilidad (fatiga, capacitación, procedimientos ambiguos, presión temporal, carga cognitiva).

**🎖️ Ejemplo — Infraestructura Crítica FAC:**  
Análisis de operadores de IDS: durante turnos nocturnos superiores a 8 horas, la probabilidad de error en clasificación de alertas aumenta un **40%**. Controles implementados: rotación de turnos, umbrales de alerta optimizados y procedimientos estandarizados de respuesta.

---

### 15. 🔧 Mantenimiento Enfocado en la Confiabilidad *(RCM)*

![Tipo](https://img.shields.io/badge/Tipo-Cuantitativo-378ADD?style=flat-square) ![Fase](https://img.shields.io/badge/Fase-Operación-1D9E75?style=flat-square)

**Definición técnica:**  
Estrategia estructurada de gestión de mantenimiento que identifica las acciones más efectivas para garantizar que los activos continúen realizando sus funciones en su contexto operacional, priorizando según consecuencias de falla y relación costo-beneficio.

**🎖️ Ejemplo — Infraestructura Crítica FAC:**  
Aplicado a servidores de mando y control y equipos de comunicaciones: se identifican funciones críticas, modos de falla (software, hardware, ciberseguridad), consecuencias y tareas de mantenimiento preventivo/predictivo óptimas para mantener la disponibilidad operacional requerida.

---

### 16. 🕵️ Análisis de Circuito Furtivo *(Sneak Circuit Analysis)*

![Tipo](https://img.shields.io/badge/Tipo-Cualitativo-1D9E75?style=flat-square) ![Riesgo](https://img.shields.io/badge/Backdoors-Supply%20Chain-A32D2D?style=flat-square)

**Definición técnica:**  
Técnica de revisión de diseño que identifica caminos o condiciones **ocultas** en circuitos o software que pueden causar operaciones no deseadas o prevenir operaciones deseadas, sin existir una falla convencional.

**🎖️ Ejemplo — Infraestructura Crítica FAC:**  
En análisis de sistemas embebidos de aeronaves militares: se identifican rutas de código no documentadas en firmware que podrían activarse bajo condiciones específicas y alterar sistemas de navegación. Permite detectar backdoors introducidas en el proceso de desarrollo por actores de la cadena de suministro.

---

### 27. 🔍 Análisis de Causa Raíz *(RCA)*

![Tipo](https://img.shields.io/badge/Tipo-Cualitativo-1D9E75?style=flat-square) ![Fase](https://img.shields.io/badge/Fase-Post--Incidente-A32D2D?style=flat-square)

**Definición técnica:**  
Metodología retrospectiva de investigación de incidentes que va más allá de los síntomas superficiales para identificar las causas fundamentales que permitieron que ocurriera un evento. Su objetivo es implementar correcciones que eviten la recurrencia.

**🎖️ Ejemplo — Infraestructura Crítica FAC:**  
Tras acceso no autorizado a la red de la base, el RCA identifica:
- **Causa raíz técnica:** credenciales de administrador compartidas sin rotación
- **Causa raíz organizacional:** ausencia de política de identidades privilegiadas
- **Causa raíz cultural:** cultura de compartir contraseñas por conveniencia operacional

---

## Grupo 3 — Análisis Cuantitativo y Probabilístico

### 17. 🎲 Simulación Monte Carlo

![Tipo](https://img.shields.io/badge/Tipo-Cuantitativo-378ADD?style=flat-square) ![Iteraciones](https://img.shields.io/badge/N-100.000%2B%20iteraciones-185FA5?style=flat-square)

**Definición técnica:**  
Técnica computacional de análisis cuantitativo que utiliza generación aleatoria de escenarios (muestreo de distribuciones de probabilidad) para modelar sistemas complejos y estimar la distribución de resultados posibles.

**🎖️ Ejemplo — Infraestructura Crítica FAC:**  
Modelamiento del riesgo de disponibilidad del sistema ATC: variables de entrada (frecuencia de ataques, tiempo de detección, tiempo de recuperación) como distribuciones de probabilidad. Resultado de 100,000 simulaciones: **5% de probabilidad** de interrupción superior a 6 horas en un año.

---

### 18. 🕸️ Redes Bayesianas

![Tipo](https://img.shields.io/badge/Tipo-Cuantitativo-378ADD?style=flat-square) ![Método](https://img.shields.io/badge/Teorema-de%20Bayes-534AB7?style=flat-square)

**Definición técnica:**  
Modelos gráficos probabilísticos que representan variables aleatorias y sus dependencias condicionales mediante un grafo acíclico dirigido (DAG). Permiten inferir probabilidades de eventos dados ciertos indicadores observados, actualizando creencias según nueva evidencia.

**🎖️ Ejemplo — Infraestructura Crítica FAC:**  
Red bayesiana para evaluar probabilidad de ciberataque estatal: nodos incluyen *(tensión geopolítica alta + patrones anómalos de tráfico + intentos de intrusión incrementados + vulnerabilidades no parchadas)*. La red actualiza dinámicamente la probabilidad de ataque al observar cada nuevo IOC (*Indicator of Compromise*).

---

### 19. 🛡️ Análisis de Capas de Protección *(LOPA)*

![Tipo](https://img.shields.io/badge/Tipo-Semicuantitativo-BA7517?style=flat-square) ![Concepto](https://img.shields.io/badge/IPL-Capas%20Independientes-1D9E75?style=flat-square)

**Definición técnica:**  
Técnica semi-cuantitativa que evalúa si existen capas de protección independientes (IPL) suficientes para reducir la frecuencia de un escenario a un nivel tolerable. Cada capa reduce la frecuencia del evento en un Factor de Reducción de Riesgo (PFD).

**🎖️ Ejemplo — Infraestructura Crítica FAC:**

| Capa | Control | PFD |
|------|---------|-----|
| 1 | Segmentación física de red | 0.01 |
| 2 | Autenticación multifactor | 0.1 |
| 3 | IDS con respuesta automática | 0.1 |
| **Resultado** | **Frecuencia reducida** | **0.0001 eventos/año** |

---

### 20. 🎀 Análisis de Esquema de Corbatín *(Bow Tie)*

![Tipo](https://img.shields.io/badge/Tipo-Cualitativo-1D9E75?style=flat-square) ![Integra](https://img.shields.io/badge/FTA%20+%20ETA-combinado-534AB7?style=flat-square)

**Definición técnica:**  
Representación gráfica que combina árbol de amenazas (izquierda) con árbol de consecuencias (derecha), conectados por el evento crítico central. Visualiza simultáneamente causas, barreras preventivas, evento central, barreras de mitigación y consecuencias.

![Bow Tie FAC](images/bowtie_diagram.svg)

**🎖️ Ejemplo — Infraestructura Crítica FAC:**

```
AMENAZAS          BARRERAS    EVENTO CENTRAL    BARRERAS    CONSECUENCIAS
─────────         ─────────   ──────────────    ─────────   ─────────────
Phishing ─────────┐ Capacit.│                  │ Cifrado │─ Fuga Info
Insider ──────────┤ Control ├─ ACCESO NO    ───┤ DLP     ├─ Daño Reput.
Vulner. Técn. ─── ┘ Acceso │  AUTORIZADO       │ Plan IR │─ Sanciones
                  ─────────                    ─────────
```

---

### 21. 📈 Análisis de Markov

![Tipo](https://img.shields.io/badge/Tipo-Cuantitativo-378ADD?style=flat-square) ![Concepto](https://img.shields.io/badge/Estados-Discretos-185FA5?style=flat-square)

**Definición técnica:**  
Técnica matemática que modela sistemas con diferentes estados discretos y transiciones probabilísticas entre estados. Permite calcular la disponibilidad, confiabilidad y mantenibilidad de sistemas complejos con redundancia.

**🎖️ Ejemplo — Infraestructura Crítica FAC:**  
Sistema de comunicaciones militares con tres estados: **Normal → Degradado → Falla Total**. Las tasas de transición se determinan a partir de datos históricos de incidentes, calculando la disponibilidad esperada y optimizando estrategias de mantenimiento y redundancia.

---

### 22. 📊 Matriz de Consecuencia y Probabilidad *(Matriz de Riesgo)*

![Tipo](https://img.shields.io/badge/Tipo-Semicuantitativo-BA7517?style=flat-square) ![Escala](https://img.shields.io/badge/Escala-5×5-1F4E79?style=flat-square)

**Definición técnica:**  
Herramienta semi-cuantitativa que combina en una tabla bidimensional la probabilidad de ocurrencia y la magnitud de consecuencias, generando una clasificación del nivel de riesgo para priorización.

**🎖️ Ejemplo — Infraestructura Crítica FAC:**

|  | **Impacto 1** | **Impacto 2** | **Impacto 3** | **Impacto 4** | **Impacto 5** |
|---|---|---|---|---|---|
| **Prob 5** | 🟡 Medio | 🟠 Alto | 🔴 Crítico | 🔴 Crítico | 🔴 Crítico |
| **Prob 4** | 🟢 Bajo | 🟡 Medio | 🟠 Alto | 🔴 Crítico | 🔴 **Ransomware** |
| **Prob 3** | 🟢 Bajo | 🟡 Medio | 🟡 Medio | 🟠 Alto | 🔴 Crítico |
| **Prob 2** | 🟢 Bajo | 🟢 Bajo | 🟡 Medio | 🟡 Medio | 🟠 Alto |
| **Prob 1** | 🟢 Bajo | 🟢 Bajo | 🟢 Bajo | 🟡 Medio | 🟡 Medio |

> 🔴 **Riesgo Intolerable** — Requiere tratamiento inmediato  
> 🟠 **Riesgo Alto** — Requiere acción a corto plazo  
> 🟡 **Riesgo Medio** — Monitoreo y controles  
> 🟢 **Riesgo Bajo** — Aceptable con controles básicos

---

### 28. 🌿 Análisis de Árbol de Eventos *(ETA)*

![Tipo](https://img.shields.io/badge/Tipo-Cuantitativo-378ADD?style=flat-square) ![Dirección](https://img.shields.io/badge/Inductivo-Bottom--Up-1D9E75?style=flat-square)

**Definición técnica:**  
Técnica inductiva que, partiendo de un evento iniciador, desarrolla las posibles secuencias de eventos subsiguientes considerando el éxito o fracaso de los sistemas de mitigación y respuesta, calculando las probabilidades de cada resultado final.

**🎖️ Ejemplo — Infraestructura Crítica FAC:**  
Evento iniciador *"Detección de malware en sistema de navegación"*: árbol desarrolla ramas según respuesta del antivirus (éxito/fallo), detección por el piloto (éxito/fallo), activación del sistema de respaldo (éxito/fallo) e intervención del controlador en tierra. Cada camino tiene probabilidad y consecuencia calculada.

---

### 29. 📉 Índices de Riesgo

![Tipo](https://img.shields.io/badge/Tipo-Cuantitativo-378ADD?style=flat-square) ![Uso](https://img.shields.io/badge/Uso-Priorización-BA7517?style=flat-square)

**Definición técnica:**  
Técnica de evaluación relativa que utiliza puntuaciones o índices compuestos para comparar y clasificar riesgos o activos. Los índices integran múltiples factores en una puntuación única que facilita la priorización.

**🎖️ Ejemplo — Infraestructura Crítica FAC:**

```
IRC = (Valor del Activo × Nivel de Amenaza × Nivel de Vulnerabilidad)
      ─────────────────────────────────────────────────────────────────
                        Efectividad de Controles

Sistema ATC:        IRC = (10 × 9 × 8) / 9 = 80/100 → PRIORIDAD CRÍTICA
Red Administrativa: IRC = (6 × 5 × 6) / 7 = 26/100 → PRIORIDAD BAJA
```

---

## Grupo 4 — Apoyo a la Decisión

### 13. 🌲 Árbol de Decisión

![Tipo](https://img.shields.io/badge/Tipo-Cuantitativo-378ADD?style=flat-square) ![Método](https://img.shields.io/badge/Valor-Esperado-185FA5?style=flat-square)

**Definición técnica:**  
Herramienta de análisis y selección de opciones que representa gráficamente las decisiones posibles y sus consecuencias probabilísticas, permitiendo calcular el **valor esperado** de cada alternativa para optimizar la toma de decisiones bajo incertidumbre.

**🎖️ Ejemplo — Infraestructura Crítica FAC:**  
Ante la detección de intrusión en la red: el árbol modela *Decisión 1 (aislar sistemas vs. monitorear)*, con probabilidades de éxito/fracaso e impactos operacionales. Permite al Oficial de Seguridad elegir la respuesta óptima balanceando interrupción operacional vs. riesgo de propagación del ataque.

---

### 23. 💰 Análisis de Costo/Beneficio

![Tipo](https://img.shields.io/badge/Tipo-Cuantitativo-378ADD?style=flat-square) ![Métrica](https://img.shields.io/badge/ROI-Retorno%20Seguridad-1D9E75?style=flat-square)

**Definición técnica:**  
Técnica económica que compara el costo total de implementar controles contra el beneficio esperado en términos de reducción del riesgo. La decisión óptima maximiza el beneficio neto (pérdidas evitadas - costo de controles).

**🎖️ Ejemplo — Infraestructura Crítica FAC:**

```
Sistema XDR (Detección y Respuesta Extendida):

Inversión:  $500,000 implementación + $100,000/año mantenimiento
Beneficio:  80% reducción probabilidad incidente mayor
            $2,000,000/año en pérdidas evitadas (interrupción + sanciones)

Relación B/C = $2,000,000 / $600,000 = 3.2 : 1  ✅ INVERSIÓN JUSTIFICADA
```

---

### 24. ⚖️ Análisis de Decisión por Criterios Múltiples *(MCDM)*

![Tipo](https://img.shields.io/badge/Tipo-Cuantitativo-378ADD?style=flat-square) ![Métodos](https://img.shields.io/badge/AHP%20|%20TOPSIS%20|%20VIKOR-métodos-534AB7?style=flat-square)

**Definición técnica:**  
Marco metodológico que evalúa y compara alternativas de tratamiento considerando simultáneamente múltiples criterios con diferentes pesos de importancia. Incluye métodos como AHP (Proceso Analítico Jerárquico), TOPSIS y VIKOR.

**🎖️ Ejemplo — Infraestructura Crítica FAC:**

| Criterio | Peso | Aislamiento Total | Contención Parcial | Monitoreo Activo |
|---|---|---|---|---|
| Efectividad técnica | 35% | 9.0 | 7.0 | 5.0 |
| Tiempo implementación | 25% | 3.0 | 7.0 | 9.0 |
| Costo | 20% | 5.0 | 7.0 | 8.0 |
| Impacto operaciones | 20% | 2.0 | 6.0 | 9.0 |
| **Puntaje ponderado** | | **5.55** | **6.85** | **7.35** |
| **Decisión** | | | | **✅ SELECCIONADO** |

---

### 30. 🎯 Método Delphi

![Tipo](https://img.shields.io/badge/Tipo-Cualitativo-1D9E75?style=flat-square) ![Proceso](https://img.shields.io/badge/Rondas-Iterativas%20Anónimas-534AB7?style=flat-square)

**Definición técnica:**  
Técnica estructurada de consulta iterativa a un panel de expertos que busca alcanzar consenso sobre un tema complejo o incierto. Mediante rondas sucesivas de cuestionarios anónimos con retroalimentación controlada, se reduce gradualmente la dispersión de opiniones hasta alcanzar convergencia.

**🎖️ Ejemplo — Infraestructura Crítica FAC:**  
La Dirección de Ciberseguridad aplica Delphi para estimar la probabilidad de ciberataques de alta sofisticación contra infraestructura crítica en los próximos 5 años. Panel de 15 expertos en inteligencia, ciberseguridad y defensa completan 3 rondas de cuestionarios anónimos. El resultado consensuado informa el plan estratégico de ciberseguridad y la priorización de inversiones.

---

## 📑 Referencia Rápida — Las 30 Técnicas

| N° | Técnica | Tipo | Fase Principal | Norma |
|---|---|---|---|---|
| 01 | Lluvia de ideas | Cualitativo | Identificación | IEC 31010 A.3 |
| 02 | Lista de verificación | Cualitativo | Identificación | IEC 31010 A.4 |
| 03 | HACCP | Cualitativo | Identificación | IEC 31010 A.5 |
| 04 | Análisis de escenarios | Cualitativo | Identificación | IEC 31010 A.9 |
| 05 | AMEF / FMEA | Cuantitativo | Análisis | IEC 31010 A.17 |
| 06 | Entrevista estructurada | Cualitativo | Identificación | IEC 31010 A.6 |
| 07 | Análisis primario de peligros (PHA) | Cualitativo | Diseño | IEC 31010 A.12 |
| 08 | Valoración del riesgo ambiental | Cualitativo | Contexto | ISO 31000 §6.3 |
| 09 | Análisis de impacto al negocio (BIA) | Cuantitativo | Continuidad | ISO 22301 |
| 10 | Árbol de fallas (FTA) | Cuantitativo | Análisis | IEC 31010 A.19 |
| 11 | Análisis de causa y consecuencia | Semicuantitativo | Análisis | IEC 31010 A.21 |
| 12 | Causa/efecto — Ishikawa | Cualitativo | Diagnóstico | IEC 31010 A.22 |
| 13 | Árbol de decisión | Cuantitativo | Decisión | IEC 31010 A.24 |
| 14 | Confiabilidad humana (HRA) | Cuantitativo | Análisis | IEC 31010 A.25 |
| 15 | Mantenimiento RCM | Cuantitativo | Operación | IEC 60300-3-11 |
| 16 | Análisis de circuito furtivo | Cualitativo | Diseño | NASA |
| 17 | Simulación Monte Carlo | Cuantitativo | Análisis | IEC 31010 A.26 |
| 18 | Redes bayesianas | Cuantitativo | Análisis | IEC 31010 A.27 |
| 19 | Capas de protección (LOPA) | Semicuantitativo | Análisis | IEC 61511-3 |
| 20 | Esquema corbatín (Bow Tie) | Cualitativo | Análisis | IEC 31010 A.29 |
| 21 | Análisis de Markov | Cuantitativo | Análisis | IEC 31010 A.28 |
| 22 | Matriz consecuencia/probabilidad | Semicuantitativo | Evaluación | IEC 31010 A.30 |
| 23 | Análisis costo/beneficio | Cuantitativo | Decisión | IEC 31010 A.31 |
| 24 | Criterios múltiples (MCDM) | Cuantitativo | Decisión | IEC 31010 A.32 |
| 25 | HAZOP | Cualitativo | Análisis | IEC 31010 A.14 |
| 26 | SWIFT | Cualitativo | Identificación | IEC 31010 A.10 |
| 27 | Causa raíz (RCA) | Cualitativo | Post-incidente | IEC 31010 A.23 |
| 28 | Árbol de eventos (ETA) | Cuantitativo | Análisis | IEC 31010 A.18 |
| 29 | Índices de riesgo | Cuantitativo | Evaluación | IEC 31010 A.11 |
| 30 | Método Delphi | Cualitativo | Identificación | IEC 31010 A.7 |

---

## 📚 Referencias Normativas

```
ISO 31000:2018   — Risk Management — Guidelines
IEC 31010:2019   — Risk Assessment Techniques
ISO/IEC 27001:2022 — Information Security Management Systems
ISO/IEC 27032:2023 — Cybersecurity Guidelines
ISO 22301:2019   — Business Continuity Management
IEC 61511-3      — Safety Instrumented Systems
```

---

<div align="center">

**Curso de Estado Mayor — CEM 2026**  
 
*Módulo: Ciberseguridad y Gestión de Riesgos*

![GitHub](https://img.shields.io/badge/Documento-Académico-1F4E79?style=for-the-badge)
![Uso](https://img.shields.io/badge/Uso-Académico%20Interno-534AB7?style=for-the-badge)

</div>
