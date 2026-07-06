---
layout: default
title: "💻 Módulo 8: Controles Tecnológicos"
parent: "02. Criterios Anexo A"
---

# 💻 Módulo 8: Controles Tecnológicos

Este módulo contiene las guías de revisión, objetivos de auditoría y criterios de evaluación para los **34 controles tecnológicos** definidos en el Anexo A de la ISO 27001:2022. 

El foco principal de este bloque es verificar la correcta implementación técnica de las salvaguardas digitales.

---

## 📋 Guías de Verificación Disponibles

A continuación se listan los procedimientos de auditoría y checklists documentados en el toolkit:

| Control / Documento | Enfoque de Auditoría (¿Qué busco?) |
| :--- | :--- |
| [**8.1 - Dispositivos de usuario final**](./8.1-Acceso-Redes-No-Corporativas.md) | Verificación de requisitos de seguridad en dispositivos de acceso externo. |
| [**8.2 - Derechos de acceso**](./8.2-Acceso-Control-Informacion.md) | Control de privilegios elevados y segregación de funciones. |
| [**8.5 - Gestión de información de autenticación**](./8.5-Contrasenas.md) | Validación de contraseñas robustas y despliegue de MFA. |
| [**8.7 - Protección contra malware**](./8.7-Antimalware.md) | Comprobación de despliegue de EDR/antimalware y alertas centrales. |
| [**8.10 - Borrado de información**](./8.10-Borrado-Seguro.md) | Revisión de métodos de eliminación irreversible de datos. |
| [**8.11 - Gestión de comunicaciones**](./8.11-Correo-Electronico.md) | Auditoría de seguridad en pasarelas de correo y cifrado. |
| [**8.12 - Prevención de fuga de datos**](./8.12-Almacenamiento-Red-Corporativa.md) | Evaluación de reglas DLP y permisos en servidores de ficheros. |
| [**8.13 - Copias de seguridad**](./8.13-Sistema-Copias-Seguridad.md) | Verificación de regla 3-2-1, inmutabilidad y tests de restauración. |
| [**8.15 - Registro de eventos**](./8.15-Gestion-Logs.md) | Inspección de centralización de logs (SIEM) y sincronización NTP. |
| [**8.19 - Gestión de vulnerabilidades técnicas**](./8.19-Actualizacion-Software.md) | Ciclo de vida de parches y escaneos de vulnerabilidades. |
| [**8.19 - Control de software**](./8.19-Aplicaciones-Permitidas.md) | Restricción de software (whitelisting/AppLocker). |
| [**8.22 - Seguridad servicios web**](./8.22-Pagina-Web.md) | Filtrado web y protección de portales corporativos. |
| [**8.23 - Seguridad servicios en la nube**](./8.32-Almacenamiento-Nube.md) | Hardening y gobierno en entornos Cloud (SaaS/PaaS/IaaS). |
| [**8.24 - Uso de criptografía**](./8.24-Tecnicas-Criptograficas.md) | Gestión de claves y algoritmos de cifrado fuertes. |
| [**8.28 - Auditoría técnica**](./8.28-Auditorias-Sistema.md) | Planificación y autorización de pruebas técnicas. |

---
> **Nota del Auditor:** En la revisión de los controles tecnológicos, la evidencia puramente documental es insuficiente. Como Auditor Líder, se deben solicitar muestras técnicas en tiempo real (GPOs, logs, informes de restauración).

---

## 🗺️ Navegación Rápida

* 🛡️ [Volver al Índice del Anexo A (Controles)](../)
* 📈 [Ir al Cuadro de Mando: Dashboard SoA](../../Dashboard-SoA.md)
