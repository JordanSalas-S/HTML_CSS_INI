# CSS
 
- Hoja de estilos en cascada **(Cascading Style Sheets)**
- Es un lenguaje para dar estilos a la web (1996)
 
## VINCULACION HTML - CSS
 
1. Hoja de estilo externa usando etiqueta "link" 

```html
<link rel="stylesheet" href="./styles.css" />
```

2. Usando la etiqueta "**style**"
 
```html
<style>
  h1 {
    color: red;
  }
</style>
```
 
3. De manera inline en el elemento con el atributo "**style**"
 
```html
<h1 style="color: red">CSS</h1>
```
 
## SINTAXIS
 
- Como se puede establecer codigo CSS.
 
```css
h1 {
  color: red;
}
```
 
- **h1** : Selector
- **color** : Propiedad
- **red** : Valor
 
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
 
---

# ESTILOS DE TEXTO
 
## PROPIEDADES
 
- **color** _sirve para poder cambiar el color al texto_
```css
h1{
  color: rgb(157, 189, 28);
}
```

- **font-size (em,rem,px)** _sirve para poder agrandar el texto, en base a *_*px** (pixeles)_
- **em** : _se basa en el tamaño de la fuente del elemento actual, lo que significa que el tamaño de un elemento en em será relativo al tamaño de la fuente del elemento que lo contiene_
- **rem**: _es una unidad de medida que se utiliza para especificar el tamaño de un elemento en una página web que se basa en el tamaño de la fuente del elemento raíz o etiqueta html_  
```css
h1{
  font-size: 25px;
}
```
- **font-weight (peso de tipografia)** _especifica el peso o groso de la letra de 100 a 900_
  - **normal**  Igual que 400.
  - **bold** Grueso ancho (negrita). Igual que 700
```css
h1{
  font-weight: 300;
}
```

- **text-transform: uppercase | lowercase | capitalize** _Permite tranformar el texto , en formatos especiales para poder escribir en mayuscula las primeras letras de cada palabra_
```css
h1{
  text-transform: uppercase;
}
```

- **text-align : left | center | right** _sirve para alinear un bloque de texto_
```css
h1 {
  text-align: center;
}
```

- **text-decoration : none | underline** _Especifica si la etiqueta tendra un borde_
  - **none** esto no causara ningun cambio 
  - **underline**  subrayado
```css
h1{
  text-decoration: underline;
}
```

- font-family (google fonts - fontface) define una lista de fuentes
- estilo entre navegadores (normalize.css)
 
## SELECTORES
 
- Selector de Etiqueta(1)
- Selector de Clase(10)
- Selector de ID(100)
- Selector Universal (uso box model)
 
 
<!-- Actualizar el repositorio con lo visto en la 2da parte
  1) Explicar los conceptos con ejemplos
  2) (Agregar una nueva tipografia de google fonts, usando font-face)
-->
 