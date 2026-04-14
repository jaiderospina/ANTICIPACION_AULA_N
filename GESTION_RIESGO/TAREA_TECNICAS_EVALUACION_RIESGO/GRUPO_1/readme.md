# Técnicas de Evaluación de Riesgos en Ciberseguridad
## Basado en ISO 31000 e ISO 31010

Este documento presenta un compendio de técnicas de evaluación de riesgos aplicadas al dominio de la ciberseguridad, alineadas con estándares internacionales de gestión de riesgos. Cada técnica incluye una definición breve y un ejemplo aplicado.


## 1. Técnicas de Identificación de Riesgos

### Lluvia de ideas
**Definición:** Técnica cualitativa colaborativa para identificar riesgos mediante generación libre de ideas sin filtros iniciales.  
**Ejemplo:** Equipo de ciberdefensa identifica vectores como ransomware, phishing y ataques a la cadena de suministro.


### Entrevista estructurada
**Definición:** Recolección sistemática de información mediante preguntas predefinidas a expertos.  
**Ejemplo:** Entrevistar al administrador OT para identificar debilidades en segmentación de red.


### Método Delphi
**Definición:** Consulta iterativa a expertos para lograr consenso mediante rondas anónimas.  
**Ejemplo:** Expertos estiman probabilidad de ciberataques en infraestructura crítica.


### Lista de verificación (Checklist)
**Definición:** Comparación contra listas de control basadas en estándares.  
**Ejemplo:** Validar uso de MFA, cifrado y parches según NIST.


## 2. Técnicas de Análisis de Peligros

### Análisis primario de peligros (PHA)
**Definición:** Identificación temprana de riesgos antes de implementar sistemas.  
**Ejemplo:** Detectar transmisión de datos sin cifrado en sistemas tácticos.


### HAZOP
**Definición:** Análisis estructurado de desviaciones mediante palabras guía.  
**Ejemplo:** “No autenticación” → acceso no autorizado.


### SWIFT
**Definición:** Técnica basada en preguntas “¿qué pasaría si…?”.  
**Ejemplo:** ¿Qué pasa si comprometen el servidor central?


## 3. Técnicas de Análisis de Fallas

### AMEF (FMEA)
**Definición:** Identifica modos de falla, causas y efectos, priorizando riesgos.  
**Ejemplo:** Falla en autenticación → acceso indebido → impacto en datos clasificados.


### Árbol de fallas (FTA)
**Definición:** Análisis deductivo de causas de eventos críticos.  
**Ejemplo:** Brecha causada por phishing + falta de MFA.


### Árbol de eventos (ETA)
**Definición:** Análisis inductivo de consecuencias tras un evento.  
**Ejemplo:** Intrusión → contención o escalamiento.


## 4. Impacto y Negocio

### Análisis de impacto al negocio (BIA)
**Definición:** Evalúa consecuencias operativas y estratégicas.  
**Ejemplo:** Caída de sistema militar afecta operaciones.


### Valoración del riesgo ambiental
**Definición:** Evalúa impacto ambiental de riesgos tecnológicos.  
**Ejemplo:** Ataque a sistema energético genera daño ambiental.


## 5. Técnicas Causales

### Análisis de causa raíz (RCA)
**Definición:** Identifica causa fundamental de incidentes.  
**Ejemplo:** Brecha por mala configuración en la nube.


### Análisis causa–efecto
**Definición:** Relaciona causas potenciales de un problema.  
**Ejemplo:** Fuga de datos por factores humanos y tecnológicos.


### Análisis causa y consecuencia
**Definición:** Integra causas y efectos en un modelo completo.  
**Ejemplo:** Vulnerabilidad → explotación → impacto.


## 6. Confiabilidad

### Análisis de confiabilidad humana (HRA)
**Definición:** Evalúa errores humanos en sistemas.  
**Ejemplo:** Configuración incorrecta de firewall.


