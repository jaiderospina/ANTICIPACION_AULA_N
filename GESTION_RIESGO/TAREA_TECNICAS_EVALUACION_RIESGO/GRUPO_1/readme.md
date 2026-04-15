# Técnicas de Evaluación de Riesgos en Ciberseguridad
## Basado en ISO 31000 e ISO 31010

Este documento presenta un compendio de técnicas de evaluación de riesgos aplicadas al dominio de la ciberseguridad, alineadas con estándares internacionales de gestión de riesgos. Cada técnica incluye una definición breve y un ejemplo aplicado.

<img width="1600" height="1600" alt="WhatsApp Image 2026-04-14 at 14 45 46" src="https://github.com/user-attachments/assets/9c0c467f-8264-403f-9e9c-1c0b8d47d3e1" />

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

**Cuadro Resumen**

<img width="1128" height="507" alt="image" src="https://github.com/user-attachments/assets/a7bc5277-86cc-4f54-a556-df8a88f35518" />
<img width="1128" height="510" alt="image" src="https://github.com/user-attachments/assets/a8908b2e-aa4a-4752-a655-6e187fabc850" />
<img width="1129" height="234" alt="image" src="https://github.com/user-attachments/assets/0209f57b-1274-469c-97c3-e1ca8a76f165" />




