# Contexto del Proyecto - Portfolio de Jesús Castilla

Este archivo contiene el contexto necesario para agentes de Inteligencia Artificial que deban retomar, modificar o ampliar el trabajo en el portfolio de Jesús Castilla. 

---

## Propósito del Proyecto

El objetivo de este proyecto es servir como un portfolio / currículum vitae web formal para Jesús Castilla, documentando su perfil como **Desarrollador de Software**. 

**Premisa crítica:**
Queda explícitamente reflejado en la web que la programación es un **hobby y una vocación**. Todos los proyectos presentados se han desarrollado sin ánimo de lucro y no reportan ingresos económicos.

---

## Arquitectura y Tecnologías

- **Tipo de proyecto:** Web estática clásica (HTML5, CSS3, Vanilla JS si fuera necesario).
- **Enfoque técnico:** Sin frameworks (cero dependencias, ni npm, ni compilación). Diseñado para máxima simplicidad, compatibilidad y facilidad de despliegue.
- **Estilos (`styles.css`):**
  - Estilo formal, sobrio y profesional, alineado con la identidad de Lebeche.
  - Paleta: papel crema (`#F5F5F0`), tinta (`#141414`), acentos azul marino (`#041E2B`) y ámbar (`#E8A33D`). Tipografías Inter (cuerpo) y Playfair Display (títulos).
  - Diseño totalmente *responsive* (Grid y Flexbox).

---

## Estructura de Archivos

```text
Portfolio-Pelotxo/
├── index.html        # Página principal: Declaración de intenciones, listado de lenguajes y proyectos
├── contacto.html     # Página secundaria: Enlaces profesionales (LinkedIn, WhatsApp, GitHub) y formulario
├── styles.css        # Hoja de estilos global
└── CONTEXT.md        # Documentación para IA (este archivo)
```

---

## Detalles del Contenido

### 1. `index.html` (Proyectos)
La página se divide semánticamente por **Lenguajes y Tecnologías**, basándose en el historial real del desarrollador:
- **Kotlin & Android Development:** App Barrioteca v2, Calendario Lebeche.
- **TypeScript, React & Frontend Web:** Frontend Web/PWA de Barrioteca, Lebeche Web Oficial.
- **Swift & iOS:** App wrapper nativo de iOS para Barrioteca.
- **PHP & Bases de Datos:** Backend SLiMS de Barrioteca.
- **Sistemas, Shell Scripting y Linux:** Creación del sistema operativo DiplodocOS, configuración de Nginx en Synology.

### 2. `contacto.html` (Contacto y Enlaces)
Se incluyen enlaces y vías de contacto directos:
- **LinkedIn:** [https://www.linkedin.com/in/jesuscastillalacal](https://www.linkedin.com/in/jesuscastillalacal)
- **GitHub:** [https://github.com/jesuscastilla](https://github.com/jesuscastilla)
- **WhatsApp (DiploTech):** `+34687407347` (Enlace directo vía `wa.me`)
- Un **formulario de contacto** maquetado (actualmente sin backend configurado, usa `action="#"`).

---

## Despliegue en el NAS (Instrucciones)

Este proyecto está diseñado para alojarse en el NAS Synology de Jesús (`pelotxo.synology.me`), utilizando **Web Station** (Nginx/Apache). El dominio dedicado es `corrientelebeche.es` (ver `LEBECHE/docs/GUIA_DOMINIO_CORRIENTELEBECHE.md`).

### Pasos de despliegue local manual (Red interna)
1. Acceder al NAS a través de la red local mediante SMB: `\\192.168.50.94\web\` (o la ruta correspondiente al volumen web).
2. Crear la carpeta `/Portfolio/` (o copiar la carpeta `Portfolio-Pelotxo` entera) dentro de la carpeta compartida web.
3. Copiar el contenido (`index.html`, `contacto.html`, `styles.css`) en dicha carpeta.
4. El servidor Web Station servirá directamente el contenido HTML a través de la IP local o del dominio en el subdirectorio correspondiente (p.ej. `https://www.corrientelebeche.es/portfolio/`).

---

## Directrices para futuros cambios

1. **No mencionar a la IA:** Ningún texto visible en los archivos HTML o en la consola debe hacer referencia a que fue generado, sugerido o creado por Inteligencia Artificial.
2. **Mantener la formalidad:** El tono del texto debe ser siempre profesional, directo y formal.
3. **No alterar la declaración de Hobby:** El descargo de responsabilidad indicando que el trabajo de desarrollo de software no es comercial debe mantenerse prominentemente en la página principal.

