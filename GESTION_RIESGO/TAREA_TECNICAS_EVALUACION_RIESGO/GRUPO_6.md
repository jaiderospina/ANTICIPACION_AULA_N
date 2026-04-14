# Glosario de Técnicas de Análisis de Riesgo Aplicadas a la Ciberseguridad y Ciberdefensa Marítima

Este documento presenta un glosario sintético de técnicas de análisis de riesgo, con ejemplos aplicados al contexto de la **ciberseguridad** y la **ciberdefensa**, especialmente en sistemas embarcados, buques, redes OT marítimas, sistemas de navegación, puente y máquinas.

## Propósito

El objetivo de este glosario es servir como base conceptual para trabajos académicos, artículos, matrices de análisis o evaluaciones de riesgo en entornos marítimos, donde las amenazas cibernéticas pueden afectar la seguridad de la navegación, la continuidad operativa y la misión institucional.

---

## 1. Lluvia de ideas (Brainstorming)

**Definición:**  
Técnica grupal para generar rápidamente amenazas, vulnerabilidades, fallas o escenarios posibles, sin filtrar inicialmente las ideas.

**Ejemplo en ciberseguridad marítima:**  
Un equipo del buque identifica posibles vectores de ataque contra ECDIS, AIS, red administrativa, CCTV, PLC de lastre y sistema satelital.

---

## 2. Entrevista estructurada

**Definición:**  
Recolección sistemática de información mediante preguntas definidas previamente a operadores, técnicos o responsables de procesos.

**Ejemplo en ciberseguridad marítima:**  
Entrevistar al oficial de guardia, al jefe de máquinas y al administrador TI para identificar cómo se conectan memorias USB a sistemas críticos de navegación.

---

## 3. Método Delphi

**Definición:**  
Consulta iterativa a expertos, en rondas, buscando convergencia de criterio sin presión directa entre ellos.

**Ejemplo en ciberseguridad marítima:**  
Solicitar a especialistas navales, OT y ciberdefensa que valoren cuál es el mayor riesgo cibernético de un patrullero: GPS spoofing, ransomware en red logística o compromiso del sistema de propulsión auxiliar.

---

## 4. Lista de verificación (Checklist)

**Definición:**  
Listado de controles o condiciones que se revisan para detectar ausencias, incumplimientos o debilidades.

**Ejemplo en ciberseguridad marítima:**  
Verificar si el buque tiene segmentación entre IT y OT, control de puertos USB, respaldo offline de cartas electrónicas y cuentas privilegiadas separadas.

---

## 5. Análisis primario de peligros (PHA)

**Definición:**  
Identificación temprana y rápida de peligros relevantes antes de entrar a un análisis más detallado.

**Ejemplo en ciberseguridad marítima:**  
En la fase de alistamiento de un buque se identifican como peligros principales la manipulación remota de sensores, pérdida de integridad del GPS y acceso no autorizado a la red de control.

---

## 6. Estudio de peligros y operatividad (HAZOP)

**Definición:**  
Método estructurado que analiza desviaciones respecto al funcionamiento esperado usando palabras guía como “más”, “menos”, “ninguno” o “inverso”.

**Ejemplo en ciberseguridad marítima:**  
En el sistema de combustible controlado digitalmente se analiza la desviación “sin señal”, “señal errónea” o “más caudal del esperado” causada por manipulación cibernética.

---

## 7. Análisis de peligros y puntos críticos de control (HACCP)

**Definición:**  
Método enfocado en identificar puntos donde un peligro puede prevenirse, detectarse o controlarse.

**Ejemplo en ciberseguridad marítima:**  
Definir como puntos críticos el servidor de autenticación del buque, la consola ECDIS y el gateway entre red administrativa y red de control.

---

## 8. Valoración del riesgo ambiental

**Definición:**  
Análisis del riesgo sobre el entorno natural por una falla o incidente.

**Ejemplo en ciberseguridad marítima:**  
Evaluar cómo un ciberataque al sistema de lastre o al sistema de combustible puede derivar en vertimiento, colisión o encallamiento con impacto ambiental.

---

## 9. Estructura “¿qué pasa si?” (SWIFT)

**Definición:**  
Técnica basada en preguntas del tipo “¿qué pasa si...?” para explorar fallas, eventos no deseados y sus consecuencias.

**Ejemplo en ciberseguridad marítima:**  
¿Qué pasa si un atacante altera la hora del servidor?, ¿qué pasa si el AIS transmite una posición falsa?, ¿qué pasa si el enlace satelital cae durante una maniobra de aproximación?

---

## 10. Análisis de escenarios

**Definición:**  
Construcción de situaciones plausibles futuras para entender exposición, impacto y respuesta.

