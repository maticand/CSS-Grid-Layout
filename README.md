<!-- wp:heading -->
<h2>¿Qué es CSS Grids?</h2>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p><strong>CSS Grid Layout</strong> es un módulo de maquetación CSS que nos permite generar layouts en nuestras páginas web de una forma más eficiente, está basado en un sistema de grillas (filas y columnas) y además es soportado por todos los navegadores modernos.</p>
<!-- /wp:paragraph -->

<!-- wp:heading {"level":3} -->
<h3>Conceptos fundamentales sobre CSS Grid Layout</h3>
<!-- /wp:heading -->

<!-- wp:html -->
<div style="height:20px" aria-hidden="true" class="wp-block-spacer"></div>
<!-- /wp:html -->

<!-- wp:paragraph -->
<p><strong>grid container:</strong> es el elemento padre, y hay que asignarle un nuevo tipo de display llamado <strong>grid</strong> dentro de la hoja de estilos. </p>
<!-- /wp:paragraph -->

<!-- wp:code -->
<pre class="wp-block-code"><code>display: grid;</code></pre>
<!-- /wp:code -->

<!-- wp:html -->
<div style="height:20px" aria-hidden="true" class="wp-block-spacer"></div>
<!-- /wp:html -->

<!-- wp:paragraph -->
<p><strong>grid item:</strong> son los hijos directos de un <strong>grid container</strong>, y son los componentes que vamos a poder colocar a nuestro gusto dentro del layout.</p>
<!-- /wp:paragraph -->

<!-- wp:code -->
<pre class="wp-block-code"><code>&lt;!-- Grid container -->
  &lt;section class="container">
&lt;!-- Grid item --> 
    &lt;div class="item">contenido 1&lt;/div>
    &lt;div class="item">contenido 2&lt;/div>
    &lt;div class="item">contenido 3&lt;/div>
    &lt;div class="item">contenido 4&lt;/div>
    &lt;div class="item">contenido 5&lt;/div>
    &lt;div class="item">contenido 6&lt;/div> 
  &lt;/section></code></pre>
<!-- /wp:code -->

<!-- wp:html -->
<div style="height:20px" aria-hidden="true" class="wp-block-spacer"></div>
<!-- /wp:html -->

<!-- wp:paragraph -->
<p><strong>grid line:</strong>&nbsp;son lineas invisibles verticales y horizontales que dividen la grilla y separan las columnas y filas.</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>En este caso corresponde a las lineas azules:</p>
<!-- /wp:paragraph -->

<!-- wp:image {"id":202} -->
<figure class="wp-block-image"><img src="http://matiascandia.mitemplate.com/wp-content/uploads/sites/35/2019/06/grid-lines-css-grid.png" alt="" class="wp-image-202"/></figure>
<!-- /wp:image -->

<!-- wp:html -->
<div style="height:20px" aria-hidden="true" class="wp-block-spacer"></div>
<!-- /wp:html -->

<!-- wp:paragraph -->
<p><strong>grid cell:</strong>&nbsp;es un componente dentro de la grilla y se lo denomina como celda.</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>En este caso corresponde al contenido 3:</p>
<!-- /wp:paragraph -->

<!-- wp:image {"id":222,"width":524,"height":153} -->
<figure class="wp-block-image is-resized"><img src="http://matiascandia.mitemplate.com/wp-content/uploads/sites/35/2019/06/grid-cell-css-grid-1.png" alt="" class="wp-image-222" width="524" height="153"/></figure>
<!-- /wp:image -->

<!-- wp:html -->
<div style="height:20px" aria-hidden="true" class="wp-block-spacer"></div>
<!-- /wp:html -->

<!-- wp:paragraph -->
<p><strong>grid track:</strong>&nbsp;se corresponde con las filas y columnas.</p>
<!-- /wp:paragraph -->

<!-- wp:image {"id":225} -->
<figure class="wp-block-image"><img src="http://matiascandia.mitemplate.com/wp-content/uploads/sites/35/2019/06/grid-track-css-grid.png" alt="" class="wp-image-225"/></figure>
<!-- /wp:image -->

<!-- wp:html -->
<div style="height:20px" aria-hidden="true" class="wp-block-spacer"></div>
<!-- /wp:html -->

<!-- wp:paragraph -->
<p><strong>grid area:</strong> es un espacio conformado por 4 <strong>grid lines</strong>, el cual, puede ser desde 1 celda a muchas.</p>
<!-- /wp:paragraph -->

<!-- wp:image {"id":232} -->
<figure class="wp-block-image"><img src="http://matiascandia.mitemplate.com/wp-content/uploads/sites/35/2019/06/grid-area-css-grid.png" alt="" class="wp-image-232"/></figure>
<!-- /wp:image -->

