# 🃏 Prueba Técnica - Componente de Cards Responsivo

Este repositorio contiene la solución implementada para el componente de cards responsivo, enfocada en crear un layout inteligente que se adapta automáticamente de 3 columnas (desktop) a 2 columnas (tablet) y 1 columna (móvil) usando únicamente HTML y CSS.

## 📁 Estructura del proyecto

```
/
├── index.html
├── styles.css
└── README.md
```

## 🎯 Componente de Cards Responsivo

**Objetivo:** Crear un grid de cards totalmente responsive (3 columnas desktop, 2 tablet, 1 móvil) usando solo HTML y CSS moderno.

#### 🔧 Implementación

##### Estructura HTML Semántica
- **Contenedor principal:** Usé `<section class="cards">` para definir semánticamente esta área como una sección de contenido relacionado
- **Cada card como artículo:** Implementé `<article class="card">` porque cada card representa contenido independiente que tiene sentido por sí solo
- **Jerarquía correcta:** El `<h2>` para el título de sección y `<h3>` para títulos de cards establece una estructura semántica clara
- **Convención BEM:** Aplicé una nomenclatura consistente y escalable

##### CSS Grid Inteligente
- **Responsive automático:** Implementé `repeat(auto-fit, minmax(300px, 1fr))` que crea el comportamiento deseado sin media queries complicadas
- **Flexbox para estructura interna:** Usé flexbox dentro de cada card para controlar la distribución del contenido
- **Alturas uniformes:** Todas las cards mantienen la misma altura independientemente del contenido
- **Efectos interactivos modernos:** Hover suave con elevación y transiciones optimizadas

#### 💡 Decisiones Técnicas Clave

**¿Por qué CSS Grid con `auto-fit`?**
Porque crea automáticamente el comportamiento responsive deseado:
- **Desktop:** 3 columnas cuando hay espacio para 3 cards de 300px
- **Tablet:** 2 columnas cuando solo caben 2
- **Móvil:** 1 columna cuando el espacio es menor

**¿Por qué Flexbox anidado?**
Grid maneja el layout general, pero Flexbox es perfecto para la estructura interna de cada card. Esto me permite que el contenido se distribuya correctamente y los footers queden alineados.

**¿Por qué `height: 100%` en las cards?**
Garantiza que todas las cards tengan la misma altura, creando una apariencia uniforme aunque el contenido tenga diferente longitud.

**¿Por qué `margin-top: auto` en el footer?**
Empuja automáticamente los botones hacia el fondo de cada card, manteniendo una alineación perfecta independientemente del texto de descripción.

---

## 🏆 Resultados Obtenidos

### ✅ Layout Responsive Inteligente
- Grid que se adapta automáticamente según el espacio disponible
- Transición suave entre breakpoints
- Funciona sin frameworks ni librerías externas
- Compatible con todos los navegadores modernos

### ✅ Experiencia de Usuario Optimizada
- Efectos hover elegantes con elevación sutil
- Botones interactivos con feedback visual
- Alturas uniformes para consistencia visual
- Transiciones suaves en todas las interacciones

### ✅ Código Limpio y Mantenible
- HTML semántico y accesible
- Convención BEM consistente
- CSS moderno sin dependencias

---

## 🚀 Tecnologías Utilizadas

- **HTML5** - Estructura semántica con `<section>` y `<article>`
- **CSS3** - Grid Layout, Flexbox, Transitions
- **Metodología BEM** - Nomenclatura clara y escalable

---

## 📱 Comportamiento Responsive

- ✅ **Desktop (>1024px)** - 3 columnas automáticas
- ✅ **Tablet (768px-1023px)** - 2 columnas optimizadas  
- ✅ **Móvil (768px)** - 1 columna con ajustes específicos
- ✅ **Móvil pequeño (<480px)** - Layout vertical optimizado

---
