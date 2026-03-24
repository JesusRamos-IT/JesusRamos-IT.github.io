---
layout: null
---
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="{{ '/assets/css/style.css' | relative_url }}">
    <title>ISO27001 Framework</title>
</head>
<body>
    <header class="main-header">
        <div class="header-overlay">
            <div class="header-content">
                <h1>🛡️ ISO27001 Framework</h1>
                <p class="tagline">Controles organizativos y tecnológicos</p>
                <a href="{{ '/' | relative_url }}" class="btn-github">⬅ Volver al Índice</a>
            </div>
        </div>
    </header>

    <main class="container">
        <article class="card">

{% capture my_markdown %}

# 📑 Framework de Controles ISO 27001:2022

Este directorio centraliza la documentación relativa a la gobernanza IT y los 29 anexos de seguridad.

---

## 🏛️ Módulos de Control
* **Módulo 1:** Controles Organizativos.
* **Módulo 2:** Controles de Personas.
* **Módulo 3:** Controles Físicos.
* **Módulo 4:** Controles Tecnológicos.

[Volver al Índice Principal]({{ '/' | relative_url }})

{% endcapture %}
{{ my_markdown | markdownify }}

        </article>
    </main>
</body>
</html>
