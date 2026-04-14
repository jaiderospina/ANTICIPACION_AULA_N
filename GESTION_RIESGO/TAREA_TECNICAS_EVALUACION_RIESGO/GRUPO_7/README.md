# Técnicas de Evaluación de Riesgos

Referencia estructurada de las principales técnicas para identificar, analizar y gestionar riesgos en seguridad de la información e infraestructura tecnológica.

\---

## 1\. Identificación y Consulta

Técnicas orientadas a recopilar información y detectar riesgos mediante la participación de personas.

|Técnica|Descripción|
|-|-|
|**Lluvia de ideas**|Sesión grupal para identificar amenazas y vulnerabilidades de forma creativa|
|**Entrevista estructurada**|Consulta formal a expertos mediante preguntas predefinidas|
|**Delphi**|Consenso anónimo y sistemático entre especialistas externos|
|**Lista de verificación**|Auditoría de controles frente a criterios preestablecidos (ej. ISO/IEC 27001)|
|**SWIFT**|Preguntas hipotéticas del tipo "¿qué pasa si…?" para descubrir escenarios de riesgo|

\---

## 2\. Análisis de Peligros y Procesos

Técnicas centradas en identificar desviaciones y puntos críticos en sistemas y procesos.

|Técnica|Descripción|
|-|-|
|**PHA** (Análisis primario de peligros)|Identificación temprana de riesgos críticos en fases iniciales de un proyecto|
|**HAZOP**|Examen sistemático de desviaciones en procesos que puedan generar riesgos|
|**HACCP**|Identificación de puntos de control críticos donde un fallo puede ser catastrófico|
|**Valoración del riesgo ambiental**|Evaluación de amenazas físicas o naturales sobre la infraestructura|

\---

## 3\. Análisis de Impacto y Fallas

Técnicas para comprender las causas, consecuencias y modos de fallo de los sistemas.

|Técnica|Descripción|
|-|-|
|**BIA** (Análisis de impacto al negocio)|Cuantifica las consecuencias de interrupciones en procesos críticos|
|**RCA** (Análisis de causa raíz)|Identifica el origen fundamental de un incidente para evitar repetición|
|**FMEA** (Análisis de modo y efecto de falla)|Evalúa cómo puede fallar un componente y el impacto de dicho fallo|
|**FTA** (Árbol de fallas)|Método deductivo que parte de un evento no deseado para encontrar sus causas|
|**ETA** (Árbol de eventos)|Método inductivo que parte de un evento y analiza sus posibles consecuencias|
|**Análisis de causa y consecuencia**|Combina FTA y ETA para una visión integral del riesgo|
|**Ishikawa** (Causa/efecto)|Representación visual de todos los factores que contribuyen a un problema|
|**LOPA** (Análisis de capas de protección)|Evalúa la efectividad de barreras de defensa independientes|
|**Bow Tie**|Visualiza causas, evento central y consecuencias con sus barreras preventivas y reactivas|

\---

## 4\. Modelado y Confiabilidad

Técnicas para modelar el comportamiento de sistemas y evaluar la confiabilidad humana y operacional.

|Técnica|Descripción|
|-|-|
|**Árbol de decisión**|Modelo gráfico para evaluar opciones y sus resultados bajo incertidumbre|
|**Análisis de confiabilidad humana**|Estudia el impacto de errores u omisiones humanas en la seguridad del sistema|
|**RCM** (Mantenimiento enfocado en confiabilidad)|Estrategia para asegurar que los activos mantengan su función de seguridad|
|**Análisis de circuito furtivo**|Identifica rutas o funciones ocultas no deseadas en sistemas o aplicaciones|

\---

## 5\. Estadística y Probabilidad

Técnicas cuantitativas que usan modelos matemáticos para estimar probabilidades y simular escenarios.

|Técnica|Descripción|
|-|-|
|**Análisis de Markov**|Modela sistemas que cambian de estado de forma aleatoria con el tiempo|
|**Simulación Monte Carlo**|Usa muestreo aleatorio para estimar costos y probabilidades en situaciones inciertas|
|**Redes bayesianas**|Modelos probabilísticos que representan variables y sus dependencias causales|
|**Índices de riesgo**|Puntajes numéricos para priorizar riesgos (ej. CVSS para vulnerabilidades)|

\---

## 6\. Valoración y Decisión

Técnicas para clasificar, comparar y seleccionar entre alternativas de gestión del riesgo.

|Técnica|Descripción|
|-|-|
|**Matriz consecuencia/probabilidad**|Clasifica riesgos visualmente según impacto y frecuencia esperada|
|**Análisis de costo/beneficio**|Compara el costo de un control de seguridad frente al riesgo que mitiga|
|**MCDA** (Decisión por criterios múltiples)|Evalúa alternativas de seguridad con criterios contrapuestos (costo, cumplimiento, tiempo de respuesta)|

\---

## Mapa de referencia rápida

```
Técnicas de Evaluación de Riesgos
├── Identificación y Consulta
│   ├── Lluvia de ideas
│   ├── Entrevista estructurada
│   ├── Delphi
│   ├── Lista de verificación
│   └── SWIFT
├── Análisis de Peligros y Procesos
│   ├── PHA
│   ├── HAZOP
│   ├── HACCP
│   └── Valoración del riesgo ambiental
├── Análisis de Impacto y Fallas
│   ├── BIA
│   ├── RCA
│   ├── FMEA
│   ├── FTA / ETA
│   ├── Análisis de causa y consecuencia
│   ├── Ishikawa
│   ├── LOPA
│   └── Bow Tie
├── Modelado y Confiabilidad
│   ├── Árbol de decisión
│   ├── Confiabilidad humana
│   ├── RCM
│   └── Análisis de circuito furtivo
├── Estadística y Probabilidad
│   ├── Análisis de Markov
│   ├── Monte Carlo
│   ├── Redes bayesianas
│   └── Índices de riesgo
└── Valoración y Decisión
    ├── Matriz consecuencia/probabilidad
    ├── Análisis de costo/beneficio
    └── MCDA
```

