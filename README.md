# Frontend Mentor - Four card feature section solution

Esta es una solución al desafío [Four card feature section de Frontend Mentor](https://www.frontendmentor.io/challenges/four-card-feature-section-weK1eFYK). Los desafíos de Frontend Mentor te ayudan a mejorar tus habilidades en desarrollo frontend mediante la construcción de proyectos realistas.

## Tabla de contenidos

- [Visión general](#visión-general)
  - [El desafío](#el-desafío)
  - [Captura de pantalla](#captura-de-pantalla)
  - [Enlaces](#enlaces)
- [Mi proceso](#mi-proceso)
  - [Construido con](#construido-con)
  - [Lo que aprendí](#lo-que-aprendí)
  - [Desarrollo continuo](#desarrollo-continuo)
  - [Colaboración con IA](#colaboración-con-ia)
- [Autor](#autor)

---

## Visión general

### El desafío

Los usuarios deben ser capaces de:

- Visualizar el diseño óptimo del sitio en función del tamaño de pantalla de su dispositivo (Mobile & Desktop).


### Enlaces

- URL de la solución: [Añade la URL del repositorio aquí](https://github.com/YeiYei98/four-card-feature-section-master.git)
- URL del sitio web en vivo: [Añade la URL de GitHub Pages o Vercel aquí](https://yeiyei98.github.io/four-card-feature-section-master/)

---

## Mi proceso

### Construido con

- HTML5 semántico (`<main>`, `<section>`, `<h1>`, `<h2>`)
- Propiedades personalizadas de CSS (Variables)
- Flexbox (Para centrado global y estructura interna de las tarjetas)
- CSS Grid (`grid-template-areas` para el maquetado asimétrico)
- Enfoque *Mobile-first*
- Tipografía importada desde Google Fonts (Poppins: 200, 400, 600)

### Lo que aprendí

En este proyecto reforcé la alineación de tarjetas con **CSS Grid** en la vista de escritorio utilizando `grid-template-areas`. Esto me permitió manejar la disposición en cascada de forma clara y semántica:

\`\`\`css
@media (min-width: 600px) {
  main section:nth-child(2) {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    grid-template-rows: repeat(2, 1fr);
    grid-template-areas: 
      "supervisor builder    calculator"
      "supervisor karma      calculator";
    gap: 20px;
    align-items: center;
  }
}
\`\`\`

También trabajé la separación de bordes superiores dinámicos mediante colores de acento definidos con variables CSS:

\`\`\`css
.supervisor { border-top: 4px solid var(--color-cyan); }
.builder    { border-top: 4px solid var(--color-red); }
.karma      { border-top: 4px solid var(--color-orange); }
.calculator { border-top: 4px solid var(--color-blue); }
\`\`\`

### Desarrollo continuo

En mis próximos proyectos quiero enfocarme en:
- Reemplazar el posicionamiento absoluto en elementos secundarios dentro de tarjetas y priorizar **Flexbox** (`align-self`, `margin-top: auto`) para evitar colisiones de contenido.
- Refinar los puntos de interrupción (*media queries*) para asegurar transiciones suaves entre dispositivos medianos (tablets) y grandes monitores.

### Colaboración con IA

Utilicé asistentes de IA como apoyo técnico para:
- Refactorizar las áreas del **CSS Grid** y optimizar la alineación vertical de las tarjetas centrales (`Team Builder` y `Karma`).
- Auditar la semántica del marcado HTML y optimizar la nomenclatura de clases CSS.

---

## Autor

- Frontend Mentor - [@tu-usuario](https://www.frontendmentor.io/profile/tu-usuario)
- GitHub - [Ernesto González](https://github.com/YeiYei98)