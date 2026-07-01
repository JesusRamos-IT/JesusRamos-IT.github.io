---
layout: default
title: "📊 Cuadro de Mando: Evaluación de la Declaración de Aplicabilidad (SoA)"
---

# 📊 Cuadro de Mando: Evaluación de la Declaración de Aplicabilidad (SoA)

En el marco de una auditoría ISO 27001:2022, la **Declaración de Aplicabilidad (SoA)** es el documento central que define el alcance operativo del SGSI. Este cuadro de mando actúa como guía de referencia analítica para evaluar la integridad, consistencia y validez técnica del SoA presentado por la organización auditada.

---

## 🔍 Criterios de Auditoría para el SoA (Requisitos Cláusula 6.1.3)

Al evaluar el SoA de una organización, se deben verificar de forma obligatoria los siguientes puntos de control antes de entrar en la fase técnica:

1. **Integridad:** Comprobar que los **93 controles** del Anexo A han sido considerados y explícitamente enumerados (ninguno puede quedar en el olvido).
2. **Justificación de Inclusión:** Verificar que se detalla claramente por qué los controles seleccionados son necesarios y el estado actual de su implementación.
3. **Justificación de Exclusión:** Validar que cualquier control marcado como "No Aplicable" cuenta con una justificación técnica o de negocio real, documentada y coherente con el alcance del SGSI.

---

## 🛡️ Matriz de Referencia Especializada (Estructura de los 93 Controles)

Esta matriz organiza los 93 controles del Anexo A de la versión 2022 en sus 4 grandes bloques temáticos. Utiliza este mapa para dirigir la revisión hacia las guías de evidencias de tu framework:

| Bloque Normativo | Nº Controles | Foco de la Auditoría (¿Qué evidencias buscar?) | Estado del Toolkit | Enlace a la Guía |
| :--- | :---: | :--- | :---: | :--- |
| **A.5 Controles Organizativos** | 37 | Políticas de seguridad, gestión de activos, control de accesos corporativo, relaciones con proveedores, gestión de incidentes y continuidad de negocio. | 🟢 Operativo | [Módulo 5](./02-Criterios-Anexo-A/5-Organizativos/) |
| **A.6 Controles de Personas** | 8 | Ciclo de vida del personal (antes, durante y tras el cese), acuerdos de confidencialidad, directrices de teletrabajo y planes de concienciación. | 🟢 Operativo | [Módulo 6](./02-Criterios-Anexo-A/6-Personas/) |
| **A.7 Controles Físicos** | 14 | Perímetros de seguridad, barreras físicas, protección contra amenazas ambientales, seguridad en oficinas, instalaciones y soportes de almacenamiento. | 🟢 Operativo | [Módulo 7](./02-Criterios-Anexo-A/7-Fisicos/) |
| **A.8 Controles Tecnológicos** | 34 | Autenticación, gestión de privilegios, cifrado, copias de seguridad, monitorización de sistemas, gestión de vulnerabilidades y desarrollo seguro. | 🟢 Operativo | [Módulo 8](./02-Criterios-Anexo-A/8-Tecnologicos/) |

---

## ⚖️ Guía de Validación de Exclusiones Comunes

De cara a una auditoría del SGSI, la defensa de una exclusión debe ser rigurosa. Te detallo un ejemplo de justificación válida, frente a un argumento no válido, durante la fase de campo:

* **Controles de Desarrollo Seguro (A.8.25 a A.8.34):**
  * *Válido:* "La organización no realiza desarrollo propio ni modificaciones de software; opera exclusivamente con soluciones SaaS comerciales bajo acuerdos de nivel de servicio (SLA)."
  * *No Válido:* "No los aplicamos porque subcontratamos a una empresa externa para programar la web de la empresa, pero no supervisamos su código." *(Si hay subcontratación de desarrollo, se deben aplicar los controles de supervisión de proveedores).*

---

## 🛠️ Herramientas de Campo de Auditoría
* [➕ Registrar hallazgo / No Conformidad (NC)](./03-Plantillas-y-Toolkits/Template-Registro-NC.md)
* [📝 Redactar Informe Final de Auditoría](./03-Plantillas-y-Toolkits/Template-Informe-Auditoria.md)
