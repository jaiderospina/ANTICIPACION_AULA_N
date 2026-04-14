# Glosario de Técnicas de Evaluación de Riesgos

Referencia rápida de las principales técnicas utilizadas para identificar, analizar y priorizar riesgos en sistemas de seguridad de la información e infraestructura tecnológica.

\---

## Técnicas de Identificación

### 🧠 Lluvia de ideas (Brainstorming)

Sesión grupal para identificar de forma creativa posibles amenazas y vulnerabilidades.

> \*\*Ejemplo:\*\* Reunir al equipo de respuesta a incidentes para imaginar nuevos vectores de ataque contra una API recientemente desplegada.

\---

### 🎙️ Entrevista estructurada

Consulta formal a expertos mediante preguntas predefinidas para recopilar datos sobre riesgos.

> \*\*Ejemplo:\*\* Entrevistar al administrador de red para detallar los controles de acceso existentes en el centro de datos.

\---

### 🔵 Delphi

Método para alcanzar un consenso entre expertos de forma anónima y sistemática.

> \*\*Ejemplo:\*\* Consultar a diversos especialistas externos para determinar la probabilidad de un ciberataque de tipo "zero-day" en el sector energético a cinco años.

\---

### ✅ Lista de verificación (Checklist)

Verificación de controles y requisitos frente a una lista de criterios preestablecidos.

> \*\*Ejemplo:\*\* Auditar una infraestructura de nube siguiendo los puntos de control del estándar ISO/IEC 27001.

\---

### ⚠️ Análisis primario de peligros (PHA)

Identificación temprana de los riesgos más críticos en las fases iniciales de un proyecto.

> \*\*Ejemplo:\*\* Identificar que la falta de cifrado en una base de datos es el peligro principal antes de lanzar una aplicación móvil.

\---

### 🔍 Estudio de peligros y operatividad (HAZOP)

Examen sistemático para identificar desviaciones en los procesos que puedan generar riesgos.

> \*\*Ejemplo:\*\* Analizar el flujo de datos en un cortafuegos (firewall) para detectar reglas que permitan tráfico no deseado por error de configuración.

\---

### 🔒 Análisis de peligros y puntos críticos de control (HACCP)

Identificación de puntos específicos donde el control es vital para prevenir fallos críticos.

> \*\*Ejemplo:\*\* Establecer el servidor de autenticación multifactor (MFA) como un punto crítico cuya caída detendría todo el acceso remoto seguro.

\---

### 🌱 Valoración del riesgo ambiental

Evaluación de riesgos derivados del entorno físico o natural que afectan la infraestructura.

> \*\*Ejemplo:\*\* Analizar la vulnerabilidad de un centro de datos ante inundaciones o cortes de energía por desastres naturales.

\---

### 💬 Estructura "Qué pasa si" (SWIFT)

Técnica de equipo que utiliza preguntas hipotéticas para identificar riesgos.

> \*\*Ejemplo:\*\* "¿Qué pasa si el proveedor de servicios DNS sufre un ataque de denegación de servicio (DDoS)?"

\---

## Técnicas de Análisis

### 📖 Análisis de escenarios

Exploración detallada de situaciones futuras posibles y sus impactos.

> \*\*Ejemplo:\*\* Simular el impacto operativo y reputacional de un ataque de ransomware que cifre todos los servidores de producción.

\---

### 💼 Análisis de impacto al negocio (BIA)

Determinación de las consecuencias de la interrupción de procesos críticos.

> \*\*Ejemplo:\*\* Calcular la pérdida financiera por hora de inactividad de una plataforma de comercio electrónico.

\---

### 🔎 Análisis de causa raíz (RCA)

Identificación del origen fundamental de un incidente para evitar su repetición.

> \*\*Ejemplo:\*\* Determinar que una brecha de datos ocurrió porque un desarrollador dejó una clave de acceso expuesta en un repositorio público de código.

\---

