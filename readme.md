# CSS
 
1. Hoja de estilos en cascada
 
## VINCULACION HTML - CSS
 
1. Hoja de estilo externa usando etiqueta "link"
 
```html
<link rel="stylesheet" href="./styles.css" />
```
 
2. Usando la etiqueta "style"
 
```html
<style>
  h1 {
    color: red;
  }
</style>
```
 
3. De manera inline en el elemento con el atributo "style"
 
```html
<h1 style="color: red">CSS</h1>
```
# CSS
 
- Es un lenguaje para dar estilos a la web (1996)
 
## SINTAXIS
 
- Como se puede establecer codigo CSS
 
```css
h1 {
  color: red;
}
```
 
- h1 : Selector
- color : Propiedad
- red : Valor
 
## CONCEPTOS IMPORTANTES CSS
 
- 4 Conceptos importantes de CSS
 
### SELECTORES
 
- Indica a que elemento o elementos, se aplicara estilos
 
```css
/* SELECTOR DE ETIQUETA */
h1 {
  color: red;
}
 
/* SELECTOR DE DESCENDENCIA */
nav ul li a {
  color: red;
}
```
 
### HERENCIA
 
- Elementos ancestros heredan algunas propiedades a sus descendientes.
 
```html
<p>Hola mundo <a href="#">Esto es un enlace</a></p>
```
 
```css
p {
  color: peru;
}
 
a {
  color: inherit;
}
```
 
### CASCADA
 
- Significa que los estilos que llegan en ultimo lugar , sobreescriben a los de antes.
- La especificidad vence a la cascada
 
```css
h1 {
  color: red;
}
 
h1 {
  color: blue;
}
```
 
### ESPECIFICIDAD
 
- Es un valor numerico que adquieren los selectores y se aplica cuando hay conflictos
 
```html
<!-- Selector de Etiqueta (1) -->
 
<!-- Selector de Clase (10) -->
 
<!-- Selector de ID (100) -->
 
<!-- INLINE (1000) -->
 
<!-- IMPORTANT (infinito) -->
```
 
tiene menú contextual

