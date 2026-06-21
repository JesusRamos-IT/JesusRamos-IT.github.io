---
layout: default
title: "🔄 Windows Update for Business (WUfB)"
subtitle: "Gestión de parches vía GPO sin infraestructura WSUS"
---

# Gestión de Actualizaciones Cloud-Direct

Este estándar técnico define la configuración de directivas de grupo (GPO) para permitir que los endpoints de la infraestructura gestionen sus actualizaciones directamente desde los servidores de Microsoft, eliminando la necesidad de un servidor WSUS local y optimizando el consumo de recursos internos.

## ⚙️ Configuración de la Directiva Principal
La configuración se aplica a nivel de equipo en la siguiente ruta:
`Configuración del equipo > Plantillas administrativas > Componentes de Windows > Windows Update`

### 1. Directivas de Actualización Automática
* **Configuración de actualizaciones automáticas:** Habilitada (Opción 4 - Descargar automáticamente e instalar según programación).
* **Instalación inmediata:** Habilitada para actualizaciones que no interrumpan servicios críticos.
* **Actualizaciones recomendadas:** Incluidas en el ciclo de actualizaciones automáticas.

### 2. Directivas de Aplazamiento (Deferral Policies)
Para garantizar la estabilidad antes del despliegue masivo, se establecen los siguientes periodos de gracia:
* **Actualizaciones de calidad:** Aplazamiento de **30 días** (parches de seguridad y críticos).
* **Actualizaciones de características:** Aplazamiento según la rama de mantenimiento (General Availability Channel).

## ⚠️ Puntos Críticos de Verificación (Anti-Conflictos)
Para que el servicio WUfB funcione correctamente sin WSUS, es imperativo validar:

* **Servicio de Intranet:** La directiva *"Especificar la ubicación del servicio Microsoft Update en la intranet"* debe estar **No configurada**. Cualquier valor aquí forzará al cliente a buscar un servidor local inexistente.
* **Dual Scan:** Al configurar aplazamientos, el cliente activa el escaneo dual. Se debe asegurar que no existan políticas heredadas que apunten a servidores de actualización internos.

## 📊 Monitorización y Cumplimiento
El estado de la aplicación de estas políticas puede verificarse localmente mediante el comando:

```powershell
# Verificación de políticas aplicadas en el registro
Get-ItemProperty -Path "HKLM:\SOFTWARE\Policies\Microsoft\Windows\WindowsUpdate\AU"
```

---

🧪 Recursos Adicionales

   * 🚀 [Ver Laboratorio Paso a Paso (Modo Lab)](./Labs/Manual-GPO-Updates-Detallado.md)

---

⬅️ Navegación

[Volver a Windows Admin](../index.md)

[Volver al Índice de Playbooks](../../index.md)