**Ejemplo en ciberseguridad marítima:**  
Escenario 1: ransomware en puerto.  
Escenario 2: spoofing de GPS en aproximación.  
Escenario 3: compromiso del sistema de mantenimiento predictivo conectado al fabricante.

---

## 11. Análisis de impacto al negocio (BIA)

**Definición:**  
Determina qué activos, procesos y servicios son críticos, cuánto daño genera su pérdida y qué dependencias existen.

**Ejemplo en ciberseguridad marítima:**  
Establecer que perder ECDIS o el servidor de comunicaciones en una unidad naval afecta la misión, la seguridad de la navegación, la continuidad operativa y la capacidad de mando y control.

---

## 12. Análisis de causa raíz (RCA)

**Definición:**  
Busca la causa fundamental de un incidente, no solo el síntoma visible.

**Ejemplo en ciberseguridad marítima:**  
Tras una caída del sistema de monitoreo de motores, descubrir que la causa raíz no fue error del operador sino una actualización remota mal controlada y sin validación.

---

## 13. Análisis de modo y efecto de falla (AMEF / FMEA)

**Definición:**  
Identifica modos de falla, sus efectos y, en algunos casos, su criticidad y detectabilidad.

**Ejemplo en ciberseguridad marítima:**  
Modo de falla: sensor de rumbo entrega dato manipulado.  
Efecto: error de navegación.  
Consecuencia: riesgo de derrota insegura o colisión.

---

## 14. Análisis de árbol de fallas (FTA)

**Definición:**  
Método deductivo que parte de un evento no deseado y retrocede lógicamente hacia sus causas.

**Ejemplo en ciberseguridad marítima:**  
Evento superior: pérdida del posicionamiento confiable.  
Causas posibles: spoofing GNSS, fallo de antena, error de configuración o malware en el procesador de datos.

---

## 15. Análisis de árbol de eventos (ETA)

**Definición:**  
Parte de un evento iniciador y sigue ramas según funcionen o fallen controles y barreras.

**Ejemplo en ciberseguridad marítima:**  
Evento iniciador: entrada de malware por USB.  
Ramas: antivirus detecta/no detecta, segmentación contiene/no contiene, respaldo restaura/no restaura.

---

## 16. Análisis de causa y consecuencias (CCA)

**Definición:**  
Combina el enfoque de causas y consecuencias en un solo modelo lógico.

**Ejemplo en ciberseguridad marítima:**  
Causa inicial: acceso remoto no autorizado al PLC de bombas.  
Consecuencias: pérdida de control, inundación local, degradación de la misión y parada de operación.

---

## 17. Análisis de causa/efecto (Ishikawa)

**Definición:**  
Organiza posibles causas de un problema por categorías.

**Ejemplo en ciberseguridad marítima:**  
Incidente: caída de la red OT.  
Causas agrupadas en personas, procesos, software, hardware, comunicaciones, proveedor y configuración.

---

## 18. Análisis de capas de protección (LOPA)

**Definición:**  
Evalúa si existen barreras independientes suficientes para reducir un riesgo a un nivel aceptable.

**Ejemplo en ciberseguridad marítima:**  
Frente a acceso no autorizado al sistema de propulsión, las capas pueden ser autenticación multifactor, firewall industrial, segmentación, listas blancas, enclavamiento manual y parada segura local.

---

## 19. Árbol de decisión

**Definición:**  
Modelo de decisiones secuenciales que compara opciones, criterios y resultados posibles.

**Ejemplo en ciberseguridad marítima:**  
Decidir si un buque debe aislar completamente la red satelital al detectar una intrusión, mantener la misión degradada o migrar a operación manual.

---

## 20. Análisis de confiabilidad humana (HRA)

**Definición:**  
Evalúa la probabilidad de error humano dentro de una tarea crítica y sus factores condicionantes.

**Ejemplo en ciberseguridad marítima:**  
Estimar la probabilidad de que un operador conecte un USB no autorizado al ECDIS durante una actualización urgente en navegación.

---

## 21. Análisis de esquema de corbatín (BowTie)

**Definición:**  
Representa en un solo diagrama el evento central, sus causas, consecuencias y barreras preventivas y mitigadoras.

**Ejemplo en ciberseguridad marítima:**  
Evento central: compromiso del ECDIS.  
A la izquierda: USB infectado o credenciales robadas.  
A la derecha: derrota errónea, riesgo de varada y pérdida de continuidad operativa.

---

## 22. Mantenimiento enfocado en la confiabilidad (RCM)

**Definición:**  
Define qué mantenimiento conviene aplicar para asegurar que los sistemas sigan cumpliendo su función.

