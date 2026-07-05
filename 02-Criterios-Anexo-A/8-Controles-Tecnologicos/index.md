---
layout: default
title: "💻 Módulo 8: Controles Tecnológicos"
parent: "02. Criterios Anexo A"
---

# 💻 Módulo 8: Controles Tecnológicos

Este módulo contiene las guías de revisión, objetivos de auditoría y criterios de evaluación para los **34 controles tecnológicos** definidos en el Anexo A de la ISO 27001:2022. 

El foco principal de este bloque es verificar la correcta implementación técnica de las salvaguardas digitales, garantizando la seguridad en las redes, la protección de los endpoints, la gestión de accesos técnicos, el cifrado de datos y la integridad operativa de los sistemas de información de la organización.

---

## 📋 Guías de Verificación Disponibles

A continuación se listan los procedimientos de auditoría y checklists documentados en el toolkit:

| Control / Documento | Enfoque de Auditoría (¿Qué busco?) |
| :--- | :--- |
| [**8.1 - Dispositivos de usuario final (Acceso desde Redes No Corporativas)**](./8.1-Acceso-Redes-No-Corporativas.md) | Verificación de que los dispositivos que acceden desde redes externas cumplen con los requisitos de seguridad (parches, AV, firewall local) previos a la conexión y uso de recursos. |
| [**8.2 - Derechos de acceso privilegiados (Control de Acceso a la Información)**](./8.2-Acceso-Control-Informacion.md) | Inspección de la asignación y revocación de cuentas con privilegios elevados (admin, root). Control de la segregación de funciones y cumplimiento estricto del principio de mínimo privilegio. |
| [**8.5 - Autenticación segura (Gestión de Contraseñas)**](./8.5-Contrasenas.md) | Validación de políticas robustas de contraseñas de forma centralizada (complejidad, longitud, rotación) y la obligatoriedad del Doble Factor de Autenticación (MFA) en accesos críticos. |
| [**8.7 - Protección contra malware (Antimalware)**](./8.7-Antimalware.md) | Comprobación del despliegue del agente EDR/antimalware en la totalidad de la infraestructura, asegurando la actualización automática de firmas y el correcto envío de alertas al panel central. |
| [**8.10 - Borrado de información (Borrado Seguro)**](./8.10-Borrado-Seguro.md) | Revisión de las herramientas y métodos de desmagnetización, sobreescritura o destrucción física utilizados para la eliminación irreversible de datos en soportes de almacenamiento obsoletos. |
| [**8.11 - Enmascaramiento e intercambio de información (Correo Electrónico)**](./8.11-Correo-Electronico.md) | Auditoría de los mecanismos de seguridad en pasarelas de correo (antispam, SPF/DKIM/DMARC) y protocolos seguros o herramientas de cifrado para el intercambio de archivos sensibles. |
| [**8.12 - Prevención de fuga de datos (Almacenamiento en Red Corporativa)**](./8.12-Almacenamiento-Red-Corporativa.md) | Evaluación de los controles técnicos (reglas DLP, permisos NTFS/ACLs en servidores de ficheros) para monitorizar, restringir y alertar ante intentos de exfiltración o accesos no autorizados. |
| [**8.13 - Copias de seguridad (Sistema de Copias de Seguridad)**](./8.13-Sistema-Copias-Seguridad.md) | Verificación técnica de la regla 3-2-1 de backups, la inmutabilidad de las copias, el cifrado del almacenamiento de destino y, críticamente, los registros de los tests de restauración periódicos. |
| [**8.15 - Registro de eventos (Gestión de Logs)**](./8.15-Gestion-Logs.md) | Inspección de la centralización de registros (SIEM/Syslog), protección frente a modificaciones no autorizadas, políticas de retención temporal y sincronización horaria mediante NTP fiable. |
| [**8.19 - Gestión de vulnerabilidades técnicas (Actualización de Software)**](./8.19-Actualizacion-Software.md) | Evaluación del ciclo de vida de parches (Patch Management) en sistemas operativos y aplicaciones del alcance, analizando los informes de escaneos de vulnerabilidades recientes. |
| [**8.19 - Instalación de software en sistemas operativos (Aplicaciones Permitidas)**](./8.19-Aplicaciones-Permitidas.md) | Control de los mecanismos de restricción de software (AppLocker, políticas de grupo o eliminación de privilegios locales de administrador) para evitar la instalación de software no corporativo. |
| [**8.22 - Filtrado web (Restricciones de Acceso a Páginas Web)**](./8.22-Pagina-Web.md) | Verificación de políticas perimetrales o de endpoint para el bloqueo automático de categorías web maliciosas, de alto riesgo (phishing, malware) o contrarias a la política de uso aceptable. |
| [**8.24 - Uso de criptografía (Técnicas Criptográficas)**](./8.24-Tecnicas-Criptograficas.md) | Comprobación de que el cifrado de datos (en tránsito mediante TLS 1.3/SSH y en reposo) hace uso de algoritmos fuertes y validados, revisando la correcta gestión y custodia del ciclo de vida de las claves. |
| [**8.28 - Seguridad en las actividades de auditoría (Auditorías de Sistema)**](./8.28-Auditorias-Sistema.md) | Verificación de que las pruebas técnicas invasivas (pentesting, escaneos de red masivos) están planificadas y autorizadas para mitigar riesgos de denegación de servicio o indisponibilidad. |
| [**8.32 - Seguridad en el uso de servicios en la nube (Almacenamiento en la Nube)**](./8.32-Almacenamiento-Nube.md) | Evaluación del aprovisionamiento técnico, hardening de accesos y directivas de seguridad aplicadas sobre entornos Cloud corporativos (SaaS, PaaS, IaaS) e instancias de almacenamiento compartido. |

---
> **Nota del Auditor:** En la revisión de los controles tecnológicos, la evidencia puramente documental (como una política escrita) es insuficiente. Como Auditor Líder, se deben solicitar muestras técnicas en tiempo real durante el muestreo: configuraciones activas de directivas de grupo (GPOs) para el control de contraseñas (8.5), políticas de retención y alertas en el concentrador de logs (8.15) o los informes del último test de restauración de backups (8.13) para comprobar que las copias son realmente funcionales.

---

## 🗺️ Navegación Rápida

* 🛡️ [Volver al Índice del Anexo A (Controles)](../)
* 📈 [Ir al Cuadro de Mando: Dashboard SoA](../../Dashboard-SoA.md)