<!-- wp:html -->
<div style="height:20px" aria-hidden="true" class="wp-block-spacer"></div>
<!-- /wp:html -->

<!-- wp:heading {"level":3} -->
<h3>Filas y columnas </h3>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p>Para agregar columnas hacemos algo tan simple como agregar lo siguiente al contenedor padre en el archivo .css</p>
<!-- /wp:paragraph -->

<!-- wp:code -->
<pre class="wp-block-code"><code>grid-template-columns: 25% 50% 25%;</code></pre>
<!-- /wp:code -->

<!-- wp:paragraph -->
<p>Y para agregar filas agregamos lo siguiente:</p>
<!-- /wp:paragraph -->

<!-- wp:code -->
<pre class="wp-block-code"><code>grid-template-rows: 300px,200px;</code></pre>
<!-- /wp:code -->

<!-- wp:html -->
<div style="height:20px" aria-hidden="true" class="wp-block-spacer"></div>
<!-- /wp:html -->

<!-- wp:paragraph -->
<p><strong>Grid explicito</strong>&nbsp;(explicit grid): es cuando nosotros definimos el numero de filas o columnas. Usa grid-template-rows Y grid-template-columns.</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p><strong>Grid implicito</strong>&nbsp;(implicit grid): es cuando tenemos filas o columnas que no definimos pero son parte de nuestro grid. Usa grid-auto-rows Y grid-auto-columns.</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>Aqui se explica con mas  detalle:<br><a rel="noreferrer noopener" href="https://www.quackit.com/css/grid/tutorial/explicit_vs_implicit_grid.cfm" target="_blank">Implicit/Explicit Grid</a></p>
<!-- /wp:paragraph -->

<!-- wp:image {"id":240} -->
<figure class="wp-block-image"><img src="http://matiascandia.mitemplate.com/wp-content/uploads/sites/35/2019/06/css-grid-explicito-e-implicito.png" alt="" class="wp-image-240"/></figure>
<!-- /wp:image -->

<!-- wp:paragraph -->
<p>Para designar filas y columnas de una forma resumida lo hacemos de la siguiente manera:</p>
<!-- /wp:paragraph -->

<!-- wp:code -->
<pre class="wp-block-code"><code>grid-template: 150px 150px 100px / 25% 25% 50%;</code></pre>
<!-- /wp:code -->

<!-- wp:html -->
<div style="height:20px" aria-hidden="true" class="wp-block-spacer"></div>
<!-- /wp:html -->

<!-- wp:heading {"level":3} -->
<h3>Propiedades en CSS Grid Layout</h3>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p><strong>grid-template-columns</strong>: define el numero de columnas en un grid layout, así como el tamaño en ancho de cada columna.</p>
<!-- /wp:paragraph -->

<!-- wp:preformatted -->
<pre class="wp-block-preformatted">grid-template-columns: 200px 200px 200px;</pre>
<!-- /wp:preformatted -->

<!-- wp:html -->
<div style="height:20px" aria-hidden="true" class="wp-block-spacer"></div>
<!-- /wp:html -->

<!-- wp:paragraph -->
<p><strong>grid-template-rows</strong>: para definir las filas.</p>
<!-- /wp:paragraph -->

<!-- wp:preformatted -->
<pre class="wp-block-preformatted">grid-template-rows: valores;</pre>
<!-- /wp:preformatted -->

<!-- wp:html -->
<div style="height:20px" aria-hidden="true" class="wp-block-spacer"></div>
<!-- /wp:html -->

<!-- wp:paragraph -->
<p><strong>grid-template</strong>: definir filas y columnas:</p>
<!-- /wp:paragraph -->

<!-- wp:preformatted -->
<pre class="wp-block-preformatted">grid-template: filas / columnas;</pre>
<!-- /wp:preformatted -->

<!-- wp:html -->
<div style="height:20px" aria-hidden="true" class="wp-block-spacer"></div>
<!-- /wp:html -->

<!-- wp:paragraph -->
<p><strong>display subgrid</strong>: para heredar la configuración del grid padre (cuando se esten anidando grids).</p>
<!-- /wp:paragraph -->

<!-- wp:preformatted -->
<pre class="wp-block-preformatted">display: subgrid; //No disponible aun</pre>
<!-- /wp:preformatted -->

<!-- wp:html -->
<div style="height:20px" aria-hidden="true" class="wp-block-spacer"></div>
<!-- /wp:html -->