### Mantenimiento centrado en confiabilidad (RCM)
**Definición:** Estrategia para garantizar disponibilidad de sistemas.  
**Ejemplo:** Actualización continua de sistemas OT.


## 7. Técnicas Cuantitativas

### Simulación Monte Carlo
**Definición:** Simulación probabilística de múltiples escenarios.  
**Ejemplo:** Probabilidad de ataque exitoso anual.


### Redes bayesianas
**Definición:** Modelos probabilísticos con dependencias entre variables.  
**Ejemplo:** Riesgo depende de vulnerabilidad y controles.


### Análisis de Markov
**Definición:** Modela transición entre estados del sistema.  
**Ejemplo:** Seguro → vulnerable → comprometido.


## 8. Barreras y Controles

### LOPA
**Definición:** Evalúa capas de protección independientes.  
**Ejemplo:** Firewall + IDS + SOC reducen riesgo.


### Bow-Tie
**Definición:** Relaciona causas, evento y consecuencias con controles.  
**Ejemplo:** Phishing mitigado con MFA y capacitación.


## 9. Decisión y Priorización

### Matriz probabilidad–impacto
**Definición:** Clasifica riesgos por severidad.  
**Ejemplo:** Ransomware = riesgo crítico.


### Índices de riesgo
**Definición:** Valor numérico del riesgo.  
**Ejemplo:** Riesgo = probabilidad × impacto.


### Árbol de decisión
**Definición:** Evalúa decisiones bajo incertidumbre.  
**Ejemplo:** Elegir entre SIEM o XDR.


### Análisis multicriterio (MCDA)
**Definición:** Toma decisiones con múltiples variables.  
**Ejemplo:** Evaluar herramientas por costo y eficacia.


### Costo–beneficio
**Definición:** Compara inversión frente a reducción de riesgo.  
**Ejemplo:** Implementar SOC reduce pérdidas mayores.


## 10. Otras Técnicas

### Análisis de escenarios
**Definición:** Construye posibles futuros para evaluar riesgos.  
**Ejemplo:** Guerra híbrida con ataques cibernéticos.


### HACCP
**Definición:** Identifica puntos críticos de control.  
**Ejemplo:** Autenticación como punto crítico.


### Análisis de circuito furtivo
**Definición:** Detecta rutas no intencionadas en sistemas.  
**Ejemplo:** Canal oculto para exfiltración de datos.

**cuadro resumen**

TÉCNICAS DE EVALUACIÓN DEL RIESGO — Aplicadas a Ciberseguridad y Ciberdefensa				
 ISO/IEC 31010:2019 — Gestión del riesgo – Técnicas de apreciación del riesgo				
				
