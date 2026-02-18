# Practica-de-Github-Pages
Práctica de Github Pages

# 🏥 ClinicaDevF — Landing Page

> Landing page profesional para ClinicaDevF, una clínica médica integral. Construida en HTML, CSS y JavaScript puro, sin dependencias ni frameworks.

---

## 📋 Descripción

**ClinicaDevF** es una landing page estática de una sola página diseñada para presentar los servicios, el equipo médico y la información de contacto de la clínica. Cuenta con un diseño elegante con paleta de colores verde bosque y dorado, tipografía refinada y animaciones suaves.

---

## 🗂️ Estructura del Proyecto

```
clinicadevf/
└── clinicadevf.html     # Archivo principal (todo en un solo archivo)
```

El proyecto es un archivo HTML autocontenido que incluye:
- **CSS** embebido en `<style>`
- **JavaScript** embebido en `<script>`
- **Fuentes** cargadas desde Google Fonts (requiere conexión a internet)

---

## 🚀 Cómo usar

### Opción 1 — Abrir directamente
Descarga el archivo `clinicadevf.html` y ábrelo en cualquier navegador moderno:
```bash
# Mac
open clinicadevf.html

# Linux
xdg-open clinicadevf.html

# Windows
start clinicadevf.html
```

### Opción 2 — Servidor local
```bash
# Con Python
python -m http.server 8000

# Con Node.js (npx)
npx serve .
```
Luego abre `http://localhost:8000/clinicadevf.html` en tu navegador.

---

## 📦 Tecnologías

| Tecnología | Uso |
|---|---|
| HTML5 semántico | Estructura de la página |
| CSS3 (Variables, Grid, Flexbox) | Diseño y layout |
| CSS Animations & Keyframes | Animaciones y transiciones |
| JavaScript Vanilla | Interactividad y scroll |
| Google Fonts | Tipografías (Playfair Display + DM Sans) |
| Intersection Observer API | Fade-in al hacer scroll |

---

## 🎨 Diseño

### Paleta de Colores

| Variable | Hex | Uso |
|---|---|---|
| `--cream` | `#F7F4EF` | Fondo principal |
| `--forest` | `#2C4A3E` | Color primario (botones, nav) |
| `--sage` | `#7AAF9A` | Acentos secundarios |
| `--gold` | `#C8A96E` | Destacados y hover |
| `--dark` | `#1A2E28` | Fondo oscuro (sección about) |

### Tipografía
- **Display / Títulos:** Playfair Display (serif elegante)
- **Cuerpo / UI:** DM Sans (sans-serif limpio)

---

## 🧩 Secciones

| Sección | ID | Descripción |
|---|---|---|
| Navegación | — | Barra fija con blur y links de anclaje |
| Hero | `#inicio` | Título principal, CTA y tarjeta animada con estadísticas |
| Servicios | `#servicios` | Grid de 6 especialidades médicas |
| Nosotros | `#nosotros` | Métricas de la clínica sobre fondo oscuro |
| Equipo | `#equipo` | 4 doctores con avatares |
| Testimonios | — | 3 reseñas de pacientes |
| Contacto | `#contacto` | Información + formulario de cita |
| Footer | — | Links, legal y copyright |

---

## ⚙️ Funcionalidades

- **Navegación fija** con efecto de transparencia y blur
- **Blob animado** en el hero con morfología CSS
- **Fade-in con scroll** usando `IntersectionObserver`
- **Formulario interactivo** con confirmación visual al enviar
- **Diseño responsive** adaptado a móvil, tablet y escritorio
- **Hover states** en cards, botones y links

---

## 📱 Responsive

| Breakpoint | Comportamiento |
|---|---|
| `> 900px` | Layout de 2 columnas en hero, about y contacto |
| `≤ 900px` | Layout de 1 columna, nav links ocultos |
| `≤ 600px` | Formulario apilado, footer en 1 columna |

---

## ✏️ Personalización

### Cambiar información de contacto
Busca en el HTML la sección `#contacto` y edita los datos:
```html
<span>Av. Salud 1234, Col. Centro, CDMX</span>
<span>+52 (55) 1234 5678</span>
<span>citas@clinicadevf.com</span>
```

### Cambiar colores
Modifica las variables CSS en `:root`:
```css
:root {
  --forest: #2C4A3E;  /* Color primario */
  --gold:   #C8A96E;  /* Color acento   */
  --cream:  #F7F4EF;  /* Fondo          */
}
```

### Agregar una especialidad
Duplica un bloque `.service-card` dentro del grid de servicios y actualiza el emoji, título y descripción.

---

## 📄 Licencia

Este proyecto fue creado como página de presentación para **ClinicaDevF**. Todos los derechos reservados © 2026 ClinicaDevF.

---

> Hecho con ❤️ para la salud de nuestros pacientes.