<!-- wp:paragraph -->
<p><strong>display inline-grid</strong>:&nbsp;muestra el grid en una sola linea:</p>
<!-- /wp:paragraph -->

<!-- wp:preformatted -->
<pre class="wp-block-preformatted">display: inline-grid; //No disponible aun</pre>
<!-- /wp:preformatted -->

<!-- wp:html -->
<div style="height:20px" aria-hidden="true" class="wp-block-spacer"></div>
<!-- /wp:html -->

<!-- wp:paragraph -->
<p><strong>grid-column-gap</strong>:&nbsp;espaciado entre columnas</p>
<!-- /wp:paragraph -->

<!-- wp:preformatted -->
<pre class="wp-block-preformatted">grid-column-gap: 10px; </pre>
<!-- /wp:preformatted -->

<!-- wp:html -->
<div style="height:20px" aria-hidden="true" class="wp-block-spacer"></div>
<!-- /wp:html -->

<!-- wp:paragraph -->
<p><strong>grid-row-gap</strong>:&nbsp;espaciado entre filas</p>
<!-- /wp:paragraph -->

<!-- wp:preformatted -->
<pre class="wp-block-preformatted">grid-row-gap: 10px; </pre>
<!-- /wp:preformatted -->

<!-- wp:html -->
<div style="height:20px" aria-hidden="true" class="wp-block-spacer"></div>
<!-- /wp:html -->

<!-- wp:paragraph -->
<p><strong>grid-gap</strong>:&nbsp;espaciado entre filas y columnas</p>
<!-- /wp:paragraph -->

<!-- wp:preformatted -->
<pre class="wp-block-preformatted">grid-gap: 10px 20px;</pre>
<!-- /wp:preformatted -->

<!-- wp:html -->
<div style="height:20px" aria-hidden="true" class="wp-block-spacer"></div>
<!-- /wp:html -->

<!-- wp:heading {"level":3} -->
<h3>Unidades de medida y funciones</h3>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p>Para definir el tamaño de las filas y columnas podemos utilizar cualquier unidad de medida, pero hay ciertos valores y funciones que nos pueden ayudar a hacerlo mas fácilmente:</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p><strong>fr (fracciones)</strong>: es una unidad de medida exclusiva para<strong> CSS Grid </strong>que representa una fracción del espacio disponible en el contenedor de la cuadricula. Distrubuye el espacio disponible en formas iguales.</p>
<!-- /wp:paragraph -->

<!-- wp:code -->
<pre class="wp-block-code"><code>grid-template: 1fr 2fr 3fr / repeat(4, 1fr);</code></pre>
<!-- /wp:code -->

<!-- wp:paragraph -->
<p><strong>auto</strong>: define un tamaño automático para una fila o columna, según el alto si es fila, o ancho si es columna.</p>
<!-- /wp:paragraph -->

<!-- wp:code -->
<pre class="wp-block-code"><code>grid-template: 100px / auto auto;</code></pre>
<!-- /wp:code -->

<!-- wp:paragraph -->
<p><strong>repeat (cantidad, tamaño)</strong>: esta función nos permite repetir un valor x cantidad de veces.</p>
<!-- /wp:paragraph -->

<!-- wp:code -->
<pre class="wp-block-code"><code>grid-template: 100px / repeat(4, 250px);</code></pre>
<!-- /wp:code -->

<!-- wp:paragraph -->
<p><strong>repeat (auto-fill, tamaño)</strong>: si en vez de un numero llenamos la cantidad con el valor de <em>auto-fill</em> nos permitiría crear una cantidad de columnas o filas según quepan en el <strong>grid container</strong> con el tamaño definido.</p>
<!-- /wp:paragraph -->

<!-- wp:code -->
<pre class="wp-block-code"><code>grid-template: 100px / repeat(auto-fill, 250px);</code></pre>
<!-- /wp:code -->

<!-- wp:paragraph -->
<p><strong>minmax ()</strong>:&nbsp; define un ancho flexible entre 2 números (ancho minimo y maximo) para una fila o columna.</p>
<!-- /wp:paragraph -->

<!-- wp:code -->
<pre class="wp-block-code"><code>grid-template: 100px / minmax(100px, 500px);</code></pre>
<!-- /wp:code -->

<!-- wp:html -->
<div style="height:20px" aria-hidden="true" class="wp-block-spacer"></div>
<!-- /wp:html -->

