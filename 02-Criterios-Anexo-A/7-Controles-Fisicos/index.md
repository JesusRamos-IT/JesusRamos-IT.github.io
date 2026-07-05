---
layout: default
title: "🏢 Módulo 7: Controles Físicos"
parent: "02. Criterios Anexo A"
---

# 🏢 Módulo 7: Controles Físicos

Este módulo agrupa las guías de revisión, objetivos de auditoría y criterios de evaluación para los **14 controles físicos** definidos en el Anexo A de la ISO 27001:2022. 

El foco principal de este bloque es verificar la protección de las instalaciones de la organización, el perímetro de seguridad, el equipamiento de hardware y la custodia segura de los soportes de almacenamiento y dispositivos portátiles frente a accesos no autorizados, daños o interferencias.

---

## 📋 Guías de Verificación Disponibles

A continuación se listan los procedimientos de auditoría y checklists documentados en el toolkit:

| Control / Documento | Enfoque de Auditoría (¿Qué busco?) |
| :--- | :--- |
| [**7.7 - Escritorio despejado y pantalla limpia**](./7.7-Proteccion-Puesto-Trabajo.md) | Inspección del cumplimiento operativo de la política de mesa limpia y bloqueo automático de pantalla. Verificación visual para detectar contraseñas en post-its, documentos confidenciales expuestos o sesiones desatendidas. |
| [**7.10 - Soportes de almacenamiento: Dispositivos externos**](./7.10-Almacenamiento-Dispositivos.md) | Evaluación del control del ciclo de vida de medios extraíbles (USB, discos externos). Revisión de políticas de cifrado forzoso, inventario de soportes autorizados y procedimientos de destrucción física segura. |
| [**7.10 - Soportes de almacenamiento: Equipo local**](./7.10-Almacenamiento-Equipo-Local.md) | Verificación de las medidas de protección del almacenamiento persistente en servidores y estaciones de trabajo. Comprobación del cifrado de disco completo (BitLocker, LUKS) y restricciones físicas de acceso a la torre/rack. |
| [**7.13 - Mantenimiento y protección de equipos: Dispositivos Móviles Corporativos**](./7.13-Dispositivos-Moviles-Corporativos.md) | Supervisión técnica de portátiles y smartphones propiedad de la empresa. Revisión de políticas de inventario, directivas centralizadas en el MDM, cifrado de datos y capacidad de borrado remoto en caso de pérdida o robo. |
| [**7.13 - Mantenimiento y protección de equipos: Dispositivos Móviles No Corporativos**](./7.13-Dispositivos-Moviles-No-Corporativos.md) | Gestión del riesgo derivado del acceso a recursos corporativos desde terminales personales (BYOD). Verificación de acuerdos de uso, despliegue de contenedores seguros o agentes de cumplimiento previos a la conexión. |

---
> **Nota del Auditor:** La evaluación de los controles físicos (especialmente el 7.7) requiere obligatoriamente observación directa. Durante la auditoría in situ (o la revisión por videollamada en entornos 100% remotos), se debe verificar visualmente si existen contraseñas apuntadas en post-its, documentación confidencial impresa sobre las mesas o equipos sin bloquear en ausencia del usuario.

---

## 🗺️ Navegación Rápida

* 🛡️ [Volver al Índice del Anexo A (Controles)](../)
* 📈 [Ir al Cuadro de Mando: Dashboard SoA](../../Dashboard-SoA.md)
