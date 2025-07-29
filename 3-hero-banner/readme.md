# 📋 Prueba Técnica - Hero Banner Refactorización

Este repositorio contiene la solución implementada para la refactorización del componente hero/banner de Ultragoo, enfocada en mejorar la accesibilidad, estructura HTML y diseño responsive.

## 📁 Estructura del proyecto

```
/
├── index.html
├── styles.css
└── README.md
```

## 🎯 Refactorización del Hero Banner

**Objetivo:** Mejorar un componente hero/banner con problemas de accesibilidad, estructura HTML pobre y estilos no responsivos.

#### 🔧 Mejoras Implementadas

##### Estructura HTML
- **Etiquetas semánticas:** Cambié `<div class="main">` por `<section class="hero">` para mejor semántica
- **Accesibilidad mejorada:** 
  - Agregué `role="banner"` para identificar el banner principal
  - Incluí `aria-labelledby="hero-title"` para conectar la sección con su título
  - Agregué `aria-label` al botón CTA para mayor contexto
- **Jerarquía correcta:** Cambié `<h2>` por `<h1>` ya que es el título principal de la página
- **Convención BEM:** Implementé una nomenclatura clara y consistente

##### Estilos CSS Modernos
- **Flexbox para centrado:** Reemplacé el `margin-top: 200px` por Flexbox, más confiable y responsive
- **Mejora visual:** Agregué un overlay con `linear-gradient` para mejorar la legibilidad del texto
- **Tipografía responsive:** Implementé `clamp()` para texto que se adapta automáticamente
- **Botón interactivo:** Creé efectos modernos de hover/focus con `transform` y `box-shadow`
- **Diseño responsive:** Media queries optimizadas para tablet y móvil

#### 💡 Decisiones Técnicas Clave

**¿Por qué Flexbox?**
El código original usaba `margin-top: 200px` que es poco confiable. Flexbox garantiza centrado perfecto en cualquier dispositivo.

**¿Por qué `clamp()` en typography?**
Permite texto que se escala automáticamente entre un mínimo y máximo, eliminando la necesidad de múltiples media queries.

**¿Por qué el overlay degradado?**
Mejora significativamente la legibilidad del texto blanco sobre imágenes con colores variables.

---

## 🏆 Resultados Obtenidos

### ✅ Mejoras en Accesibilidad
- Estructura semántica completa
- Atributos ARIA implementados
- Navegación por teclado optimizada
- Contraste mejorado con overlays

### ✅ Performance y UX
- Diseño totalmente responsive sin frameworks
- Efectos interactivos suaves
- Tipografía escalable automáticamente
- Carga optimizada de imágenes

### ✅ Código Limpio
- Convención BEM consistente
- CSS moderno (Flexbox/Grid)
- HTML semántico y válido

---

## 🚀 Tecnologías Utilizadas

- **HTML5** - Estructura semántica
- **CSS3** - Flexbox, Grid, Custom Properties
- **Metodología BEM** - Nomenclatura de clases
- **Progressive Enhancement** - Funciona en todos los navegadores

---

## 📱 Compatibilidad

- ✅ Chrome/Edge (últimas versiones)
- ✅ Firefox (últimas versiones)  
- ✅ Safari (últimas versiones)
- ✅ Dispositivos móviles
- ✅ Lectores de pantalla

---

## 🔍 Cómo revisar el código

1. **Estructura:** Revisa cómo se implementó la semántica HTML
2. **Estilos:** Observa el uso de Flexbox/Grid para layouts modernos
3. **Responsive:** Prueba el diseño en diferentes tamaños de pantalla
4. **Accesibilidad:** Navega usando solo el teclado o un lector de pantalla
5. **Interacciones:** Experimenta con los efectos hover/focus

---