### ⚙️ Análisis de modo y efecto de falla (FMEA)

Evaluación de las formas en que un componente puede fallar y las consecuencias de dicha falla.

> \*\*Ejemplo:\*\* Evaluar qué ocurre si falla el balanceador de carga de un sitio web crítico.

\---

### 🌳 Análisis de árbol de fallas (FTA)

Método deductivo que parte de un evento no deseado para encontrar sus causas potenciales.

> \*\*Ejemplo:\*\* Mapear todas las combinaciones de fallos técnicos y humanos que podrían permitir un acceso no autorizado a la base de datos de clientes.

\---

### 🌿 Análisis de árbol de eventos (ETA)

Método inductivo que parte de un evento inicial y analiza sus posibles evoluciones.

> \*\*Ejemplo:\*\* Modelar las posibles consecuencias después de que un empleado haga clic en un enlace de phishing.

\---

### 🔗 Análisis de causa y consecuencia

Combinación de los árboles de fallas y eventos para una visión integral del riesgo.

> \*\*Ejemplo:\*\* Analizar el origen de un fallo en el sistema de respaldo y cómo ese fallo escala hasta la pérdida total de datos.

\---

### 🐟 Análisis de causa/efecto (Ishikawa)

Representación visual de los factores que contribuyen a un problema de seguridad.

> \*\*Ejemplo:\*\* Diagramar los factores (personal, tecnología, procesos) que causan lentitud en la aplicación de parches de seguridad.

\---

### 🛡️ Análisis de capas de protección (LOPA)

Evaluación de la efectividad de las barreras de defensa sucesivas.

> \*\*Ejemplo:\*\* Analizar cómo el firewall, el antivirus y la segmentación de red actúan como capas independientes para detener una intrusión.

\---

### 🌲 Árbol de decisión

Modelo gráfico para evaluar opciones y sus resultados probables bajo incertidumbre.

> \*\*Ejemplo:\*\* Decidir entre pagar un rescate en un ataque de ransomware o intentar restaurar desde copias de seguridad de hace 48 horas.

\---

### 👤 Análisis de confiabilidad humana

Estudio del impacto de los errores u omisiones humanas en la seguridad del sistema.

> \*\*Ejemplo:\*\* Evaluar la probabilidad de que un administrador de sistemas configure incorrectamente una política de permisos en la nube.

\---

### 🎀 Análisis de esquema de corbatín (Bow Tie)

Visualización del riesgo que une las causas, el evento central y las consecuencias, mostrando las barreras preventivas y reactivas.

> \*\*Ejemplo:\*\* Visualizar una infección por malware, situando el software antivirus como barrera preventiva y el plan de recuperación ante desastres como barrera reactiva.

\---

### 🔧 Mantenimiento enfocado en la confiabilidad (RCM)

Estrategia para asegurar que los activos continúen realizando su función de seguridad.

> \*\*Ejemplo:\*\* Establecer un programa riguroso de actualizaciones y pruebas de hardware para los servidores del centro de operaciones de seguridad (SOC).

\---

### 🕵️ Análisis de circuito furtivo

Identificación de rutas o funciones no deseadas que pueden activarse en condiciones específicas.

> \*\*Ejemplo:\*\* Detectar "puertas traseras" o funciones de administración ocultas en el código de una aplicación antigua.

\---

## Técnicas Cuantitativas

### 📊 Análisis de Markov

Modelado matemático de sistemas que cambian de estado de forma aleatoria con el tiempo.

> \*\*Ejemplo:\*\* Predecir la disponibilidad de un sistema crítico basándose en el tiempo medio entre fallos y el tiempo medio de reparación.

\---

### 🎲 Simulación Monte Carlo

Uso de muestreo aleatorio para modelar la probabilidad de diferentes resultados en situaciones inciertas.

> \*\*Ejemplo:\*\* Realizar miles de simulaciones para estimar el costo total anual esperado por incidentes de ciberseguridad.

\---

