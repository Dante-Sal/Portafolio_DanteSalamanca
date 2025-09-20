# Mi Portafolio Web

Este repositorio contiene mi **sitio web de portafolio** (Simón Dante Salamanca Galvis).  
Este README **documenta el funcionamiento del sitio** (seguir la siguiente tabla para navegar por los contenidos):

| Tabla de contenidos                                                |
| ------------------------------------------------------------------ |
| [Vista general](#vista-general)                                    |
| [Ir al sitio](#ir-al-sitio)                                        |
| [Estructura del proyecto](#estructura-del-proyecto)                |
| [Secciones del sitio (index.html)](#secciones-del-sitio-indexhtml) |
| [Estilos y diseño](#estilos-y-dise%C3%B1o)                         |
| [Variables de color globales](#variables-de-color-globales)        |
| [Responsive](#responsive)                                          |
| [Licencia](#licencia)                                              |
| [Autor](#autor)                                                    |


## Vista general

- **Tipo de proyecto:** sitio estático (HTML + CSS).
- **Entrada principal:** `index.html`.  
- **Hojas de estilo:** `css/index.css` (estilos base) y `css/responsive.css`.  
- **Assets:** imágenes y PDF dentro de `./storage/`.

El sitio está pensado como **single-page** con navegación por anclas.

## Ir al sitio:

<a href="https://dante-sal.github.io/Portafolio_DanteSalamanca/">
   <img src="https://img.shields.io/badge/Portafolio-Web-blue?style=flat&logo=google-chrome" alt="Portfolio">
</a>

## Estructura del proyecto

```
.
├─ css/
│  ├─ index.css               # Estilos base y variables (paleta)
│  └─ responsive.css          # Reglas responsive (breakpoints)
├─ storage/
│   ├─ files/
│   |   └─ HV.DANTE.SALAMANCA.DESARROLLADORSOFTWARE.pdf  # Hoja de vida
│   ├─ img/
│   │  ├─ icons/               # Íconos (logo, redes, secciones)
│   │  ├─ projects/            # Thumbnails de proyectos
│   │  ├─ soft_skills/         # Íconos de habilidades blandas
│   │  ├─ technologies_abilities/  # Logos de tecnologías/habilidades
│   |  └─ banner.jpeg          # Imagen principal del banner
│   └─ files/
│      └─ HV.DANTE.SALAMANCA.DESARROLLADORSOFTWARE.pdf  # Hoja de vida
└─ index.html                 # Estructura y contenido de la página
```

## Secciones del sitio (index.html)

1. **Navbar (`.navbar`)**  
   - Logo (`./storage/img/icons/DSlogo.png`).  
   - Menú con anclas a cada sección: `#banner`, `#aboutme`, `#skills`, `#soft_skills`, `#projects`, `#professional_goals`, `#services`, `#mvv`, `#contacts`.

2. **Banner (`#banner`)**  
   - Fondo (`banner.jpeg`).
   - Botón interactivo para descargar la HV.
   - Texto principal y *slogan*.

3. **Sobre mí (`#aboutme`)**  
   - **YouTube embed**: `<iframe src="https://www.youtube.com/embed/...">`.  
   - Párrafo de presentación.

4. **Habilidades técnicas (`#skills`)**  
   - Tecnologías con logo + nombre.

5. **Habilidades blandas (`#soft_skills`)**  
   - Mismo patrón que técnicas, pero con íconos de habilidades blandas.

6. **Proyectos (`#projects`)**  
   - Tarjetas `.projects__card` con **imagen**, **título**, **stack (íconos de las tecnologías usadas)**, **descripción** y **botones** (Repo / Demo / README).

7. **Objetivos profesionales (`#professional_goals`)**  
   - Sección descriptiva con imagen ilustrativa.

8. **Servicios (`#services`)**  
   - Lista de servicios con subtítulos y descripciones.

9. **Misión, Visión y Valores (`#mvv`)**  
   - Cada apartado contiene ícono, título y texto descriptivo.

10. **Contacto (`#contacts`)**  
    - Nombre, email, teléfono y ubicación.  
    - Botones con enlaces a **GitHub** y **LinkedIn** (íconos en `./storage/img/icons/`).

## Estilos y diseño

### Variables de color globales
Definidas en `:root` (`css/index.css`):
```css
:root {
  --hex-light-emphasis: #d6d6d6;
  --hex-primary-emphasis: #ffee32;
  --hex-regular: #ffd100;
  --hex-dark: #202020;
  --hex-semidark: #333533;
  /* equivalentes RGB para transparencias con slash syntax */
  --rgb-light-emphasis: 214 214 214;
  --rgb-primary-emphasis: 255 238 50;
  --rgb-regular: 255 209 0;
  --rgb-dark: 32 32 32;
  --rgb-semidark: 51 53 51;
}
```

- El diseño usa **unidades relativas** (`vw`) para tamaños y márgenes en desktop.  
- El **banner** usa `background-attachment: fixed` en desktop y se desactiva en móviles por rendimiento.

### Responsive
Las reglas adaptativas están en `css/responsive.css` con *breakpoints* principales:
- `1200px`, `992px`, `768px` y `480px`  
Ajustan alturas, tamaños de fuente, espaciados y layout de tarjetas/proyectos.

## Licencia

Este sitio se distribuye para uso personal. Si se clona estructura o estilos a modo de plantilla, se agradece la atribución.

## Autor

**Simón Dante Salamanca Galvis**  
<p>
  <a href="mailto:dantesalamancagalvis@gmail.com">
    <img src="https://img.shields.io/badge/Email-DanteSalamanca-red?style=flat&logo=gmail&logoColor=white" alt="Email">
  </a>
  <a href="https://github.com/dante-sal/">
    <img src="https://img.shields.io/badge/GitHub-Dante_Sal-black?style=flat&logo=github" alt="GitHub">
  </a>
  <a href="https://www.linkedin.com/in/sim%C3%B3n-dante-salamanca-galvis-5370b2356/?profileId=ACoAAFilq3sBrRfMRLrRXmGbFXxmwU-fWU8LsGo">
    <img src="https://img.shields.io/badge/LinkedIn-Conecta-0A66C2" alt="LinkedIn">
  </a>
</p>
