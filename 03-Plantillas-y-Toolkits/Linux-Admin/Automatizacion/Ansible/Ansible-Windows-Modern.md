---
layout: default
title: "🤖 Automatización: Ansible & Windows"
subtitle: "Gestión de infraestructura mediante OpenSSH y Win_Updates"
---

# Gestión Automatizada de Windows Server con Ansible

Este documento define el estándar de configuración para la gestión de servidores Windows (incluidos Controladores de Dominio) utilizando **Ansible** sobre el protocolo **SSH**, evitando el uso del legado WinRM.

## 🏗️ Arquitectura de Conexión
La comunicación se establece desde un nodo de control (Ubuntu Server) hacia los nodos gestionados (Windows Server 2016/2019/2022) mediante **OpenSSH for Windows**.

### Requisitos del Nodo Gestionado
* **Servicio:** OpenSSH Server habilitado y en ejecución.
* **Autenticación:** Basada en clave pública (ED25519) para evitar el tráfico de credenciales en texto claro.
* **Shell por defecto:** PowerShell.

## 🔑 Configuración de Seguridad
Para garantizar el acceso administrativo, se utiliza la gestión de llaves en la ruta de administración del sistema:
* **Ruta de llaves:** `%ProgramData%\ssh\administrators_authorized_keys`
* **Permisos:** Restringidos exclusivamente al grupo `Administradores` y al sistema `SYSTEM`.

## 📂 Definición de Inventario (Hosts)
Para asegurar la resolución de nombres y la conexión correcta, se recomienda el uso de **UPN (User Principal Name)** en el archivo de inventario:

```ini
[windows_servers]
win-dc-01 ansible_host=192.168.200.200 ansible_user=ansible@dominio.local ansible_ssh_private_key_file=/root/.ssh/id_ed25519_ansible
```
## 🔄 Gestión de Actualizaciones (WUfB)

La automatización de parches en entornos de Controlador de Dominio se realiza mediante el módulo ansible.windows.win_updates.

| Parámetro | Valor Recomendado | Motivo |
| :--- | :--- | :--- |
| category_names |"SecurityUpdates, CriticalUpdates" | Estabilidad del sistema |
| reboot | yes | Garantiza la aplicación del parche |
|reboot_timeout | 3600 | Margen para cierre de servicios de AD |

🛠️ Comandos de Verificación (Health Check)

Ejecución de validación de conectividad desde el nodo de control:

ansible windows_servers -m win_ping

---

🧪 Recursos Adicionales

   🚀 [Ver laboratorio paso a paso](./Labs/Manual-Ansible-Windows-Detallado.md)

---
⬅️ Navegación:
   * [Volver a Automatización](../index.md)
   * [Volver al Inicio](../../index.md)