### 🕸️ Redes bayesianas

Modelos probabilísticos que representan variables y sus dependencias causales.

> \*\*Ejemplo:\*\* Estimar la probabilidad de una amenaza persistente avanzada (APT) basándose en una serie de anomalías detectadas en el tráfico de red.

\---

### 🔢 Índices de riesgo

Puntajes numéricos utilizados para priorizar riesgos según métricas específicas.

> \*\*Ejemplo:\*\* Utilizar el sistema de puntuación CVSS para priorizar el parcheo de vulnerabilidades según su gravedad técnica.

\---

## Técnicas de Evaluación y Decisión

### 📉 Matriz de consecuencia y probabilidad

Herramienta visual que clasifica los riesgos según su impacto y su frecuencia esperada.

> \*\*Ejemplo:\*\* Ubicar el riesgo de "fuga de información por empleado descontento" en un cuadrante de alto impacto y baja probabilidad.

\---

### 💰 Análisis de costo/beneficio

Comparación entre el costo de implementar una medida de seguridad y el beneficio (reducción de riesgo) obtenido.

> \*\*Ejemplo:\*\* Evaluar si la inversión en un sistema de detección de intrusos (IDS) de 100,000 USD justifica la prevención de una brecha que costaría 1 millón de USD.

\---

### ⚖️ Análisis de decisión por criterios múltiples (MCDA)

Evaluación de alternativas de seguridad basadas en diversos criterios contrapuestos.

> \*\*Ejemplo:\*\* Seleccionar un proveedor de seguridad gestionada evaluando costo, experiencia técnica, cumplimiento legal y tiempos de respuesta.

\---

## Resumen de técnicas

|Técnica|Tipo|Uso principal|
|-|-|-|
|Brainstorming|Cualitativo|Identificación inicial de amenazas|
|Entrevista estructurada|Cualitativo|Recolección de datos con expertos|
|Delphi|Cualitativo|Consenso anónimo entre especialistas|
|Checklist|Cualitativo|Auditoría contra estándares|
|PHA|Cualitativo|Riesgos críticos en etapas tempranas|
|HAZOP|Cualitativo|Desviaciones en procesos|
|HACCP|Cualitativo|Puntos de control críticos|
|Riesgo ambiental|Cualitativo|Amenazas físicas/naturales|
|SWIFT|Cualitativo|Escenarios hipotéticos|
|Análisis de escenarios|Mixto|Simulación de impactos futuros|
|BIA|Mixto|Impacto en procesos de negocio|
|RCA|Cualitativo|Causa raíz de incidentes|
|FMEA|Mixto|Modos de falla de componentes|
|FTA|Cuantitativo|Causas de un evento no deseado|
|ETA|Cuantitativo|Consecuencias de un evento inicial|
|Causa y consecuencia|Cuantitativo|Visión integral del riesgo|
|Ishikawa|Cualitativo|Factores que causan un problema|
|LOPA|Cuantitativo|Efectividad de barreras de defensa|
|Árbol de decisión|Cuantitativo|Evaluación de opciones bajo incertidumbre|
|Confiabilidad humana|Mixto|Errores humanos en seguridad|
|Bow Tie|Mixto|Causas, evento y consecuencias|
|RCM|Mixto|Mantenimiento de activos críticos|
|Circuito furtivo|Cualitativo|Rutas o funciones ocultas no deseadas|
|Markov|Cuantitativo|Disponibilidad de sistemas a lo largo del tiempo|
|Monte Carlo|Cuantitativo|Estimación probabilística de costos|
|Redes bayesianas|Cuantitativo|Dependencias causales entre variables|
|Índices de riesgo|Cuantitativo|Priorización de vulnerabilidades|
|Matriz consecuencia/probabilidad|Mixto|Clasificación visual de riesgos|
|Costo/beneficio|Cuantitativo|Justificación de inversiones en seguridad|
|MCDA|Mixto|Selección de alternativas con múltiples criterios|



