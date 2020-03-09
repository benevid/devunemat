# HTML para iniciantes

> From: https://html.com/
>
> https://github.com/ronreiter/interactive-tutorials
>
> https://www.tutorialspoint.com/html/index.htm
>
> https://www.caelum.com.br/apostila-html-css-javascript/

## Onde vamos chegar?

### Mern Stack

A frase "pilha MERN" ou *Mern Stack* refere-se às seguintes tecnologias:

- **M**ongoDB: é um programa de banco de dados orientado a documentos multiplataforma
- **E**xpress.js:  ou simplesmente **Express**, é um framework para aplicações web para Node.js
- **R**eact: é uma biblioteca JavaScript para criar interfaces de usuário (Front-End).
- **N**ode.js: é um ambiente open source que executa o código JavaScript fora de um navegador



![Imagem relacionada](https://i.morioh.com/139b757e13.png)



## 5 aplicações feitas com a pilha MERN

### FaceBook



![img](https://miro.medium.com/max/2000/1*uarchLLEO5mIYHZ3FebzVw.jpeg)

### Instagram



![img](https://miro.medium.com/max/3000/1*KT-t4xip0H4Zv6i3J2U0lA.jpeg)

### WhatsApp



![img](https://miro.medium.com/max/2560/1*6XKvsvlvcyT_q33k6cWxhg.jpeg)

## DropBox



![img](https://miro.medium.com/max/1600/1*YsRZaWrj-nLrDUuUIGvsNg.jpeg)

## NetFlix



![img](https://miro.medium.com/max/2800/1*fczbqHBKuYq9XL1QQVifJA.jpeg)



### O que é HTML?

Ok, então este é o único pedaço de teoria obrigatória. Para começar a escrever HTML, ajuda se você souber o que está escrevendo.

HTML é o **idioma em que a maioria dos sites é escrita** . HTML é usado para criar páginas e torná-las funcionais.

### A história do HTML

O HTML foi criado pela primeira vez por **Tim Berners-Lee, Robert Cailliau** e outros a partir de **1989** . Significa Hyper Text Markup Language.

Hipertexto significa que o documento contém **links que permitem ao leitor pular para outros locais** do documento ou para outro documento completamente. A versão mais recente é conhecida como [HTML5](https://html.com/html5/) .

#### O que são tags HTML?

[As tags](https://html.com/tags/) são usadas para **marcar o início de um elemento HTML** e geralmente são colocadas entre colchetes angulares. Um exemplo de uma tag é: `<h1>`.

A maioria das tags deve ser aberta `<h1> `e fechada `</h1>`para funcionar.

#### O que são atributos HTML?

[Os atributos](https://html.com/attributes/) contêm **informações adicionais** . Os atributos assumem a forma de uma tag de abertura e informações adicionais são **inseridas** .

Um exemplo de um atributo é:

`<img src="mydog.jpg" alt="A photo of my dog.">`

Nesse caso, a fonte da imagem (src) e o texto alternativo (alt) são atributos da  da `<img>` tag..

#### Construção básica de uma página HTML

![Estrutura HTML](https://html.com/wp-content/uploads/html-homepage-layout-demo.png)



#### Tags adicionais

Dentro da tag `<head>`, há uma tag  inclusa `<title>`, mas há outras que são igualmente importantes:

- `<title>`

  É aqui que **inserimos o nome da página** , que aparecerá na parte superior da janela ou guia do navegador.

- `<meta>`

  É aqui que as informações *sobre* o documento são armazenadas: codificação de caracteres, nome (contexto da página), descrição.

**Vamos experimentar uma ``seção básica :**

```html
<head>
<title>Minha Página</title>
<meta charset="UTF-8">
<meta name="description" content="breve descrição da pagina.">.
<meta name="author" content="Dev Unemat">
</header>
```

### Adicionando conteúdo

Só para lhe dar uma pequena empolgação com o HTML, um **HTML Hello World** . 

```html
<!DOCTYPE html>
<html>
   <head>
      <title>Minha Primeira Página</title>
   </head>	
   <body>
      <h1>Olá mundo</h1>
      <p>Hello World!</p>
   </body>	
</html>
```

# Elementos básicos

Os elementos básicos de uma página HTML são:

Um cabeçalho de texto, denotado usando os , , , , , tags.`<h1><h2><h3><h4><h5><h6>`
Um parágrafo, indicado usando a tag`<p>`
Uma régua horizontal, indicada usando a tag `<hr>`
Um link, indicado usando a tag (anchor) `<a>`
Uma lista, indicada usando as tags (lista não ordenada), (lista ordenada) e (elemento da lista).`<ul><ol><li>`
Uma imagem, denotada usando a tag `<img>`
Um divisor, indicado usando a tag`<div>`
Um período de texto, indicado usando a tag `<span>`

Cada elemento também pode ter atributos - cada elemento tem um conjunto diferente de atributos relevantes para o elemento. Existem alguns elementos globais, os mais comuns deles são:

- `id`- Indica o ID exclusivo de um elemento em uma página. Usado para localizar elementos usando links, JavaScript e muito mais.
- `class`- Indica a classe CSS de um elemento. Explicado no tutorial [Básico de CSS](https://www.learn-html.org/en/CSS_Basics) .
- `style`- Indica os estilos CSS a serem aplicados a um elemento. Explicado no tutorial [Básico de CSS](https://www.learn-html.org/en/CSS_Basics) .
- `data-x` atributos - um prefixo geral para atributos que armazenam informações brutas para fins programáticos. Explicado em detalhes na seção [Atributos de Dados](https://www.learn-html.org/en/Data_Attributes) .

### Ligações (Links)

------

Um link ("**âncora**") é um pequeno espaço de texto que o direcionará para uma seção diferente da página ou para uma página diferente. Para criar um link, você precisará especificar para onde deseja que o usuário seja direcionado quando o link for clicado, especificando o `href`atributo.

Por exemplo:

```html
<a href="https://www.google.com">A link to Google</a>
```

Para criar um link para uma seção diferente na mesma página, você precisará usar um sinal de hash junto com o ID do elemento para onde deseja que o navegador vá. Por exemplo:

```html
<a href="#faq">Click here to read the Frequently Asked Questions</p>
```

O ID do elemento é indicado usando o `id`atributo:

```html
<h3 id="faq">Frequently asked questions</h3>
<p>The first rule about fight club is that you do not talk about fight club.</p>
```

Vamos tentar:

```html
<!DOCTYPE html>
<html>
    <head>
    </head>
    <body>
        <h1>My First Page</h1>
        <p>This is my first page.</p>
        <a href="#faq">Click here to read the Frequently Asked Questions</a>
        <hr/>
        <h3 id="faq">Frequently asked questions</h3>
        <p>The first rule about fight club is that you do not talk about fight club.</p>
        <p>However, if you do have questions, please e-mail me at foo@bar.com</p>

    </body>
</html>
```

# Listas

------

O HTML fornece uma maneira de criar uma lista ordenada (com contagem de elementos 1, 2, 3 ...) e uma lista não ordenada com marcadores em vez de números. As listas são uma boa maneira de formalizar uma lista de itens e permitir que o estilo HTML faça o trabalho por você.

### Listas ordenadas

Aqui está um exemplo de como criar uma lista ordenada:

```html
<p>Here is a list of ordered items:</p>
<ol>
    <li>First item</li>
    <li>Second item</li>
    <li>Third item</li>
</ol>
```

As listas ordenadas têm um atributo "type" que define a convenção de numeração a ser usada.

Para contar usando números, use o tipo = "1":

```html
<p>Here is a list of ordered items:</p>
<ol type="1">
    <li>First item</li>
    <li>Second item</li>
    <li>Third item</li>
</ol>
```

Para contar usando letras maiúsculas, use o tipo = "A":

```html
<p>Here is a list of ordered items:</p>
<ol type="A">
    <li>First item</li>
    <li>Second item</li>
    <li>Third item</li>
</ol>
```

Para contar usando letras minúsculas, use o tipo = "a":

```html
<p>Here is a list of ordered items:</p>
<ol type="a">
    <li>First item</li>
    <li>Second item</li>
    <li>Third item</li>
</ol>
```

Para contar usando algarismos romanos maiúsculos, use o tipo = "I":

```html
<p>Here is a list of ordered items:</p>
<ol type="I">
    <li>First item</li>
    <li>Second item</li>
    <li>Third item</li>
</ol>
```

Para contar usando números romanos em minúsculas, use o tipo = "i":

```html
<p>Here is a list of ordered items:</p>
<ol type="i">
    <li>First item</li>
    <li>Second item</li>
    <li>Third item</li>
</ol>
```

### Listas não ordenadas

Aqui está um exemplo de como criar uma lista não ordenada:

```html
<p>Here is a list of unordered items:</p>    
<ul>
    <li>First item</li>
    <li>Second item</li>
    <li>Third item</li>
</ul>
```

Para alterar os atributos de estilo da lista, podemos usar o atributo CSS chamado `list-style-type`. Os tipos disponíveis são:

- disco (disc)
- círculo (circle)
- quadrado (square)
- Nenhum (none)

Aqui está um exemplo do tipo de estilo da lista de discos:

```html
<p>Here is a list of unordered items:</p>    
<ul style="list-style-type: disc">
    <li>First item</li>
    <li>Second item</li>
    <li>Third item</li>
</ul>
```

Aqui está um exemplo do tipo de estilo da lista de círculos:

```html
<p>Here is a list of unordered items:</p>    
<ul style="list-style-type: circle">
    <li>First item</li>
    <li>Second item</li>
    <li>Third item</li>
</ul>
```

Aqui está um exemplo do tipo de estilo de lista quadrada:

```html
<p>Here is a list of unordered items:</p>    
<ul style="list-style-type: square">
    <li>First item</li>
    <li>Second item</li>
    <li>Third item</li>
</ul>
```

Aqui está um exemplo do tipo de estilo da lista none:

```html
<p>Here is a list of unordered items:</p>    
<ul style="list-style-type: none">
    <li>First item</li>
    <li>Second item</li>
    <li>Third item</li>
</ul>
```



### Imagens

------

Imagens em HTML são elementos embutidos que podem ser colocados em um parágrafo. Para adicionar uma imagem, use a tag junto com o atributo para especificar o local da imagem.```src`

```html
<img src="/static/img/code.jpg">
```

Você pode usar o JavaScript para acionar um evento quando a imagem terminar de carregar.

```html
<img src="/static/img/code.jpg" onload="alert('image loaded')">
```

O redimensionamento da imagem pode ser feito usando os atributos de largura e altura de uma imagem ou, alternativamente, usando CSS:

```html
<img src="/static/img/code.jpg" width="100">

<img src="/static/img/code.jpg" style="width: 100px">
```

Ter um atributo "alt" definido para a imagem é útil para quando uma imagem não pôde ser carregada ou quando você deseja adicionar uma descrição da dica de ferramenta que será exibida ao passar o mouse sobre uma imagem.

```html
<img src="/static/img/code.jpg" style="width: 100px" alt="A picture of some code">
```

#### Tipos de imagem

Existem três tipos principais de formatos de imagem que você deve usar.

- Formatos sem perdas - úteis para quando você precisa de gráficos perfeitos em pixels, por exemplo, para logotipos. O formato mais comum é PNG. O PNG também suporta transparência alfa, o que significa que você pode usar qualquer plano de fundo desejado e sobrepor a imagem em cima desse plano de fundo.
- Formatos com perdas - úteis para exibir imagens ricas. Usar um formato sem perdas, como PNG, seria uma ordem de magnitude maior se usado em tais imagens. O formato mais comum usado nesta categoria é JPG.
- Formatos animados - úteis para mostrar imagens animadas curtas. O formato mais comum é o GIF, embora seja um formato muito antigo e amplamente suportado, com muitas desvantagens inerentes, como um limite de 256 cores em cada quadro e uma compactação ruim.

## Paramos AQUI ⚠️

### Estilos

------

CSS significa Cascading Style Sheets e é a linguagem visual da web. Com ele, podemos projetar a aparência das páginas HTML. O CSS nos permite separar os dados da página, codificados no HTML, e o estilo da página, codificado no CSS da página.

O motivo pelo qual o CSS é "em cascata" deve-se à maneira como define quais estilos usar. Os elementos HTML herdam seus estilos de maneira "em cascata", de acordo com um conjunto muito específico de prioridades, da menor para a maior:

- O padrão do navegador
- Estilos definidos na página
- Alguns estilos herdarão um estilo para seus filhos, por exemplo, qual fonte usar
- A última regra a ser definida na ordem de carregamento será a que entrará em vigor
- etc.

### Definindo CSS

CSS pode ser definido usando quatro métodos:

#### 1. Inline

Para definir um estilo CSS usando o método inline, use o `style`atributo HTML :

```html
<p>Isto é um parágrafo.</p>

<p style="font-family: sans-serif">Isto é um parágrafo com a fonte sans-serif. </p>
```

#### 2. Usando uma tag CSS

> Definir CSS embutido não é recomendado, evite-o o máximo que puder. 

Você sempre deve definir uma folha de estilo CSS e usar seletores para aplicar as folhas de estilo. 

Aqui está um exemplo:

```html
<!DOCTYPE html>
<head>
    <style>
        .nice {
            font-family: sans-serif;
        }
    </style>
</head>
<body>
    <p>Isto é um parágrafo.</p>

    <p class="nice">Isto é um parágrafo com a fonte sans-serif.</p>

</body>
```

#### 3. Usando uma folha de estilo diferente

Você pode definir uma folha de estilo CSS em um arquivo externo (geralmente anotado com a extensão .css) e carregá-la.

Aqui está um exemplo para definir a mesma classe CSS definida no exemplo anterior, mas em um arquivo chamado "style.css".

```html
.nice {
    font-family: sans-serif;
}
```

Para carregar o arquivo CSS, precisaríamos usar a tag HTML da seguinte maneira:``

```html
<link rel="stylesheet" href="nice.css">
```

Observe que a folha de estilo deve ser posicionada corretamente em relação à página HTML. Neste exemplo, o arquivo HTML e o arquivo CSS precisariam estar no mesmo diretório.

A tag do link deve ser posicionada dentro da seção da página HTML, assim:``

```html
<!DOCTYPE html>
<head>
    <link rel="stylesheet" href="nice.css">    
</head>
<body>
    <p>Isto é um parágrafo.</p>

    <p class="nice">Isto é um parágrafo com a fonte sans-serif.</p>

</body>
```

#### 4. Acesso programático (via JS)

Os elementos HTML têm o atributo `style` , o qual você pode usar para adicionar estilos programaticamente.

Por exemplo:

```html
<!DOCTYPE html>
<body>
    <p id="serif-text">Isto é um parágrafo.</p>

    <p class="nice" id="sans-serif-text">Isto é um parágrafo com a fonte sans-serif.</p>

    <script>
        var sansSerifText = document.getElementById("sans-serif-text");
        sansSerifText.style.fontFamily = "sans-serif";
    </script>
</body>
```

### Classes

As classes CSS são comumente usadas para definir um conjunto de estilos CSS e depois aplicá-las em um elemento HTML usando seletores. Para definir uma classe em uma folha de estilo CSS, use o **seletor de pontos**, da seguinte maneira:

```html
<style>
.nice {
    font-family: sans-serif;
}
</style>
```

Cada elemento HTML pode ter um conjunto de classes, ordenadas em uma ordem específica. Cada classe potencialmente adicionará um conjunto de definições de CSS de acordo com os estilos definidos na página. Neste pedaço de código, definimos uma regra CSS que será aplicada a todos os elementos que contenham a classe "nice". Isso significa que, uma vez que esse trecho de código tenha sido definido dentro da página HTML, o seguinte parágrafo HTML terá o estilo aplicado a ele:

```html
<style>
.nice {
    font-family: sans-serif;
}
</style>
<p class="nice">Isto é um parágrafo.</p>
```



### API classList do HTML5

O HTML5 introduziu uma nova maneira de editar a lista de classes de um elemento usando a `classList`. Cada elemento HTML retorna a coleção acessando o `element.classList`. A lista de classes permite adicionar, remover, alternar e verificar se um elemento contém uma classe específica.

Vamos ver um exemplo:

```html
<!DOCTYPE html>
<html>
<head>
    <style>
    .nice {
        font-family: sans-serif;
    }
    </style>
</head>
<body>
    <p id="mytext">My text</p>
    <script>
        var el = document.getElementById("mytext");
        el.classList.add("nice");    // add a classe nice ao paragrafo
        el.classList.remove("nice"); // remove a classe nice ao paragrafo
        el.classList.toggle("nice"); // add a classe nice ao paragrafo again, desde que não tenha atualmente
        // verifica se contém a classe nice.
        if (el.classList.contains("nice")) {
            alert("The element contains the 'nice' class.");
        }
    </script>
</body>
</html>
```

Como o HTML5 é um padrão relativamente novo, ele não é suportado em todos os navegadores. É seguro o suficiente para usar hoje, mas abaixo está a tabela de compatibilidade para o recurso: [http://caniuse.com/#search=classlist](https://caniuse.com/#search=classlist)

### Seletores

Os seletores CSS são extremamente úteis para definir uma consulta em um subconjunto dos elementos em uma página. A consulta nos permite fazer uma de duas coisas:

- declarar um estilo a ser aplicado no conjunto de elementos em uma folha de estilo CSS 
- ou receber uma lista de elementos HTML programaticamente de acordo com a consulta, usando o `querySelector`.

Aqui está um exemplo - se quisermos colorir todos os parágrafos do documento em azul, podemos simplesmente escrever:

```html
<style>
p {
    color: blue;
}
</style>
<p>I am blue</p>
<p class="example">I am also blue</p>
<p id="last" class="example">I am blue as well</p>
```

O seletor CSS "p" selecionará todos os "`<p>`" (parágrafos) na página.

Podemos adicionar restrições à consulta e aplicar um CSS diferente a alguns elementos usando um seletor mais específico. 

Para isto vamos então colorir todos os elementos "p" que possuem a classe "exemplo" com verde. 

> Observe que, neste exemplo, a ordem das definições de CSS não importa, pois o segundo seletor é mais específico - portanto, substituirá a definição de CSS menos específica.

```html
<style>
p.example {
    color: green;
}

p {
    color: blue;
}    
</style>
<p>I am blue</p>
<p class="example">I am green now</p>
<p id="last" class="example">I am also green now</p>
```

Podemos repetir o mesmo processo, mas desta vez adicionando um seletor de ID em vez do seletor de classe.

```html
<style>
p#last {
    color: red;    
}

p.example {
    color: green;
}

p {
    color: blue;
}    
</style>
<p>I am blue</p>
<p class="example">I am green now</p>
<p id="last" class="example">And now I am red</p>
```

Os seletores de CSS também suportam a separação por vírgula para aplicar o mesmo bloco de estilo a vários elementos. No exemplo abaixo, define-se cores para `h1`, `h2`e `h3`em azul e `h4`, `h5`e `h6`em vermelho.

```html
<style>
h1, h2, h3 {
    color: blue;
}

h4, h5, h6 {
    color: red;
}
</style>
<h1>h1 title</h1>
<h2>h2 title</h2>
<h3>h3 title</h3>
<h4>h4 title</h4>
<h5>h5 title</h5>
<h6>h6 title</h6>
```

### Seletores Descendentes e Filhos

Além de especificar um tipo de elemento, um ID e/ou um nome de classe, também podemos criar seletores que selecionam um filho específico apenas se ele estiver contido em uma hierarquia específica. 

Por exemplo, digamos que queremos colorir todas as  tags `<strong>` em qualquer parágrafo que tenha a classe "`strongblue`".

```html
<style>
.strongblue strong {
    color: blue;    
}
</style>
<p>This is the <strong>first</strong> sentence.</p>
<p class="strongblue">This is the <strong>second</strong> sentence.</p>
```

Existem dois tipos de seletores filhos:

- um seletor ancestral como o citado acima
-  e um seletor de filho direto (`>`), que seleciona **apenas o primeiro nível de hierarquia** no elemento pai que foi selecionado. 

Aqui está o mesmo código, mas com um seletor filho direto:

```html
<style>
.strongblue > strong {
    color: blue;    
}
</style>
<p>This is the <strong>first</strong> sentence.</p>
<p class="strongblue">This is the <strong>second</strong> sentence.</p>
```

Se o ``elemento tiver sido encapsulado em um link, esse seletor não funcionará, pois depende de um relacionamento pai-filho direto entre `.strongblue`e o `strong`elemento.

```html
<style>
.strongblue > strong {
    color: blue;    
}
</style>
<p>This is the <strong>first</strong> sentence.</p>
<p class="strongblue">This is the <a><strong>second</strong></a> sentence.</p>
```

### Métodos querySelector e querySelectorAll

HTML5 introduziu os novos métodos `document.querySelector`e `document.querySelectorAll` que nos permite executar os mesmos seletores e receber o primeiro elemento que corresponde ao seletor, ou uma lista de elementos, dependendo do método utilizado.

Vamos ver um exemplo:

```html
<p class="nice">This is a nice paragraph.</p>
<p class="nice">This is another nice paragraph.</p>
<p>This is a standard paragraph.</p>

<script>
    // this code colors the first nice paragraph in blue
    var firstNiceParagraph = document.querySelector(".nice");
    firstNiceParagraph.style.color = "blue";
</script>
```

### Pseudo-Classes

O HTML fornece pseudo-classes, classes que são definidas por padrão e nos permitem aplicar um estilo em:

1. Um elemento que está em um estado específico.
2. Um conjunto específico de elementos por sua hierarquia.

Discutiremos o primeiro nesta página e daremos exemplos para cada pseudo-classe. 

> Lembre-se de que não há como incluir pseudo-classes no CSS.

#### Links

Um `link` pode estar em um estado **não visitado** ou em um estado **visitado**. Um link não visitado é um `:link` que <u>não foi clicado</u>. Um link `:visited` é um link que <u>foi clicado</u>.

```html
<style>
a.special:link {
    color: green;
}

a.special:visited {
    color: red;
}
</style>

<p><a href="#">This is a standard link, it will become purple when clicked</a></p>
<p><a class="special" href="#">This is a special colored link and become red when clicked</a></p>
```

#### Hover

A pseudo classe CSS `:hover` pode ser usada para definir estilos para elementos HTML nos quais o usuário está <u>passando sobre</u> ao usar o mouse.

```html
<style>
p:hover {
    background-color: yellow;
}
</style>
<p>Paragraphs now have a yellow background when hovering over them.</p>
```

#### Active e Target

A pseudo classe CSS `:active` define os estilos a serem usados para um elemento que está sendo clicado no momento.

```html
<style>
a:active {
    font-weight: bold;    
}
</style>
<p>
    <a href="#first">First Section</a>
    <a href="#second">Second Section</a>
    <a href="#third">Third Section</a>
</p>
```

Navegar para uma seção específica da página também nos permite estilizar o elemento de destino.

```html
<style>
p:target {
    font-weight: bold;    
}
</style>
<p>
    <a href="#first">First Section</a>
    <a href="#second">Second Section</a>
    <a href="#third">Third Section</a>
</p>
<p id="first">This is the text of the first section.</p>
<p id="second">This is the text of the second section.</p>
<p id="third">This is the text of the third section.</p>
```

#### Focus

A pseudo-classe :focus define os estilos a serem usados para um elemento que é focado.

```html
<style>
input:focus {
    font-weight: bold;    
}
</style>
<form>
    <p><input type="text" value="First field"></p>
    <p><input type="text" value="Second field"></p>
    <p><input type="text" value="Third field"></p>        
</form>
```

### Propriedades tipográficas e fontes

Da mesma maneira que alteramos cores, podemos alterar o texto. Podemos definir fontes com o uso da propriedade `font-family`.

Podemos alterar a família de fontes que queremos utilizar em nosso documento para a família "sans-serif" (sem serifas), que contém, por exemplo, as fontes "Arial" e "Helvetica". Podemos também declarar que queremos utilizar uma família de fontes "monospace" como, por exemplo, a fonte "Courier".

```css
h1 {
  font-family: serif;
}

h2 {
  font-family: sans-serif;
}

p {
  font-family: monospace;
}
```

Em nossos projetos, as fontes não têm ornamentos, vamos declarar essa propriedade para todo o documento por meio do seu elemento `body`:

```css
body {
  font-family: "Arial", "Helvetica", sans-serif;
}
```

Temos outras propriedades para manipular a fonte, como a propriedade `font-style`, que define o estilo da fonte que pode ser: `normal` (normal na vertical), `italic` (inclinada) e `oblique` (oblíqua).

### Alinhamento e decoração

Uma das propriedades mais simples, porém muito utilizada, é a que diz respeito ao alinhamento de texto: a propriedade `text-align`.

```css
p {
  text-align: right;
}
```

O exemplo anterior determina que todos os parágrafos da nossa página tenham o texto alinhado para a direita. Também é possível determinar que um elemento tenha seu conteúdo alinhado ao centro ao definirmos o valor `center` para a propriedade `text-align`, ou então definir que o texto deve ocupar toda a largura do elemento aumentando o espaçamento entre as palavras com o valor `justify`. O padrão é que o texto seja alinhado à esquerda, com o valor `left`, porém é importante lembrar que essa propriedade propaga-se em cascata.

É possível configurar também uma série de espaçamentos de texto com o CSS:

```css
p {
  line-height: 3px; /* tamanho da altura de cada linha */
  letter-spacing: 3px; /* tamanho do espaço entre cada letra */
  word-spacing: 5px; /* tamanho do espaço entre cada palavra */
  text-indent: 30px; /* tamanho da margem da primeira linha do texto */
}
```

### Imagem de fundo

A propriedade `background-image` permite indicar um arquivo de imagem para ser exibido ao fundo do elemento. Por exemplo:

```css
h1 {
  background-image: url(sobre-background.jpg);
}
```

Com essa declaração, o navegador vai requisitar um arquivo `sobre-background.jpg`, que deve estar na mesma pasta do arquivo CSS onde consta essa declaração.

### Bordas

As propriedades do CSS para definirmos as **bordas** de um elemento nos apresentam uma série de opções. Podemos, para cada borda de um elemento, determinar sua cor, seu estilo de exibição e sua largura. Por exemplo:

```css
body {
  border-color: red;
  border-style: solid;
  border-width: 1px;
}
```

A propriedade `border` tem uma forma resumida para escrever os mesmos estilos que adicionamos acima, mas de uma maneira mais simples:

```css
body {
  border: 1px solid red;
}
```

Para que o efeito da cor sobre a borda surta efeito, é necessário que a propriedade `border-style` tenha qualquer valor diferente do padrão `none`.

### Espaçamento, margem e dimensões

Utilizamos a propriedade `padding` para **espaçamento**, `margin` para **margem**, `height` e `width` para alterar dimensões dos elementos. Vejamos cada uma e como elas diferem entre si.

#### Padding

A propriedade **padding** é utilizada para definir um espaçamento interno em alguns elementos (por espaçamento interno queremos dizer a distância entre o limite do elemento, sua borda, e seu respectivo conteúdo) e tem as subpropriedades listadas a seguir:

- padding-top
- padding-right
- padding-bottom
- padding-left

Essas propriedades aplicam uma distância entre o limite do elemento e seu conteúdo acima, à direita, abaixo e à esquerda respectivamente. Essa ordem é importante para entendermos como funciona a *shorthand property* do padding.

Podemos definir todos os valores para as subpropriedades do padding em uma única propriedade, chamada exatamente de `padding`, e seu comportamento é descrito nos exemplos a seguir:

Se passado somente um valor para a propriedade `padding`, esse mesmo valor é aplicado em todas as direções.

```css
p {
  padding: 10px;
}
```

Se passados dois valores, o primeiro será aplicado acima e abaixo (equivalente a passar o mesmo valor para `padding-top` e `padding-bottom`) e o segundo será aplicado à direita e à esquerda (equivalente ao mesmo valor para `padding-right` e `padding-left`).

```css
p {
  padding: 10px 15px;
}
```

Se passados três valores, o primeiro será aplicado acima (equivalente a `padding-top`), o segundo será aplicado à direita e à esquerda (equivalente a passar o mesmo valor para `padding-right` e `padding-left`) e o terceiro valor será aplicado abaixo do elemento (equivalente a `padding-bottom`).

```css
p {
  padding: 10px 20px 15px;
}
```

Se passados quatro valores, serão aplicados respectivamente a `padding-top`, `padding-right`, `padding-bottom` e `padding-left`. Para facilitar a memorização dessa ordem, basta lembrar que os valores são aplicados em **sentido horário**.

```css
p {
  padding: 10px 20px 15px 5px;
}
```

#### Margin

A propriedade `margin` é bem parecida com a propriedade `padding`, exceto que ela adiciona espaço após o limite do elemento, ou seja, é um espaçamento além do elemento em si. Além das subpropriedades listadas a seguir, há a *shorthand property* `margin` que se comporta da mesma maneira que a *shorthand property* do `padding` vista no tópico anterior.

- margin-top
- margin-right
- margin-bottom
- margin-left

Há ainda uma maneira de permitir que o navegador defina qual será a dimensão da propriedade `padding` ou `margin` conforme o espaço disponível na tela: definimos o valor `auto` para os espaçamentos que quisermos.

No exemplo a seguir, definimos que um elemento não tem nenhuma margem acima ou abaixo de seu conteúdo e que o navegador define uma margem igual para ambos os lados de acordo com o espaço disponível:

```css
p {
  margin: 0 auto;
}
```

#### Dimensões

É possível determinar as dimensões de um elemento, por exemplo:

```css
p {
  background-color: red;
  height: 300px;
  width: 300px;
}
```



## Position: static, relative, absolute e fixed

Existe um conjunto de propriedades que podemos utilizar para posicionar um elemento na página, que são `top`, `left`, `bottom` e `right`. Porém essas propriedades, por padrão, não são obedecidas por nenhum elemento, pois elas dependem de uma outra propriedade, a `position`.

A propriedade `position` determina qual é o modo de posicionamento de um elemento, e ela pode receber como valor: **static**, **relative**, **absolute** ou **fixed**. Veremos o comportamento de cada um deles, junto com as propriedades de coordenadas.

O primeiro valor, padrão para todos os elementos, é o **static**. Um elemento com posição `static` permanece sempre em seu local original no documento, aquele que o navegador entende como sendo sua posição de renderização. Se passarmos valores para as propriedades de coordenadas, eles não serão respeitados.

Um dos valores para a propriedade `position` que aceitam coordenadas é o **relative**. Com ele, as coordenadas que passamos são obedecidas em relação à posição original do elemento. Por exemplo:

```css
.logotipo {
    position: relative;
    top: 20px;
    left: 50px;
}
```

Os elementos em nosso documento que receberem o valor "logotipo" em seu atributo `class` terão 20px adicionados ao seu topo e 50px adicionados à sua esquerda em relação à sua posição original. Note que, ao definirmos coordenadas, estamos adicionando pixels de distância naquela direção, então o elemento será renderizado mais abaixo e à direita em comparação à sua posição original.

O próximo modo de posicionamento que temos é o **absolute**, e ele é um pouco complexo. Existem algumas regras que alteram seu comportamento em determinadas circunstâncias. Por definição, o elemento que tem o modo de posicionamento absolute toma como referência qualquer elemento que seja seu pai na estrutura do HTML cujo modo de posicionamento seja diferente de `static` (que é o padrão), e obedece às coordenadas de acordo com o tamanho total desse elemento pai.

Quando não há nenhum elemento em toda a hierarquia daquele que recebe o posicionamento `absolute` que seja diferente de `static`, o elemento vai aplicar as coordenadas tendo como referência a porção visível da página no navegador. Por exemplo:

**Estrutura HTML**

```html
<div class="quadrado"></div>
<div class="quadrado absoluto"></div>
```

**Estilos CSS**

```css
.quadrado {
    background-color: green;
    height: 200px;
    width: 200px;
}

.absoluto {
    position: absolute;
    top: 20px;
    right: 30px;
}
```

Seguindo o exemplo acima, o segundo elemento `<div>`, que recebe o valor "absoluto" em seu atributo `class`, não tem nenhum elemento como seu "pai" na hierarquia do documento, portanto ele vai alinhar-se ao topo e à direita do limite visível da página no navegador, adicionando respectivamente 20px e 30px nessas direções. Vamos analisar agora o exemplo a seguir:

**Estrutura HTML**

```html
<div class="quadrado relativo">
    <div class="quadrado absoluto"></div>
</div>
```

**Estilos CSS**

```css
.quadrado {
    background-color: green;
    height: 200px;
    width: 200px;
}

.absoluto {
    position: absolute;
    top: 20px;
    right: 30px;
}

.relativo {
    position: relative;
}
```

Nesse caso, o elemento que recebe o posicionamento absolute é "filho" do elemento que recebe o posicionamento `relative` na estrutura do documento, portanto, o elemento `absolute` vai usar como ponto de referência para suas coordenadas o elemento `relative` e se posicionar 20px ao topo e 30px à direita da **posição original** desse elemento.

O outro modo de posicionamento, **fixed**, sempre vai tomar como referência a porção visível do documento no navegador, e mantém essa posição inclusive quando há rolagem na tela. É uma propriedade útil para avisos importantes que devem ser visíveis com certeza.

### Um resumo de position

**static**

- Sua posição é dada automaticamente pelo fluxo da página: por padrão ele é renderizado logo após seus irmãos
- Não aceita um posicionamento manual (left, right, top, bottom)
- O tamanho do seu elemento pai leva em conta o tamanho do elemento static

**relative**

- Por padrão, o elemento será renderizado da mesma maneira que o static
- Aceita posicionamento manual
- O tamanho do seu elemento pai leva em conta o tamanho do elemento relative, porém sem levar em conta seu posicionamento. O pai não sofreria alterações mesmo se o elemento fosse static

**fixed**

- Uma configuração de posicionamento vertical (top ou bottom) e uma horizontal (left ou right) é obrigatória
- O elemento será renderizado na página na posição indicada. Mesmo que ocorra uma rolagem, o elemento permanecerá no mesmo lugar
- Seu tamanho não conta para calcular o tamanho do elemento pai, é como se não fosse elemento filho

**absolute**

- Uma configuração de posicionamento vertical (top ou bottom) e uma horizontal (left ou right) é obrigatória
- O elemento será renderizado na posição indicada, porém relativa ao primeiro elemento pai cujo position seja diferente de static ou, se não existir este pai, relativa à página
- Seu tamanho não conta para calcular o tamanho do elemento pai



## border-radius

Uma das novidades mais celebradas do CSS3 foi a adição de bordas arredondadas via CSS. Até então, a única forma de obter esse efeito era usando imagens, o que deixava a página mais carregada e dificultava a manutenção.

Com o CSS3 há o suporte a propriedade `border-radius` que recebe o tamanho do raio de arredondamento das bordas. Por exemplo:

```css
  div {
    border-radius: 5px;
  }
```



![img](https://www.caelum.com.br/apostila-html-css-javascript/img/css-avancado/border-radius.png)

Podemos também passar valores diferentes para cantos diferentes do elemento:

```css
  /* todas as bordas arredondadas com um raio de 15px */
  .a {
    border-radius: 15px;
  }

  /* borda superior esquerda e inferior direita com 5px
  borda superior direita e inferior esquerda com 20px */
  .b {
    border-radius: 5px 20px;
  }

  /* borda superior esquerda com 5px
  borda superior direita e inferior esquerda com 20px
  borda inferior direita com 50px */
  .c {
    border-radius: 5px 20px 50px;
  }

  /* borda superior esquerda com 5px
  borda superior direita com 20px
  borda inferior direita com 50px
  borda inferior esquerda com 100px */
  .d {
    border-radius: 5px 20px 50px 100px;
  }
```



![img](https://www.caelum.com.br/apostila-html-css-javascript/img/css-avancado/border-radius2.png)

## 5.7 CSS3: text-shadow

Outro efeito do CSS3 é o suporte a sombras em textos com `text-shadow`. Sua sintaxe recebe o deslocamento da sombra e sua cor:

```css
  p {
    text-shadow: 10px 10px red;
  }
```



![img](https://www.caelum.com.br/apostila-html-css-javascript/img/css-avancado/text-shadow1.png)

Ou ainda pode receber um grau de espalhamento (blur):

```css
  p {
    text-shadow: 10px 10px 5px red;
  }
```



![img](https://www.caelum.com.br/apostila-html-css-javascript/img/css-avancado/text-shadow2.png)

É possível até passar mais de uma sombra ao mesmo tempo para o mesmo elemento:

```css
  p {
    text-shadow: 10px 10px 5px red, -5px -5px 4px red;
  }
```

## box-shadow

Além de sombras em texto, podemos colocar sombras em qualquer elemento com `box-shadow`. A sintaxe é parecida com a do `text-shadow`:

```css
  box-shadow: 20px 20px black;
```



![img](https://www.caelum.com.br/apostila-html-css-javascript/img/css-avancado/box-shadow1.png)

Podemos ainda passar um terceiro valor com o blur:

```css
  box-shadow: 20px 20px 20px black;
```



![img](https://www.caelum.com.br/apostila-html-css-javascript/img/css-avancado/box-shadow2.png)

Diferentemente do `text-shadow`, o `box-shadow` suporta ainda mais um valor que faz a sombra aumentar ou diminuir:

```css
  box-shadow: 20px 20px 20px 30px black;
```



![img](https://www.caelum.com.br/apostila-html-css-javascript/img/css-avancado/box-shadow3.png)

Por fim, é possível usar a keyword **inset** para uma borda interna ao elemento:

```css
  box-shadow: inset 0 0 40px black;
```

![img](https://www.caelum.com.br/apostila-html-css-javascript/img/css-avancado/box-shadow4.png)



## Opacidade e RGBA

Desde o CSS2 é possível mudar a opacidade de um elemento para que ele seja mais transparente com o uso da propriedade `opacity`.

Veja esse exemplo com um parágrafo por cima de uma imagem:



![img](https://www.caelum.com.br/apostila-html-css-javascript/img/css-avancado/opacity1.png)

Colocamos um fundo preto e cor branca no texto. E se quisermos um efeito legal de transparência para deixar a imagem mostrar mais?



![img](https://www.caelum.com.br/apostila-html-css-javascript/img/css-avancado/opacity2.png)

É simples com a `opacity` que recebe um valor decimal entre 0 e 1:

```css
  p {
    opacity: 0.3;
  }
```

Repare como todo o elemento fica transparente, o fundo e o texto. E se quiséssemos o texto em branco opaco e o fundo com transparência? No CSS3, podemos usar outra técnica, a de definir uma cor de fundo com valor de opacidade específica.

No CSS3, além das cores hex normais (**#ffffff** pro branco), podemos criar cores a partir de seu valor RGB, passando o valor de cada canal (Red, Green, Blue) separadamente (valor entre 0 e 255):

```css
  /* todos equivalentes */
  color: white;
  color: #ffffff;
  color: rgb(255, 255, 255);
```

Porém, existe uma função chamada RGBA que recebe um quarto argumento, o chamado canal Alpha. Na prática, seria como a opacidade daquela cor (um valor entre 0 e 1):

```css
  /* branco com 80% de opacidade */
  color: rgba(255,255,255, 0.8);
```

No exemplo da foto, queríamos apenas o fundo do texto em preto transluzente (o texto não). Em vez do opacity, podemos fazer então:

```css
  p {
    background-color: rgba(0,0,0,0.3);
    color: white;
  }
```



![img](https://www.caelum.com.br/apostila-html-css-javascript/img/css-avancado/opacity3.png)

## 5.10 Prefixos

Muitos recursos do HTML5 e do CSS3 ainda são experimentais. Isso quer dizer que foram incluídos no rascunho da especificação mas ainda não são 100% oficiais. As especificações ainda estão em aberto e vai demorar algum tempo até elas serem fechadas.

Existem recursos mais estáveis e menos estáveis. Alguns já estão bastante maduros e há bastante tempo na spec, e não são esperadas mais mudanças. Por outro lado, alguns são bem recentes e talvez ainda possa haver mudança até a aprovação final da especificação.

Os navegadores desejam implementar os novos recursos antes mesmo da especificação terminar, para que os desenvolvedores possam começar a usar as novas propriedades e experimentá-las na prática. Entretanto, como a sintaxe final depois de aprovada pode ser diferente, os navegadores implementam as novas propriedades instáveis usando nomes provisórios.

A boa prática é pegar o nome da propriedade e colocar um **prefixo** específico do fabricante na frente. Quando a especificação ficar estável, tira-se esse prefixo e suporta-se a sintaxe oficial.

As bordas arredondadas, por exemplo, hoje são suportadas em todos os navegadores modernos com o nome normal da propriedade a `border-radius`. Mas até o Firefox 3.6, por exemplo, o suporte da Mozilla era experimental e a propriedade era chamada de `-moz-border-radius` nesse navegador. No Chrome até a versão 3, precisávamos usar o prefixo deles com `-webkit-border-radius`.

Os prefixos dos fabricantes mais famosos são:

- **-webkit-**: navegadores Webkit (Chrome, Safari, iOS, Android)
- **-moz-**: Firefox (Mozilla)
- **-ms-**: Internet Explorer (Microsoft)
- **-o-**: Opera

É preciso consultar tabelas de compatibilidade para saber qual navegador suporta qual propriedade e se é necessário usar prefixos para certas versões. Se quisermos o máximo de compatibilidade, precisamos colocar vários prefixos ao mesmo tempo:

```css
  p {
    /* Chrome até versão 3, Safari até versão 4 */
    -webkit-border-radius: 5px;

    /* Firefox até versão 3.6 */
    -moz-border-radius: 5px;
    /* Todas as versões modernas dos navegadores,
    incluindo IE e Opera que nunca precisaram de
    prefixo pra isso */
    border-radius: 5px;
  }
```

Nos casos de CSS3 que tratamos até agora (border-radius, text-shadow, box-shadow, rgba), todos os navegadores modernos já suportam sem uso de prefixos. Você só precisará deles se quiser suportar versões antigas (nesse caso, consulte as documentações para saber o que é necessário e quando).



## Gradientes

O CSS3 traz também suporte à declaração de gradientes sem que precisemos trabalhar com imagens. Além de ser mais simples, a página fica mais leve e a renderização fica melhor por se adaptar a todo tipo de resolução.

Existe suporte a gradientes lineares e radiais, inclusive com múltiplas paradas. A sintaxe básica é:

```css
  .linear {
    background: linear-gradient(white, blue);
  }

  .radial {
    background: radial-gradient(white, blue);
  }
```

Podemos ainda usar gradientes com angulações diferentes e diversas paradas de cores:

```css
  .gradiente {
    background: linear-gradient(45deg, #f0f9ff 0%, #cbebff 47%, #a1dbff 100%);
  }
```

### Prefixos

A especificação de gradientes já está em sua versão final e já é implementada sem prefixos em todos os browsers.

Mas, enquanto a especificação ainda estava em rascunho, antes de seu final, uma sintaxe diferente nos gradientes era usada. Isso quer dizer que versões mais antigas dos navegadores que suportavam gradientes esperam uma sintaxe diferente.

Como as especificações em rascunho são implementadas prefixadas nos navegadores, é fácil colocar essas regras com sintaxe diferente para esses navegadores. O problema é que o código fica grande e difícil de manter.

A versão atual da especificação suporta um primeiro argumento que indica a direção do gradiente:

```css
  .linear {
    background: linear-gradient(to bottom, white, blue);
  }
```

O código anterior indica um gradiente do branco para o azul vindo de cima **para baixo**. Mas na versão suportada antes do rascunho dos gradientes, o mesmo código era escrito com **top** ao invés de **to bottom**:

```css
  .linear {
    background: -webkit-linear-gradient(top, white, blue);
    background: -moz-linear-gradient(top, white, blue);
    background: -o-linear-gradient(top, white, blue);
  }
```

Pra piorar, versões bem mais antigas do WebKit - notadamente o Chrome até versão 9 e o Safari até versão 5 -, usavam uma sintaxe ainda mais antiga e complicada:

```css
  .linear {
    background: -webkit-gradient(linear, left top, left bottom,
      color-stop(0%, white), color-stop(100%, blue));
  }
```

Se quiser o máximo de compatibilidade, você terá que incluir todas essas variantes no código CSS.

### Geração de gradientes

É comum também a configuração de um `background` simples e sólido antes do gradiente, a ser usado pelos navegadores mais antigos. Como eles não entendem gradientes, usarão a cor sólida e terão um design adequado e usável. Os navegadores mais novos vão ler a regra do gradiente e ignorar a cor sólida (progressive enhancement):

```css
  .gradiente {
    background: #cbebff;
    background: linear-gradient(45deg, #f0f9ff 0%, #cbebff 47%, #a1dbff 100%);
  }
```

Uma ferramenta bastante útil e recomendada é o **Ultimate CSS Gradient Generator** da ColorZilla. Ela nos permite criar gradientes CSS3 visualmente como num editor de imagens. Além disso, já implementa todos os hacks e prefixos para navegadores diferentes. Há até uma opção que permite que enviemos uma imagem com o design de um gradiente e ele identifica as cores e gera o código correto.

http://www.colorzilla.com/gradient-editor/

## Transitions

Com as transitions, conseguimos animar o processo de mudança de algum valor do CSS.

Por exemplo: temos um elemento na posição `top:10px` e, quando passarmos o mouse em cima (:hover), queremos que o elemento vá para `top:30px`. O CSS básico é:

```css
  #teste {
    position: relative;
    top: 10px;
  }

  #teste:hover {
    top: 30px;
  }
```

Isso funciona, mas o elemento é deslocado de uma vez quando passamos o mouse. E se quisermos algo mais sutil? Uma animação desse valor mudando lentamente, mostrando o elemento se deslocando na tela? Usamos CSS3 Transitions.

Sua sintaxe possui vários recursos, mas seu uso é mais simples, para esse nosso caso, seria apenas:

```css
  #teste:hover {
    transition: top 2s;
  }
```

Isso indica que queremos animar a propriedade top durante 2 segundos.

Por padrão, a animação é linear, mas temos outros tipos para animações mais suaves:

- `linear` - velocidade constante na animação;
- `ease` - redução gradual na velocidade da animação;
- `ease-in` - aumento gradual na velocidade da animação;
- `ease-in-out` - aumento gradual, depois redução gradual na velocidade da animação;
- `cubic-bezier(x1,y1,x2,y2)` - curva de velocidade para animação customizada (avançado)

```css
  #teste:hover {
    transition: top 2s ease;
  }
```

Para explorar o comportamento dos tipos de animações disponíveis, e como criar uma curva de velocidade customizada para sua animação, existe uma ferramenta que auxilia a criação do `cubic-bezier`: http://www.roblaplaca.com/examples/bezierBuilder/

Podemos ainda usar mais de uma propriedade ao mesmo tempo, incluindo cores!

```css
  #teste {
    position: relative;
    top: 10px;
    color: white;
  }

  #teste:hover {
    top: 30px;
    color: red;
    transition: top 2s, color 1s ease;  
  }
```

Se quisermos a mesma animação, mesmo tempo, mesmo efeito para todas as propriedades, podemos usar o atalho **all** (que já é o valor padrão, inclusive):

```css
  #teste:hover {
    transition: all 2s ease;
  }
```

## 5.15 CSS3 Transforms

Com essa nova especificação, agora é possível alterar propriedades visuais dos elementos antes impossíveis. Por exemplo, agora podemos alterar o ângulo de um elemento, mostrá-lo em uma escala maior ou menor que seu tamanho padrão ou alterar a posição do elemento sem sofrer interferência de sua estrutura.

### Translate

```css
  .header {
    /* Move o elemento no eixo horizontal */
    transform: translateX(50px);
  }

  #main {
    /* Move o elemento no eixo vertical */
    transform: translateY(-20px);
  }

  footer {
    /* Move o elemento nos dois eixos (X, Y) */
    transform: translate(40px, -20px);
  }
```



![img](https://www.caelum.com.br/apostila-html-css-javascript/img/css-avancado/transform-translate.png)

### Rotate

```css
  #menu-departamentos {
    transform: rotate(-10deg);
  }
```



![img](https://www.caelum.com.br/apostila-html-css-javascript/img/css-avancado/transform-rotate.png)

### Scale

```css
  #novidades li {
    /* Alterar a escala total do elemento */
    transform: scale(1.2);
  }

  #mais-vendidos li {
    /* Alterar a escala vertical e horizontal do elemento */
    transform: scale(1, 0.6);
  }
```



![img](https://www.caelum.com.br/apostila-html-css-javascript/img/css-avancado/transform-scale.png)

### Skew

```css
  footer {
    /* Distorcer o elemento no eixo horizontal */
    transform: skewX(10deg);
  }

  #social {
    /* Distorcer o elemento no eixo vertical */
    transform: skewY(10deg);
  }
```



![img](https://www.caelum.com.br/apostila-html-css-javascript/img/css-avancado/transform-skew.png)

É possível combinar várias transformações no mesmo elemento, basta declarar uma depois da outra:

```css
  html {
    transform: rotate(-30deg) scale(0.4);
  }
```



## Bibliotecas CSS

Ao longo dos anos, muitas bibliotecas CSS e JavaScript foram introduzidas. Abaixo alguns exemplos de bibliotecas CSS que têm uma classificação alta no Google:

- Bootstrap, by Twitter ([[http://getbootstrap.com/]])
- Foundation, by Zurb ([[http://foundation.zurb.com/]])
- Pure CSS, by Yahoo ([[http://purecss.io/]])
- Bulma (based on the new CSS3 Flexbox specification - [[http://bulma.io/]])
- Skeleton ([[http://getskeleton.com/]])
- Semantic UI ([[http://semantic-ui.com/]])

## Guias de Referência

- **CSS** - https://www.w3c.br/divulgacao/guiasreferencia/css2/

- **HTML** - https://www.w3c.br/divulgacao/guiasreferencia/xhtml1/

