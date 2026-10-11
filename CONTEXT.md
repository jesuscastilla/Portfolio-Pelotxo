# Contexto del Proyecto - Portfolio de Jesús Castilla

Este archivo contiene el contexto técnico necesario para retomar, modificar o ampliar el trabajo en el portfolio de Jesús Castilla sin pérdida de información.

---

## Propósito del Proyecto

El objetivo de este proyecto es servir como un portfolio / currículum vitae web formal para Jesús Castilla, documentando su perfil como **Desarrollador de Software**. 

**Premisa (2026-10-11):** el portfolio se reposiciona como **CV profesional** orientado a LinkedIn. Tono formal y enfoque en productos reales en producción. La marca personal es **DiploTech**.

---

## Arquitectura y Tecnologías

- **Tipo de proyecto:** Web estática clásica (HTML5, CSS3, Vanilla JS). Sin frameworks, sin npm, sin build step.
- **Enfoque técnico:** Máxima simplicidad, compatibilidad y facilidad de despliegue (GitHub Pages + NAS Synology).
- **Identidad (2026-10-11):** rediseño profesional como CV para LinkedIn, con branding **DiploTech**. Paleta: papel cálido (`#F7F5EF`), tinta verde‑negro (`#1A231A`) y verde de marca (`#5F9A4B`). Tipografías **Fraunces** (títulos) y **Manrope** (cuerpo). Logo en `assets/` (transparente + versión blanca).

---

## Estructura de Archivos

```text
portfolio-pelotxo/
├── index.html        # Inicio (ES): héroe, sobre mí, stack, proyectos, CTA de contacto
├── index-en.html     # Inicio (EN)
├── contacto.html     # Contacto (ES): enlaces + formulario
├── contacto-en.html  # Contacto (EN)
├── styles.css        # Hoja de estilos global (rediseño 2026)
├── assets/           # Logo DiploTech, favicon y apple-touch-icon
└── CONTEXT.md        # Documentación técnica (este archivo)
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
2. Crear la carpeta `/Portfolio/` (o copiar la carpeta `portfolio-pelotxo` entera) dentro de la carpeta compartida web.
3. Copiar el contenido (`index.html`, `contacto.html`, `styles.css`) en dicha carpeta.
4. El servidor Web Station servirá directamente el contenido HTML a través de la IP local o del dominio en el subdirectorio correspondiente (p.ej. `https://www.corrientelebeche.es/portfolio/`).

---

## Directrices para futuros cambios

1. **Mantener la formalidad:** El tono del texto debe ser siempre profesional, directo y formal.
2. **Tono profesional:** el texto debe reflejar un perfil profesional de desarrollador (sin el antiguo descargo de «hobby no comercial»), manteniendo la autenticidad.