**Ejemplo en ciberseguridad marítima:**  
Incluir en el RCM del buque pruebas periódicas de respaldo, validación de firmware, revisión de logs y verificación de integridad de estaciones críticas OT.

---

## 23. Análisis de circuito furtivo

**Definición:**  
Busca condiciones ocultas de diseño o lógica que producen comportamientos no deseados sin que exista una falla física evidente.

**Ejemplo en ciberseguridad marítima:**  
Una combinación de estados en una red de control permite que una consola de mantenimiento habilite funciones de mando sin autorización formal.

---

## 24. Análisis de Markov

**Definición:**  
Modelo probabilístico de estados y transiciones útil cuando el sistema cambia entre condiciones operativas.

**Ejemplo en ciberseguridad marítima:**  
Modelar estados de una red del buque: normal, degradada, comprometida, contenida y recuperada, con probabilidades de transición según controles y respuesta.

---

## 25. Simulación Monte Carlo

**Definición:**  
Ejecuta muchas iteraciones aleatorias para estimar probabilidades, impactos o distribuciones de riesgo.

**Ejemplo en ciberseguridad marítima:**  
Simular miles de incidentes combinando probabilidad de phishing exitoso, tiempo de detección y efectividad del aislamiento para estimar pérdida operativa anual del buque.

---

## 26. Redes bayesianas

**Definición:**  
Modelo probabilístico que representa dependencias entre variables y actualiza probabilidades cuando aparece nueva evidencia.

**Ejemplo en ciberseguridad marítima:**  
Si se observa tráfico anómalo y pérdida intermitente de GPS, la red bayesiana actualiza la probabilidad de spoofing frente a una falla técnica ordinaria.

---

## 27. Índices de riesgo

**Definición:**  
Puntajes semicuantitativos que combinan factores para comparar riesgos entre sí.

**Ejemplo en ciberseguridad marítima:**  
Asignar un índice a cada sistema embarcado según criticidad, exposición, conectividad, dificultad de recuperación y consecuencias sobre la seguridad de la navegación.

---

## 28. Matriz de consecuencia y probabilidad

**Definición:**  
Cruza impacto y probabilidad para clasificar riesgos en niveles.

**Ejemplo en ciberseguridad marítima:**  
Un ataque de GPS spoofing puede clasificarse como probabilidad media e impacto alto en un buque en aproximación costera, quedando en zona roja.

---

## 29. Análisis de costo/beneficio

**Definición:**  
Compara el costo de un control frente a la reducción de riesgo o pérdida esperada evitada.

**Ejemplo en ciberseguridad marítima:**  
Justificar económicamente la segmentación OT, el reemplazo de switches no gestionables y la implementación de respaldos inmutables frente al costo potencial de una indisponibilidad del buque.

---

## 30. Análisis de decisión por criterios múltiples (MCDA)

**Definición:**  
Evalúa varias alternativas con varios criterios ponderados.

**Ejemplo en ciberseguridad marítima:**  
Seleccionar una solución de ciberseguridad marítima comparando costo, facilidad de integración, robustez OT, soporte offline, cumplimiento normativo y efecto en la misión.

---

## Observación final

No todas estas técnicas son exclusivas de la ciberseguridad. Muchas provienen de la ingeniería de seguridad, confiabilidad, continuidad operacional y gestión del riesgo. Sin embargo, hoy son plenamente aplicables a la ciberseguridad y ciberdefensa porque permiten analizar amenazas que afectan:

- Disponibilidad
- Integridad
- Confidencialidad
- Continuidad de la misión
- Seguridad operacional
- Resiliencia organizacional

En el entorno marítimo, su valor aumenta porque los sistemas IT y OT del buque están interconectados y un incidente cibernético puede traducirse en consecuencias físicas, operacionales, ambientales y estratégicas.

---

## Nombres normalizados de las técnicas

Para uso académico, se recomienda emplear la siguiente nomenclatura:

- Lluvia de ideas
- Entrevista estructurada
- Método Delphi
- Lista de verificación
- Análisis primario de peligros
- HAZOP
- HACCP
- Valoración del riesgo ambiental
- SWIFT
- Análisis de escenarios
- Análisis de impacto al negocio
- Análisis de causa raíz
- AMEF / FMEA
- Árbol de fallas
- Árbol de eventos
- Análisis de causa y consecuencias
- Análisis causa/efecto
- LOPA
- Árbol de decisión
- Análisis de confiabilidad humana
- BowTie
- Mantenimiento enfocado en la confiabilidad
- Análisis de circuito furtivo
- Análisis de Markov
- Simulación Monte Carlo
- Redes bayesianas
- Índices de riesgo
- Matriz de consecuencia y probabilidad
- Análisis de costo/beneficio
- Análisis de decisión por criterios múltiples
