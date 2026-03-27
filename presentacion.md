# Documentación Técnica: Tarjeta de Presentación Digital

Este documento describe las decisiones tomadas durante el desarrollo del archivo `proyecto_final_clase.html`. El propósito es explicar la estructura utilizada en la página y el uso de etiquetas semánticas siguiendo los estándares de **HTML5**.

---

## 1. Uso de Etiquetas Semánticas (Explicación)

Para construir la página se utilizaron etiquetas semánticas de HTML5. Estas permiten que el contenido tenga una estructura más clara, facilitan la comprensión del documento por parte de los navegadores y herramientas de accesibilidad, y ayudan a mantener el código organizado.

- **`<header>`**: Se usa para mostrar la parte inicial del documento. Allí se encuentra el nombre del autor y una frase o eslogan que identifica la página.

- **`<main>`**: Representa el contenido principal del documento. Dentro de este elemento se ubica la información más importante, separándola de otras secciones como el encabezado o el pie de página.

- **`<section>`**: Permite dividir el contenido en diferentes bloques temáticos. En este proyecto se usa para separar la sección de información personal de la sección de habilidades y pasatiempos.

- **`<time>`**: Esta etiqueta se utiliza para representar fechas de forma estructurada mediante el atributo `datetime`, lo que facilita que tanto los usuarios como los sistemas puedan interpretar correctamente la información.

- **`<strong>` y `<em>`**: Se emplean para destacar partes del texto. `<strong>` resalta conceptos importantes mientras que `<em>` se utiliza para dar énfasis a ciertas frases.

- **`<address>`**: Se utiliza para presentar la información de contacto del autor del documento, como el correo electrónico y la ubicación.

---

## 2. Estructura del Documento (Árbol DOM)

La siguiente representación muestra la organización jerárquica de los elementos dentro del archivo HTML, permitiendo entender cómo está estructurada la página.

```text
Documento HTML
└── head (Metadatos y estilos)
└── body
    ├── header
    │   ├── h1 (Nombre del autor)
    │   └── p > em (Frase o eslogan)
    ├── main
    │   ├── section (Información personal)
    │   │   ├── h2
    │   │   └── p (incluye strong y time)
    │   └── section (Habilidades y pasatiempos)
    │       ├── h2
    │       ├── h3
    │       ├── ul > li (lista de habilidades)
    │       └── p (pasatiempos con strong)
    └── footer
        └── address (datos de contacto)
            └── small (derechos de autor)