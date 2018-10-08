---
id: bad87fee1348bd9aedf08807
title: Import a Google Font
localeTitle: Importar una fuente de Google
challengeType: 0
videoUrl: ''
---

## Description
<section id='description'> 
Además de especificar las fuentes comunes que se encuentran en la mayoría de los sistemas operativos, también podemos especificar fuentes web no estándar y personalizadas para su uso en nuestro sitio web. Existen varias fuentes de fuentes web en Internet, pero, para este ejemplo, nos centraremos en la biblioteca de fuentes de Google. 
<a href='https://fonts.google.com/' target='_blank'>Google Fonts</a> es una biblioteca gratuita de fuentes web que puede usar en su CSS haciendo referencia a la URL de la fuente. 
Entonces, sigamos adelante, importemos y apliquemos una fuente de Google (tenga en cuenta que si Google está bloqueado en su país, deberá saltarse este desafío). 
Para importar una fuente de Google, puede copiar la URL de la (s) fuente (s) de la biblioteca de fuentes de Google y luego pegarla en su HTML. Para este desafío, importaremos la fuente <code>Lobster</code> . Para hacer esto, copie el siguiente fragmento de código y péguelo en la parte superior de su editor de código (antes del elemento de <code>style</code> apertura): 
<code>&lt;link href=&quot;https://fonts.googleapis.com/css?family=Lobster&quot; rel=&quot;stylesheet&quot; type=&quot;text/css&quot;&gt;</code> 
Ahora puedes usar la fuente <code>Lobster</code> en tu CSS usando <code>Lobster</code> como el FAMILY_NAME como en el siguiente ejemplo: <br> <code>font-family: FAMILY_NAME, GENERIC_NAME;</code> . 
El GENERIC_NAME es opcional, y es una fuente alternativa en caso de que la otra fuente especificada no esté disponible. Esto está cubierto en el próximo desafío. 
Los nombres de las familias distinguen entre mayúsculas y minúsculas y deben incluirse entre comillas si hay un espacio en el nombre. Por ejemplo, necesita citas para usar la fuente <code>&quot;Open Sans&quot;</code> , pero no para usar la fuente <code>Lobster</code> . 
</section>

## Instructions
<section id='instructions'> 
Cree una regla CSS de la <code>font-family</code> que use la fuente <code>Lobster</code> y asegúrese de que se aplicará a su elemento <code>h2</code> . 
</section>

## Tests
<section id='tests'>

```yml
tests:
  - text: Importar la fuente de la <code>Lobster</code> .
    testString: 'assert(new RegExp("googleapis", "gi").test(code), "Import the <code>Lobster</code> font.");'
  - text: Tu elemento <code>h2</code> debe usar la fuente <code>Lobster</code> .
    testString: 'assert($("h2").css("font-family").match(/lobster/i), "Your <code>h2</code> element should use the font <code>Lobster</code>.");'
  - text: Utilice un selector <code>h2</code> CSS para cambiar la fuente.
    testString: 'assert(/\s*h2\s*\{\s*font-family\:\s*(\"|")?Lobster(\"|")?\s*;\s*\}/gi.test(code), "Use an <code>h2</code> CSS selector to change the font.");'
  - text: Tu elemento <code>p</code> debería seguir utilizando la fuente <code>monospace</code> .
    testString: 'assert($("p").css("font-family").match(/monospace/i), "Your <code>p</code> element should still use the font <code>monospace</code>.");'

```

</section>

## Challenge Seed
<section id='challengeSeed'>

<div id='html-seed'>

```html
<style>
  .red-text {
    color: red;
  }

  p {
    font-size: 16px;
    font-family: monospace;
  }
</style>

<h2 class="red-text">CatPhotoApp</h2>
<main>
  <p class="red-text">Click here to view more <a href="#">cat photos</a>.</p>

  <a href="#"><img src="https://bit.ly/fcc-relaxing-cat" alt="A cute orange cat lying on its back."></a>

  <div>
    <p>Things cats love:</p>
    <ul>
      <li>cat nip</li>
      <li>laser pointers</li>
      <li>lasagna</li>
    </ul>
    <p>Top 3 things cats hate:</p>
    <ol>
      <li>flea treatment</li>
      <li>thunder</li>
      <li>other cats</li>
    </ol>
  </div>

  <form action="/submit-cat-photo">
    <label><input type="radio" name="indoor-outdoor" checked> Indoor</label>
    <label><input type="radio" name="indoor-outdoor"> Outdoor</label><br>
    <label><input type="checkbox" name="personality" checked> Loving</label>
    <label><input type="checkbox" name="personality"> Lazy</label>
    <label><input type="checkbox" name="personality"> Energetic</label><br>
    <input type="text" placeholder="cat photo URL" required>
    <button type="submit">Submit</button>
  </form>
</main>
```

</div>



</section>

## Solution
<section id='solution'>

```js
// solution required
```
</section>