N.°	Técnica	Definición	Norma de referencia	Ejemplo en Ciberseguridad y Ciberdefensa
1	Lluvia de ideas (Brainstorming)	Técnica grupal para generar ideas y recopilar información sobre fuentes de riesgo, eventos, causas y consecuencias potenciales mediante discusión libre y colaborativa.	"ISO/IEC 31010:2019
Anexo A, Cláusula B.1"	Reunión del equipo CSIRT para identificar posibles vectores de ataque contra la infraestructura crítica del sector defensa colombiano antes de un ejercicio de ciberdefensa.
2	Entrevista estructurada	Método en el que se formulan preguntas predefinidas a individuos clave para identificar riesgos, causas, consecuencias y controles existentes de manera sistemática.	"ISO/IEC 31010:2019
Anexo A, Cláusula B.2"	Entrevistas a oficiales de seguridad de la información de las Fuerzas Militares para evaluar el estado de madurez de los controles de acceso a sistemas clasificados.
3	Delphi	Técnica que busca el consenso de un panel de expertos de forma anónima e iterativa, reduciendo sesgos y logrando convergencia de opiniones sobre riesgos complejos.	"ISO/IEC 31010:2019
Anexo A, Cláusula B.3"	Consulta a expertos internacionales en ciberdefensa para estimar la probabilidad de ataques APT patrocinados por Estados contra infraestructura militar colombiana.
4	Lista de verificación (Checklist)	Listado predefinido de peligros, riesgos o fallas de control usado para identificar riesgos de manera rápida y estandarizada, basado en experiencia previa o normas.	"ISO/IEC 31010:2019
Anexo A, Cláusula B.4"	Aplicación de checklist basado en ISO 27001 para verificar cumplimiento de controles de seguridad en el Centro de Operaciones de Seguridad (SOC) de la Escuela Superior de Guerra.
5	Análisis primario de peligros (PHA)	Método cualitativo para identificar situaciones y eventos peligrosos que pueden causar daño en una etapa temprana del ciclo de vida de un sistema.	"ISO/IEC 31010:2019
Anexo A, Cláusula B.5"	Evaluación preliminar de amenazas cibernéticas durante la fase de diseño de un nuevo sistema de comunicaciones militares cifradas.
6	Estudio de peligros y operatividad (HAZOP)	Técnica sistemática para identificar desviaciones del diseño o funcionamiento previsto mediante el uso de palabras guía aplicadas a parámetros del sistema.	"ISO/IEC 31010:2019
Anexo A, Cláusula B.6"	Análisis de desviaciones en los flujos de datos de un sistema SCADA del sector energético colombiano para detectar puntos vulnerables a ciberataques.
7	Análisis de peligros y puntos críticos de control (HACCP)	Metodología para identificar peligros significativos y establecer puntos críticos de control donde se pueden aplicar medidas preventivas.	"ISO/IEC 31010:2019
Anexo A, Cláusula B.7"	Identificación de puntos críticos de control en el flujo de procesamiento de inteligencia cibernética donde una alteración de datos comprometería decisiones estratégicas.
8	Valoración del riesgo ambiental	Proceso de identificación y evaluación de riesgos que una actividad, producto o proceso representa para el medio ambiente y las personas expuestas.	"ISO/IEC 31010:2019
Anexo A, Cláusula B.8"	Evaluación del impacto ambiental de un ciberataque a sistemas de monitoreo de represas o plantas de tratamiento de agua controladas por SCADA en Colombia.
9	Estructura "qué pasa si" (SWIFT)	Técnica de identificación de riesgos basada en preguntas "¿qué pasa si...?" aplicadas sistemáticamente a un proceso, sistema o situación.	"ISO/IEC 31010:2019
Anexo A, Cláusula B.9"	Sesión SWIFT planteando escenarios como: ¿Qué pasa si un atacante compromete las credenciales del administrador de la nube del Ministerio de Defensa?
10	Análisis de escenarios	Descripción sistemática de futuros posibles basada en suposiciones sobre cómo podrían desarrollarse los eventos, para anticipar riesgos y oportunidades.	"ISO/IEC 31010:2019
Anexo A, Cláusula B.10"	Construcción de escenarios de ciberguerra simulando un ataque coordinado contra infraestructura crítica colombiana (energía, telecomunicaciones, banca) por un actor estatal.
11	Análisis de impacto al negocio (BIA)	Proceso que determina las funciones críticas de una organización y evalúa el impacto que tendría la interrupción de dichas funciones en términos de tiempo, costo y operación.	"ISO/IEC 31010:2019
Anexo A, Cláusula B.11"	Evaluación del impacto de la caída del sistema de comando y control (C2) de las Fuerzas Militares durante una operación conjunta por un ataque de ransomware.
12	Análisis de causa raíz (RCA)	Método para identificar las causas fundamentales de un evento no deseado, en lugar de tratar solo los síntomas, para prevenir su recurrencia.	"ISO/IEC 31010:2019
Anexo A, Cláusula B.12"	Investigación forense digital tras una brecha de seguridad en servidores del Ejército para determinar si la causa raíz fue phishing, vulnerabilidad no parcheada o amenaza interna.
13	Análisis de modo y efecto de falla (FMEA/EMEF)	Técnica que identifica los modos de falla potenciales de cada componente de un sistema y evalúa sus efectos sobre el desempeño del sistema.	"ISO/IEC 31010:2019
Anexo A, Cláusula B.13"	Análisis de modos de falla del firewall perimetral de una red militar: falla de reglas, saturación de tabla de estados, bypass por túnel cifrado no autorizado.
14	Análisis de árbol de fallas (FTA)	Técnica deductiva (de arriba hacia abajo) que modela las combinaciones de eventos que pueden producir un evento no deseado, usando lógica booleana.	"ISO/IEC 31010:2019
Anexo A, Cláusula B.14"	Modelado del árbol de fallas para el evento raíz "exfiltración masiva de datos clasificados", identificando combinaciones de fallas en DLP, cifrado y control de acceso.
15	Análisis de árbol de eventos (ETA)	Técnica inductiva (de abajo hacia arriba) que modela las secuencias de eventos posteriores a un evento iniciador, incluyendo éxito o falla de las barreras.	"ISO/IEC 31010:2019
Anexo A, Cláusula B.15"	A partir del evento iniciador "correo de spear-phishing abierto por oficial", modelar las ramas: ¿antivirus lo detecta?, ¿el sandbox lo bloquea?, ¿se ejecuta el payload?
16	Análisis de causa y consecuencia	Combinación de árbol de fallas y árbol de eventos que vincula causas con consecuencias, proporcionando una visión integral de las cadenas de riesgo.	"ISO/IEC 31010:2019
Anexo A, Cláusula B.16"	Análisis que vincula causas (vulnerabilidad zero-day en software militar) con consecuencias (acceso a inteligencia operativa, pérdida de vidas en operación).
17	Análisis de causa/efecto (Ishikawa)	Diagrama que organiza las posibles causas de un efecto o problema en categorías principales para facilitar la identificación de causas raíz.	"ISO/IEC 31010:2019
Anexo A, Cláusula B.17"	Diagrama de espina de pescado para analizar las causas de incidentes recurrentes de fuga de información: personas, procesos, tecnología, políticas, entorno.
18	Análisis de capas de protección (LOPA)	Método semicuantitativo que evalúa si las capas de protección independientes son suficientes para reducir el riesgo de un escenario a un nivel tolerable.	"ISO/IEC 31010:2019
Anexo A, Cláusula B.18"	Evaluación de capas de defensa en profundidad: firewall → IDS/IPS → segmentación → EDR → SOC, para determinar si reducen el riesgo de intrusión APT a nivel aceptable.
19	Árbol de decisión	Representación gráfica de decisiones secuenciales y sus posibles resultados, incluyendo probabilidades y valores, para seleccionar la mejor opción.	"ISO/IEC 31010:2019
Anexo A, Cláusula B.19"	Árbol de decisión para evaluar si invertir en un nuevo SOC propio vs. contratar un SOC gestionado vs. un modelo híbrido, considerando costos, riesgos y capacidades.
20	Análisis de confiabilidad humana (HRA)	Técnica para identificar y evaluar los errores humanos que pueden contribuir a la ocurrencia de eventos no deseados en un sistema.	"ISO/IEC 31010:2019
Anexo A, Cláusula B.20"	Evaluación de la probabilidad de error humano de analistas del SOC al clasificar alertas durante turnos nocturnos de 12 horas en operaciones de ciberdefensa.
21	Mantenimiento enfocado en la confiabilidad (RCM)	Proceso para determinar los requisitos de mantenimiento de activos físicos en su contexto operativo, enfocándose en preservar funciones críticas.	"ISO/IEC 31010:2019
Anexo A, Cláusula B.21"	Definición de políticas de parcheo y actualización de firmware para equipos de red y servidores críticos de la red militar, priorizando según criticidad operativa.
22	Análisis de circuito furtivo (Sneak Circuit)	Técnica para identificar condiciones de diseño latentes no previstas que pueden causar eventos no deseados o impedir funciones deseadas.	"ISO/IEC 31010:2019
Anexo A, Cláusula B.22"	Detección de backdoors no documentadas o conexiones lógicas ocultas en el firmware de equipos de telecomunicaciones adquiridos para uso militar.
23	Análisis de esquema de corbatín (Bow Tie)	Diagrama que muestra la relación entre las causas de un evento de riesgo (izquierda), el evento central, y las consecuencias (derecha), junto con las barreras de control.	"ISO/IEC 31010:2019
Anexo A, Cláusula B.23"	Diagrama Bow Tie para el evento "compromiso de credenciales privilegiadas": causas (phishing, fuerza bruta, insider) y consecuencias (movimiento lateral, exfiltración), con barreras MFA, PAM y monitoreo.
24	Simulación Monte Carlo	Técnica cuantitativa que utiliza muestreo aleatorio repetido para modelar la incertidumbre y obtener distribuciones de probabilidad de los resultados posibles.	"ISO/IEC 31010:2019
Anexo A, Cláusula B.24"	Simulación de 10.000 escenarios para estimar la pérdida económica esperada por ciberataques al sector financiero colombiano en un horizonte de un año.
25	Análisis de Markov	Técnica que modela sistemas con múltiples estados y transiciones probabilísticas entre ellos para calcular la disponibilidad y confiabilidad del sistema.	"ISO/IEC 31010:2019
Anexo A, Cláusula B.25"	Modelado de los estados de un sistema de defensa cibernética (operativo, degradado, comprometido, recuperación) y las probabilidades de transición ante distintos tipos de ataque.
26	Redes bayesianas	Modelos probabilísticos gráficos que representan relaciones de dependencia condicional entre variables, permitiendo actualizar probabilidades con nueva evidencia.	"ISO/IEC 31010:2019
Anexo A, Cláusula B.26"	Red bayesiana para estimar la probabilidad de un ataque exitoso de ransomware, condicionada a variables como nivel de parcheo, capacitación del personal y segmentación de red.
27	Índices de riesgo	Método semicuantitativo que combina estimaciones de factores de riesgo en un índice numérico único para clasificar y priorizar riesgos.	"ISO/IEC 31010:2019
Anexo A, Cláusula B.27"	Cálculo de un índice de riesgo cibernético para cada unidad militar, ponderando factores como exposición a internet, volumen de datos clasificados, madurez de controles y amenazas conocidas.
28	Matriz de consecuencia y probabilidad	Herramienta que combina niveles cualitativos o semicuantitativos de consecuencia y probabilidad en una matriz para clasificar riesgos por prioridad.	"ISO/IEC 31010:2019
Anexo A, Cláusula B.28"	Matriz 5×5 para clasificar ciberriesgos del Ministerio de Defensa: probabilidad (raro a casi seguro) vs. impacto (insignificante a catastrófico), ubicando amenazas como ransomware, DDoS y espionaje.
29	Análisis de costo/beneficio	Comparación sistemática de los costos de implementar controles de riesgo frente a los beneficios esperados de la reducción del riesgo.	"ISO/IEC 31010:2019
Anexo A, Cláusula B.29"	Análisis costo-beneficio de implementar un sistema de inteligencia de amenazas (CTI) en las Fuerzas Militares vs. el costo potencial de no detectar un ataque APT a tiempo.
30	Análisis de decisión por criterios múltiples (MCDA)	Método que evalúa y compara opciones de tratamiento de riesgo considerando múltiples criterios simultáneamente, ponderados según su importancia relativa.	"ISO/IEC 31010:2019
Anexo A, Cláusula B.30"	Evaluación multicriterio (costo, tiempo de implementación, efectividad, compatibilidad) para seleccionar la plataforma SIEM más adecuada para el comando cibernético colombiano.