<!-- wp:heading {"level":3} -->
<h3>Áreas de contenido</h3>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p><strong>grid-template-areas: </strong>define multiples <strong>grid area </strong>dentro del <strong>grid container</strong>, mediante un nombre personalizado para cada una de ellas, las cuales, nos permitirán modificar de manera dinámica la ubicación y cuantas filas o columnas abarcaran nuestros <strong>grid items</strong> en la cuadricula.</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>Para definir un <strong>grid area</strong> en nuestra cuadricula utilizamos comillas("") para indicar una fila y adentro definimos las columnas mediante un nombre personalizado o un punto(.) para que la celda valla vacía, y los valores los separamos con un espacio.</p>
<!-- /wp:paragraph -->

<!-- wp:code -->
<pre class="wp-block-code"><code>.container{
  display: grid;
  grid-template: 100px 1fr 150px / 200px 1fr;
  grid-gap: 10px;
  height: 100vh;
  grid-template-areas: "header header"
                       "sidebar contenido"
                       "footer footer";
}
</code></pre>
<!-- /wp:code -->

<!-- wp:paragraph -->
<p>Aquí estamos definiendo una cuadricula de 3*2 , en la cual, asignamos multiples <strong>grid areas </strong>identificadas con 4 nombres diferentes que llenaran la cuadricula cuando los asignemos a los hijos directos <strong>grid item </strong>del<strong> grid container.</strong></p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p><strong>grid-area</strong>: asigna un <strong>grid area</strong> mediante su nombre a un <strong>grid item</strong>, y se usa en conjunto para poder trabajar con la propiedad <strong>grid-template-areas.</strong></p>
<!-- /wp:paragraph -->

<!-- wp:code -->
<pre class="wp-block-code"><code>	.header {
		grid-area: header;
	}
	.sidebar {
		grid-area: sidebar;
	}
	.contenido {
		grid-area: contenido;
	}
	.footer {
		grid-area: footer;
	}
</code></pre>
<!-- /wp:code -->

<!-- wp:paragraph -->
<p>Aquí estamos asignando las <strong>grid areas</strong> que declaramos en el <strong>grid container</strong> a cada uno de los <strong>grid</strong><em><strong> </strong></em><strong>items</strong>, quedando como resultado lo siguiente:</p>
<!-- /wp:paragraph -->

<!-- wp:image {"id":272} -->
<figure class="wp-block-image"><img src="http://matiascandia.mitemplate.com/wp-content/uploads/sites/35/2019/06/areas-en-css-grid-1024x478.png" alt="" class="wp-image-272"/></figure>
<!-- /wp:image -->

<!-- wp:html -->
<div style="height:20px" aria-hidden="true" class="wp-block-spacer"></div>
<!-- /wp:html -->

<!-- wp:heading {"level":3} -->
<h3>Definiendo el tamaño de las columnas dentro de un grid</h3>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p>Para definir el número de <strong>grid lines</strong> que ocupará un elemento, usamos la propiedad <strong>grid-column-start</strong> y <strong>grid-column-end</strong>, esto para definir desde que línea comenzará determinado elemento y en que línea terminará.</p>
<!-- /wp:paragraph -->

<!-- wp:code -->
<pre class="wp-block-code"><code>grid-column-start: 1;

grid-column-end: 3;</code></pre>
<!-- /wp:code -->

<!-- wp:paragraph -->
<p>Para resumir estos parámetros podemos usar la propiedad <strong>grid-column</strong> y de esta forma ponerle los parámetros en los que empieza y termina el elemento (separados por /).</p>
<!-- /wp:paragraph -->

<!-- wp:code -->
<pre class="wp-block-code"><code>grid-column: 2 / 4;</code></pre>
<!-- /wp:code -->

<!-- wp:paragraph -->
<p>Cuando queremos ahorrarnos los parámetros de inicio y final de un elemento, podemos usar -1 en ambos casos.</p>
<!-- /wp:paragraph -->

<!-- wp:code -->
<pre class="wp-block-code"><code>grid-column:  1 / -1;</code></pre>
<!-- /wp:code -->

<!-- wp:paragraph -->
<p>Para indicar que queremos usar espacios y no líneas, usamos de antemano “span”.</p>
<!-- /wp:paragraph -->

<!-- wp:code -->
<pre class="wp-block-code"><code>grid-column: 1  / span 2;</code></pre>
<!-- /wp:code -->

<!-- wp:image {"id":275} -->
<figure class="wp-block-image"><img src="http://matiascandia.mitemplate.com/wp-content/uploads/sites/35/2019/06/tamaño-de-las-columnas-dentro-de-un-grid-css-grid-1024x478.png" alt="" class="wp-image-275"/></figure>
<!-- /wp:image -->

<!-- wp:html -->
<div style="height:20px" aria-hidden="true" class="wp-block-spacer"></div>
<!-- /wp:html -->



