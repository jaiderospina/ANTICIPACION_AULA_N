# GESTIÓN DEL RIESGO.

La gestión del riesgo es el proceso estratégico y técnico de identificar, evaluar y tratar las amenazas que pueden comprometer la integridad, disponibilidad y confidencialidad de la información.

Aunque a menudo se usan como sinónimos, la gestión del riesgo varía ligeramente en su enfoque dependiendo de si hablamos de **ciberseguridad** (protección de activos) o **ciberdefensa** (protección de la soberanía y respuesta ante ataques dirigidos).

---

## 1. Gestión del Riesgo en Ciberseguridad
En este ámbito, el enfoque es primordialmente **organizacional y preventivo**. Se trata de proteger el ecosistema digital de una entidad (datos, usuarios, procesos).

* **Identificación de Activos:** Saber qué se protege (bases de datos, infraestructura crítica, propiedad intelectual).
* **Análisis de Vulnerabilidades:** Detectar fallos técnicos o de procesos (puertos abiertos, falta de parches, errores humanos).
* **Evaluación de Amenazas:** Evaluar la probabilidad de eventos como phishing, ransomware o fugas de datos.
* **Tratamiento:** Decidir si se **mitiga** el riesgo (poniendo un firewall), se **transfiere** (contratando un ciberseguro), se **evita** (eliminando el proceso riesgoso) o se **acepta** (si el costo de protección es mayor que el valor del activo).

## 2. Gestión del Riesgo en Ciberdefensa
Aquí el enfoque es **proactivo y reactivo**, orientado generalmente a infraestructuras críticas del Estado o entornos militares. La gestión del riesgo en ciberdefensa no solo mira la vulnerabilidad, sino la **intencionalidad del actor**.

* **Inteligencia de Amenazas:** El riesgo se calcula analizando las capacidades de adversarios específicos (grupos de APT, Estados-nación).
* **Resiliencia y Recuperación:** Se asume que el ataque ocurrirá. El riesgo se gestiona asegurando que, a pesar de una intrusión, los servicios críticos (energía, agua, comunicaciones) sigan operando.
* **Disuasión:** Parte de gestionar el riesgo es elevar el "costo de ataque" para el adversario, de modo que el riesgo de ser contraatacado lo disuada de actuar.

---

## Diferencias Clave en el Análisis del Riesgo

| Característica | Ciberseguridad | Ciberdefensa |
| :--- | :--- | :--- |
| **Objetivo** | Continuidad del negocio y protección de datos. | Seguridad nacional y soberanía digital. |
| **Origen del Riesgo** | Accidentes, errores, cibercrimen común. | Ataques dirigidos, espionaje estatal, sabotaje. |
| **Enfoque** | Protección de la red interna (perimetral). | Protección del ciberespacio y activos críticos. |
| **Estándares comunes** | ISO/IEC 27005, NIST CSF 2.0. | ISO 31000, Marcos militares de ciberdefensa. |

---

## El Ciclo del Riesgo (Basado en ISO 31000 y NIST)

Para ambos mundos, el riesgo es una función del impacto y la probabilidad, expresado formalmente como:

$$Riesgo = Amenaza \times Vulnerabilidad \times Impacto$$

1.  **Contexto:** Definir qué leyes, reglamentos y objetivos rigen a la entidad.
2.  **Valoración:** Determinar qué tan grave sería perder el control de un sistema (ej. un sistema de control de reactores nucleares tiene un impacto extremo).
3.  **Monitoreo Continuo:** El riesgo en el ciberespacio no es estático; una nueva vulnerabilidad descubierta hoy (Zero-day) cambia el perfil de riesgo instantáneamente.
