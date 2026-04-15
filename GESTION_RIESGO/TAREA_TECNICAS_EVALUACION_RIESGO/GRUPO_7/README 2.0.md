# Glosario de Técnicas de Evaluación de Riesgos

---
![Diagrama de riesgo](images/riesgogrupo7.png)

## Índice

1. [Lluvia de ideas (Brainstorming)](#1-lluvia-de-ideas-brainstorming)
2. [Entrevista estructurada](#2-entrevista-estructurada)
3. [Delphi](#3-delphi)
4. [Lista de verificación (Checklist)](#4-lista-de-verificación-checklist)
5. [Análisis primario de peligros (PHA)](#5-análisis-primario-de-peligros-pha)
6. [Estudio de peligros y operatividad (HAZOP)](#6-estudio-de-peligros-y-operatividad-hazop)
7. [Análisis de peligros y puntos críticos de control (HACCP)](#7-análisis-de-peligros-y-puntos-críticos-de-control-haccp)
8. [Valoración del riesgo ambiental](#8-valoración-del-riesgo-ambiental)
9. [Estructura "Qué pasa si" (SWIFT)](#9-estructura-qué-pasa-si-swift)
10. [Análisis de escenarios](#10-análisis-de-escenarios)
11. [Análisis de impacto al negocio (BIA)](#11-análisis-de-impacto-al-negocio-bia)
12. [Análisis de causa raíz (RCA)](#12-análisis-de-causa-raíz-rca)
13. [Análisis de modo y efecto de falla (FMEA)](#13-análisis-de-modo-y-efecto-de-falla-fmea)
14. [Análisis de árbol de fallas (FTA)](#14-análisis-de-árbol-de-fallas-fta)
15. [Análisis de árbol de eventos (ETA)](#15-análisis-de-árbol-de-eventos-eta)
16. [Análisis de causa y consecuencia](#16-análisis-de-causa-y-consecuencia)
17. [Análisis de causa/efecto (Ishikawa)](#17-análisis-de-causaefecto-ishikawa)
18. [Análisis de capas de protección (LOPA)](#18-análisis-de-capas-de-protección-lopa)
19. [Árbol de decisión](#19-árbol-de-decisión)
20. [Análisis de confiabilidad humana](#20-análisis-de-confiabilidad-humana)
21. [Análisis de esquema de corbatín (Bow Tie)](#21-análisis-de-esquema-de-corbatín-bow-tie)
22. [Mantenimiento enfocado en la confiabilidad (RCM)](#22-mantenimiento-enfocado-en-la-confiabilidad-rcm)
23. [Análisis de circuito furtivo](#23-análisis-de-circuito-furtivo)
24. [Análisis de Markov](#24-análisis-de-markov)
25. [Simulación Monte Carlo](#25-simulación-monte-carlo)
26. [Redes bayesianas](#26-redes-bayesianas)
27. [Índices de riesgo](#27-índices-de-riesgo)
28. [Matriz de consecuencia y probabilidad](#28-matriz-de-consecuencia-y-probabilidad)
29. [Análisis de costo/beneficio](#29-análisis-de-costobeneficio)
30. [Análisis de decisión por criterios múltiples (MCDA)](#30-análisis-de-decisión-por-criterios-múltiples-mcda)

---

## 1. Lluvia de ideas (Brainstorming)

**📋 Definición**  
Sesión grupal para identificar de forma creativa posibles amenazas y vulnerabilidades.

**💡 Ejemplo aplicado**  
Reunir al equipo de respuesta a incidentes para imaginar nuevos vectores de ataque contra una API recientemente desplegada.

---

## 2. Entrevista estructurada

**📋 Definición**  
Consulta formal a expertos mediante preguntas predefinidas para recopilar datos sobre riesgos.

**💡 Ejemplo aplicado**  
Entrevistar al administrador de red para detallar los controles de acceso existentes en el centro de datos.

---

## 3. Delphi

**📋 Definición**  
Método para alcanzar un consenso entre expertos de forma anónima y sistemática.

**💡 Ejemplo aplicado**  
Consultar a diversos especialistas externos para determinar la probabilidad de un ciberataque de tipo "zero-day" en el sector energético a cinco años.

---

## 4. Lista de verificación (Checklist)

**📋 Definición**  
Verificación de controles y requisitos frente a una lista de criterios preestablecidos.

**💡 Ejemplo aplicado**  
Auditar una infraestructura de nube siguiendo los puntos de control del estándar ISO/IEC 27001.

---

## 5. Análisis primario de peligros (PHA)

**📋 Definición**  
Identificación temprana de los riesgos más críticos en las fases iniciales de un proyecto.

**💡 Ejemplo aplicado**  
Identificar que la falta de cifrado en una base de datos es el peligro principal antes de lanzar una aplicación móvil.

---

## 6. Estudio de peligros y operatividad (HAZOP)

**📋 Definición**  
Examen sistemático para identificar desviaciones en los procesos que puedan generar riesgos.

**💡 Ejemplo aplicado**  
Analizar el flujo de datos en un cortafuegos (firewall) para detectar reglas que permitan tráfico no deseado por error de configuración.

---

## 7. Análisis de peligros y puntos críticos de control (HACCP)

**📋 Definición**  
Identificación de puntos específicos donde el control es vital para prevenir fallos críticos.

**💡 Ejemplo aplicado**  
Establecer el servidor de autenticación multifactor (MFA) como un punto crítico cuya caída detendría todo el acceso remoto seguro.

---

## 8. Valoración del riesgo ambiental

**📋 Definición**  
Evaluación de riesgos derivados del entorno físico o natural que afectan la infraestructura.

**💡 Ejemplo aplicado**  
Analizar la vulnerabilidad de un centro de datos ante inundaciones o cortes de energía por desastres naturales.

---

## 9. Estructura "Qué pasa si" (SWIFT)

**📋 Definición**  
Técnica de equipo que utiliza preguntas hipotéticas para identificar riesgos.

**💡 Ejemplo aplicado**  
"¿Qué pasa si el proveedor de servicios DNS sufre un ataque de denegación de servicio (DDoS)?"

---

## 10. Análisis de escenarios

**📋 Definición**  
Exploración detallada de situaciones futuras posibles y sus impactos.

**💡 Ejemplo aplicado**  
Simular el impacto operativo y reputacional de un ataque de ransomware que cifre todos los servidores de producción.

---

## 11. Análisis de impacto al negocio (BIA)

**📋 Definición**  
Determinación de las consecuencias de la interrupción de procesos críticos.

**💡 Ejemplo aplicado**  
Calcular la pérdida financiera por hora de inactividad de una plataforma de comercio electrónico.

---

## 12. Análisis de causa raíz (RCA)

**📋 Definición**  
Identificación del origen fundamental de un incidente para evitar su repetición.

**💡 Ejemplo aplicado**  
Determinar que una brecha de datos ocurrió debido a que un desarrollador dejó una clave de acceso expuesta en un repositorio público de código.

---

## 13. Análisis de modo y efecto de falla (FMEA)

**📋 Definición**  
Evaluación de las formas en que un componente puede fallar y las consecuencias de dicha falla.

**💡 Ejemplo aplicado**  
Evaluar qué ocurre si falla el balanceador de carga de un sitio web crítico.

---

## 14. Análisis de árbol de fallas (FTA)

**📋 Definición**  
Método deductivo que parte de un evento no deseado para encontrar sus causas potenciales.

**💡 Ejemplo aplicado**  
Mapear todas las combinaciones de fallos técnicos y humanos que podrían permitir un acceso no autorizado a la base de datos de clientes.

---

## 15. Análisis de árbol de eventos (ETA)

**📋 Definición**  
Método inductivo que parte de un evento inicial y analiza sus posibles evoluciones.

**💡 Ejemplo aplicado**  
Modelar las posibles consecuencias después de que un empleado haga clic en un enlace de phishing.

---

## 16. Análisis de causa y consecuencia

**📋 Definición**  
Combinación de los árboles de fallas y eventos para una visión integral del riesgo.

**💡 Ejemplo aplicado**  
Analizar el origen de un fallo en el sistema de respaldo y cómo ese fallo escala hasta la pérdida total de datos.

---

## 17. Análisis de causa/efecto (Ishikawa)

**📋 Definición**  
Representación visual de los factores que contribuyen a un problema de seguridad.

**💡 Ejemplo aplicado**  
Diagramar los factores (personal, tecnología, procesos) que causan lentitud en la aplicación de parches de seguridad.

---

## 18. Análisis de capas de protección (LOPA)

**📋 Definición**  
Evaluación de la efectividad de las barreras de defensa sucesivas.

**💡 Ejemplo aplicado**  
Analizar cómo el firewall, el antivirus y la segmentación de red actúan como capas independientes para detener una intrusión.

---

## 19. Árbol de decisión

**📋 Definición**  
Modelo gráfico para evaluar opciones y sus resultados probables bajo incertidumbre.

**💡 Ejemplo aplicado**  
Decidir entre pagar un rescate en un ataque de ransomware o intentar restaurar desde copias de seguridad de hace 48 horas.

---

## 20. Análisis de confiabilidad humana

**📋 Definición**  
Estudio del impacto de los errores u omisiones humanas en la seguridad del sistema.

**💡 Ejemplo aplicado**  
Evaluar la probabilidad de que un administrador de sistemas configure incorrectamente una política de permisos en la nube.

---

## 21. Análisis de esquema de corbatín (Bow Tie)

**📋 Definición**  
Visualización del riesgo que une las causas, el evento central y las consecuencias, mostrando las barreras preventivas y reactivas.

**💡 Ejemplo aplicado**  
Visualizar una infección por malware, situando el software antivirus como barrera preventiva y el plan de recuperación ante desastres como barrera reactiva.

---

## 22. Mantenimiento enfocado en la confiabilidad (RCM)

**📋 Definición**  
Estrategia para asegurar que los activos continúen realizando su función de seguridad.

**💡 Ejemplo aplicado**  
Establecer un programa riguroso de actualizaciones y pruebas de hardware para los servidores del centro de operaciones de seguridad (SOC).

---

## 23. Análisis de circuito furtivo

**📋 Definición**  
Identificación de rutas o funciones no deseadas que pueden activarse en condiciones específicas.

**💡 Ejemplo aplicado**  
Detectar "puertas traseras" o funciones de administración ocultas en el código de una aplicación antigua.

---

## 24. Análisis de Markov

**📋 Definición**  
Modelado matemático de sistemas que cambian de estado de forma aleatoria con el tiempo.

**💡 Ejemplo aplicado**  
Predecir la disponibilidad de un sistema crítico basándose en el tiempo medio entre fallos y el tiempo medio de reparación.

---

## 25. Simulación Monte Carlo

**📋 Definición**  
Uso de muestreo aleatorio para modelar la probabilidad de diferentes resultados en situaciones inciertas.

**💡 Ejemplo aplicado**  
Realizar miles de simulaciones para estimar el costo total anual esperado por incidentes de ciberseguridad.

---

## 26. Redes bayesianas

**📋 Definición**  
Modelos probabilísticos que representan variables y sus dependencias causales.

**💡 Ejemplo aplicado**  
Estimar la probabilidad de una amenaza persistente avanzada (APT) basándose en una serie de anomalías detectadas en el tráfico de red.

---

## 27. Índices de riesgo

**📋 Definición**  
Puntajes numéricos utilizados para priorizar riesgos según métricas específicas.

**💡 Ejemplo aplicado**  
Utilizar el sistema de puntuación CVSS para priorizar el parcheo de vulnerabilidades según su gravedad técnica.

---

## 28. Matriz de consecuencia y probabilidad

**📋 Definición**  
Herramienta visual que clasifica los riesgos según su impacto y su frecuencia esperada.

**💡 Ejemplo aplicado**  
Ubicar el riesgo de "fuga de información por empleado descontento" en un cuadrante de alto impacto y baja probabilidad.

---

## 29. Análisis de costo/beneficio

**📋 Definición**  
Comparación entre el costo de implementar una medida de seguridad y el beneficio (reducción de riesgo) obtenido.

**💡 Ejemplo aplicado**  
Evaluar si la inversión en un sistema de detección de intrusos (IDS) de 100,000 USD justifica la prevención de una brecha que costaría 1 millón de USD.

---

## 30. Análisis de decisión por criterios múltiples (MCDA)

**📋 Definición**  
Evaluación de alternativas de seguridad basadas en diversos criterios contrapuestos.

**💡 Ejemplo aplicado**  
Seleccionar un proveedor de seguridad gestionada evaluando costo, experiencia técnica, cumplimiento legal y tiempos de respuesta.

---

*Glosario de 30 técnicas esenciales en ciberseguridad y gestión de riesgos.*
