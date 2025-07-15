# Guía para el Aprendizaje 

## 1. ¿Cómo se organiza el proceso de ideación y desarrollo de un producto digital como una tienda online?

El proceso se divide en etapas clave:

### Ideación:
- **Definir el usuario objetivo**: Ejemplo: "Persona que compra en línea con necesidad de envíos rápidos".
- **Realizar lluvia de ideas para soluciones**: Ejemplo: "Carrito de compras intuitivo", "Filtros avanzados".
- **Refinar ideas con técnicas como SCAMPER** y seleccionar la más viable.

### Diseño:
- **Crear wireframes y prototipos** centrados en usabilidad (UX) y aspecto visual (UI).
- **Validar con pruebas de usuario tempranas**.

### Implementación:
- **Maquetación con HTML/CSS/JavaScript** siguiendo metodologías como BEM.
- **Uso de preprocesadores** (ejemplo: SASS) para estilos mantenibles.

### Iteración:
- **Mejorar basado en métricas y feedback**: Ejemplo: tasa de conversión.

**Ejemplo**: Para una tienda online, se priorizarían flujos como "búsqueda de productos" y "checkout simplificado".

---

## 2. ¿Cuál es el rol específico del diseñador UX/UI y del desarrollador front-end en este contexto?

### Diseñador UX:
- Investiga necesidades del usuario (ejemplo: entrevistas).
- Diseña flujos de navegación (ejemplo: recorrido desde el carrito hasta el pago).

### Diseñador UI:
- Crea la interfaz visual (ejemplo: paleta de colores, botones coherentes).
- Usa herramientas como Figma o Sketch.

### Desarrollador Front-End:
- Traduce diseños a código (HTML/CSS/JavaScript).
- Implementa interactividad (ejemplo: validación de formularios).
- Asegura compatibilidad y rendimiento.

**Sinergia**: El UX/UI define "qué" y "cómo" se usa; el front-end hace que funcione.

---

## 3. ¿Qué ventajas ofrecen las metodologías como BEM u OOCSS en la construcción del sitio?

### BEM:
- **Ventaja**: Bloques independientes (ejemplo: `.card__title--highlight`) evitan conflictos.
- **Ejemplo**: Facilita mantenimiento en equipos grandes.

### OOCSS:
- **Ventaja**: Separa estructura (márgenes) de skin (colores), promoviendo reutilización.
- **Ejemplo**: Clase `.btn` para estructura y `.btn-primary` para color.

### SMACSS:
- **Ventaja**: Categoriza estilos (base, layout, módulos) para escalabilidad.

**Impacto**: Código más limpio, menos redundante y fácil de actualizar.

---

## 4. ¿Qué preprocesador CSS utilizarías y por qué?

**Recomendación**: **SASS (SCSS)**, por:

- **Variables y mixins**: Permite reutilizar colores o funciones (ejemplo: `@mixin flex-center`).
- **Anidación**: Organiza estilos jerárquicamente (ejemplo: anidar estilos de un `.navbar`).
- **Modularidad**: Divide código en archivos parciales (`_buttons.scss`, `_forms.scss`).
- **Comunidad y soporte**: Ampliamente adoptado (usado en Bootstrap).

**Alternativa**: LESS es más simple pero menos potente; Stylus es flexible pero menos popular.

---

## 5. ¿Cómo se representa de forma eficiente una guía de estilos?

Una guía útil debe ser:

- **Visual**: Incluir ejemplos de componentes (botones, formularios) con código y diseño.
- **Modular**: Organizada por categorías (tipografía, colores, componentes).
- **Actualizable**: Vinculada a repositorios (ejemplo: GitHub).
- **Educativa**: Explicar "por qué" (ejemplo: "El azul (#2BA47D) refuerza la marca").

**Ejemplo práctico**:
```markdown
## Botones  
- **Primario**: Fondo azul (`$primary-color`), padding 1em.  
  ```html 
  <button class="btn btn--primary">Comprar</button>