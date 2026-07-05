---
layout: default
title: "[ID_CONTROL] - [Nombre del Control]"
---

# 💻 [ID_CONTROL]: [Nombre del Control según ISO 27002:2022]

> **Etiqueta ISO:** #Protección #Detección | **Dominio:** [Físico / Tecnológico]

## 👤 Perfil del Control
| Campo | Detalle |
| :--- | :--- |
| **Responsable (Owner):** | [Rol o persona que responde por este control] |
| **Estado:** | [Implementado / En proceso / Planificado] |
| **Vinculación a Riesgo:** | [Referencia a qué riesgo mitiga este control] |

---

## 1. 🎯 Propósito del Control
*Define el objetivo de la medida técnica para salvaguardar la Confidencialidad, Integridad y Disponibilidad (CID).*
**Ejemplo:** Detectar, registrar y alertar sobre eventos anómalos o fallos de acceso en la infraestructura crítica.

---

## 2. 🛡️ Evidencias Objetivas (¿Qué auditar en el sistema?)
*Listado de configuraciones, logs o plataformas a inspeccionar.*
* [ ] **Configuración Segura (Baseline):** Directivas de grupo (GPOs) o scripts de automatización aplicados.
* [ ] **Trazabilidad:** Logs de auditoría, dashboards de monitorización (SIEM) o alertas configuradas.
* [ ] **Pruebas de Eficacia:** Resultados de escaneos de vulnerabilidades o tests de restauración (Backups).

---

## 3. ⚙️ Puntos de Verificación (Checklist de Auditoría Técnica)
*Preguntas para validar la implementación real frente al papel.*
1. ¿El control técnico está desplegado en todos los activos dentro del alcance, sin excepciones no documentadas?
2. ¿Las configuraciones están centralizadas y protegidas contra modificaciones no autorizadas?
3. ¿Existe sincronización de reloj (NTP) fiable para garantizar la validez legal de los registros?
4. ¿Las alertas de seguridad llegan a un responsable definido que pueda actuar a tiempo?

---

## 4. ⚖️ Matriz de Criterio (Hallazgos y NC)

| Estado Encontrado | Clasificación | Acción Correctiva Esperada |
| :--- | :---: | :--- |
| **Sistemas críticos expuestos**, sin protección perimetral, o ausencia total de recolección de eventos. | 🚨 **NC Mayor** | Aislamiento, despliegue urgente del agente/control y análisis de impacto. |
| El control está automatizado y centralizado, pero un nodo recién desplegado **no heredó la política** correctamente. | ⚠️ **NC Menor** | Corrección del nodo y ajuste en la plantilla de despliegue. |
| Las alertas funcionan, pero los umbrales generan falsos positivos que causan fatiga de alertas. | 💡 **Observación (OFI)** | Afinar las reglas de correlación del SIEM. |

---

## 🗺️ Navegación Rápida
* 📁 [Volver al Centro de Plantillas y Toolkits](./index.md)
* 📈 [Ir al Cuadro de Mando: Dashboard SoA](../Dashboard-SoA.md)
