# Curso CSS3

> Este repositório contém o que eu estou aprendendo no curso de CSS3. Nele possui exemplos de comandos e também projetos para praticá-los.

## Projetos

Acesse os projetos feitos utilizando o css.

* <a href="https://github.com/WellingtonGouv/curso-CSS3/tree/main/Projetos/Projeto%20Anna%20Bella"> Projeto Anna Bella </a>
* <a href="https://github.com/WellingtonGouv/curso-CSS3/tree/main/Projetos/Projeto%20TecBlog">Projeto TecBlog </a>

## Introdução

O CSS3 é a terceira versão do CSS (Folha de Estilo em Cascata), que tem como função definir estilos para páginas web. Com ele, podemso customizar elementos HTML, como adicionar imagens, backgrounds, fontes, cores, entre muitos outros.

## Conteúdo

No CSS3 podemos realizar as formatações de três maneiras:

* External Style Sheet
* Internal Style Sheet
* Inline Style

No Inline Style, aplicamos a formatação diretamente no elemento, na Internal Style Sheet, colocamos o estilo dentro do código, enquanto no External Style Sheet, criamos um arquivo só para as formatações(recomendado).

### Inline Style

```html
<h1> Estilo CSS (Cascading Style Sheets)</h1>
<p style="color:orange">
    Bacon ipsum dolor amet spare ribs ham biltong shankle 
    jerky, rump meatloaf salami.
</p>
<p style="color: green"> 
    Bacon ipsum dolor amet spare ribs ham biltong shankle 
    jerky, rump meatloaf salami.
</p>
```

#### Resultado

<img src="Prints Exemplos\inline_exemplo.png">

***

### Seletores

Podemos utilizar seletores para a estilização, a estrutura deles é formada pela tag HTML que desejamos formatar e as propriedades que desejamos estilizar.

Exemplo(Internal Style Sheet):

```html
<style type="text/css">
    p {
        color: red;
    }
    h1 {
        color: blue;
    }
</style>
```

#### Resultado

<img src="Prints Exemplos\seletores_exemplo.png">

***

### Classes e IDs

Um Id é um identificador, utilizamos para definir a estilização de um único intem. Por outro lado, temos as Classes, que podem ser usadas para estilizar vários elementos.

Exemplos:

```html
<style type="text/css">
    /*Classe para definir cor azul*/
    .azul {
        color: blue;
    }
    /*Id principal*/
    #principal {
        background: orange;
    }
</style>
```

```html
<body id="principal">
    <h1> Estilo CSS (Cascading Style Sheets)</h1>
    <p class="azul">
        Bacon ipsum dolor amet spare ribs ham biltong shankle 
        jerky, rump meatloaf salami.
    </p>
    <p class="azul"> 
        Bacon ipsum dolor amet spare ribs ham biltong shankle 
        jerky, rump meatloaf salami.
    </p>
</body>
```

#### Resultado

<img src="Prints Exemplos\classes_ids_exemplo.png">

***

### Div e Span

A Div é uma divisão que pode ser utilizada para agrupar elementos. Por padrão, ela é um elemento do tipo block, ou seja, ocupa toda a largura da tela.
Já o Span, agrupa os elementos linha por linha, não ocupando a tela toda.

```html
<style type="text/css">
    #conteudo {
        background: red;
    }
    #rodape {
        background: yellow;
    }
    .produto {
        background: gray;
        /*Margem*/
        margin: 10px; 
    }
    .azul {
        background: blue;
    }
</style>

```

```html
<div id="conteudo">
    <div class="produto">
        Produto 1
    </div>
    <div class="produto">
        Produto 2
    </div>
    <div class="produto">
        Produto 3
    </div>
</div>
<div id="rodape">
    Todos os <span class="azul">direitos</span> reservados
</div>
```

#### Resultado

<img src="Prints Exemplos\div_span_exemplo.png">

***

### Bordas

Como o nome ja diz, podemos utilizar bordas nas tags html. Para criar uma borda, definimos sua espessura, seu estilo e a cor. Podemos fazer de duas maneiras: <br>
Definindo suas característica em uma linha só:

```css
border: 5px solid red;
```

Definindo cada característica separadamente:

```css
border-color: blue yellow green orange;
border-width: 15px;
border-style: outset;
```

Definir as características da borda separadamente, nos dá a vantagem de definir cada lado da borda.<br>

#### Resultado

<img src="Prints Exemplos\bordas_exemplo.png">
Para mais exemplos de estilos de bordas, podemos acessar esse <a href="https://www.w3schools.com/css/css_border.asp">link</a>.

***

### Fontes e Cores

Podemos definir as cores no css de várias maneiras, para as cores mais simples, podemos simplismente escrever o nome delas.
<br>
Exemplo:

```css
color : red;
```

Para cores mais complexas, podemos utilizar seu código no formato hexadecimal, como no exemplo a seguir:

```css
color: #AB11CD;
```

Também, podemos utilizar seu código rgb da seguinte maneira:

```css
color: rgb(255, 0, 255);
```

#### Resultado

<img src="Prints Exemplos\cores_exemplo.png">


Podemos definir, também, as fontes para os nossos textos, definindo o tamanho e também a família da fonte. Ao escolher a família da fonte, estamos definindo uma prioridade, pois se o usuário não possuir aquela fonte, ele passa para a próxima até uma fonte genérica.

```css
.formatacao {
    font-size: 20px;
    font-family: "Times New Roman", Times, serif;
}
```

#### Resultado

<img src="Prints Exemplos\fontes_exemplo.png">

***

### Tamanho de textos

Podemos definir o tamanho dos nossos textos, utilizando essas 3 formas. Podemos definir por pixels, que é uma forma fixa.

```css
font-size: 60px;
```

De maneira relativa, podemos utilizar % ou 'em' para definir o tamanho do texto de acordo com o container pai.

```css
font-size: 2em;
font-size: 50%;
```

Ao definirmos o tamanho do conteiner pai com 60px, uma fonte de tamanho 2em seria o dobro, ou seja, 120px, enquanto 50% seria a metade, que é 30px.

#### Resultado

<img src="Prints Exemplos\tamanho_textos_exemplo.png">

***

### Estilos de textos

Para definir os estilos dos textos, podemos fazer de diversas maneiras, para escrever um texto em negrito, podemos escrever 'bold' ou um número de 100 a 900 para definir o nível, por exemplo:

```css
font-weight: 900;
```

Para escrever um texto em itálico, podemos utilizar o seguinte código:

```css
font-style: italic;
```

Para colocar linhas no textos, podemos utilizar destas 3 formas:

```css
text-decoration: underline;
text-decoration: overline;
text-decoration: line-through;
```

Além disso, podemos realizar essas formatações de uma só vez, podendo agrupar essas características em uma linha.

```css
font: bold 40px 'Times New Roman', Times, serif;
```

#### Resultado

<img src="Prints Exemplos\estilo_textos_exemplo.png">

***

### Cores e Imagens de fundo

Para definirmos um background para o nosso site, podemos utilizar cores e imagens. Para elas, podemos definir várias características na estilização, como a repetição da imagem, a posição dela na tela, entre outros.<br>
Definindo imagem como background:

```css
background-image: url("imagens/homemaranha.png");
```

Definindo a repetição da imagem na tela:

```css
/*repeat-x, repeat-y, no-repeat, repeat*/
background-repeat: no-repeat;
```

Definindo se a imagem segue o scroll ou não:

```css
/*scroll, fixed*/
background-attachment: fixed;
```

Definindo posição da imagem na tela:

```css
/*
  primeiro valor: left, center, right
  segundo valor: top, centerm bottom
*/
background-position: bottom right;
```

Podemos também, definir tudo isso de uma vez só:

```css
background: blue url("imagens/homemaranha.png") no-repeat fixed center top;
```

#### Resultado

<img src="Prints Exemplos\background_exemplo.png">

***

### Css Externo

Podemos centralizar todos os estilos do nosso site em um lugar só. Ao utilizarmos de um arquivo .css e o referenciando, todos os sites utilizarão os estilos contidos nele. Exemplo no arquivo estilo.css:

```css
.texto{
    color: red;
    background: orange;
}
```

Referenciação no arquivo html:

```css
<link rel="stylesheet" type="text/css" href="estilo.css">
```

#### Resultado

<img src="Prints Exemplos\css_externo_exemplo.png">

***

### Modelo de caixa

As tags html se comportam como caixas, com isso, podemos atribuir diversos estilos nelas, como margens e bordas.
Definindo espaçamentos:

```css
padding-top: 20px;
padding-right: 20px;
padding-bottom: 20px;
padding-left: 20px;
```

Definindo margens:

```css
margin-top: 20px;
margin-right: 20px;
margin-left: 20px;
margin-bottom: 20px;
```

#### Resultado

<img src="Prints Exemplos\modelo_caixa_exemplo.png">

***

### Elementos flutuantes

Podemos usar elementos flutuantes para fazer com que essas caixas que nós vimos "flutuem" no site. Com isso, podemos fazer com que elas fiquem na mesma linha, uma em cima da outra, etc.

```css
float: left;
```

Utilizamos do `clear` para que o código seguinte não pegue as características de flutuação.

```css
clear: both;
```

#### Resultado

<img src="Prints Exemplos\elemento_flutuante_exemplo.png">

***

### Elementos flutuantes na prática

Com os elementos flutuantes, podemos fazer diversas coisas. Uma delas, é um site de noticias com uma galeria de fotos, como no exemplo a seguir.

<img src="Prints Exemplos\elemento_flutuante_pratica_exemplo.png">

***

### Elementos bloco

Podemos dividir dividir os elementos html em dois grandes grupos: o grupo Inline, o grupo Block e o grupo Inline-block que é uma mistura dos dois. <br>
Os elementos do tipo bloco ocupam toda a largura da tela, ou seja, quando temos mais de um bloco, eles ficam um embaixo do outro. <br>
Exemplo:

```css
display: block;
```

Já o elemento do tipo inline, ocupam somente o espaço do seu conteúdo, ou seja, quando temos mais de um, eles podem ficar na mesma linha. <br>
Exemplo:

```css
display: inline;
```

#### Resultado

<img src="Prints Exemplos\elemento_bloco_exemplo.png">

***

### Posicionamentos (Estático e Relativo)

Podemos mudar o posicionamento dos elementos html. Por padrão, algumas tags tem posicionamento estático, mas podemos mudá-las para relativo, atribuindo sua posição top, bottom, left e right a partir da posição inicial. <br>
Exemplo:

```css
position: relative;
top: 20px;
left: 80px;
```

#### Resultado

<img src="Prints Exemplos\posicionamento_relativo_exemplo.png">

***

### Posicionamentos (Absotuluto e fixo)

Assim como os posicionamentos estático e relativo, também temos o absoluto e o fixo. <br>
O posicionamento absoluto, faz com que o elemento fique parado na posição atribuída em relação ao conteiner, ou seja, o elemento fica no lugar quando usamos o scroll. <br>
O posicionamento fixo, fixa o elemento na sua posição definida em relação à tela, ou seja, se usarmos o scroll o elemento se movimenta junto.

Exemplo:

```css
.absolute {
    border: 1px solid red;
    background: #f2f2f2;
    position: absolute;
    top: 80px;
    right: 20px;
}
```

```css
.fixed {
    border: 1px solid red;
    background: #f2f2f2;
    position: fixed;
    right: 10px;
    bottom: 0px;
}
```

#### Resultado

<img src="Prints Exemplos\posicionamento_fixo_absoluto_exemplo.png">

***

### Sobrepondo elementos

Podemos sobrepor elementos de uma maneira muito simples. Utilizando o `z-index` e o maior número atribuído ficará sobreposto aos conteúdos com o menor número. <br>
Exemplo:

```css
z-index: 1;
```

#### Resultado

<img src="Prints Exemplos\sobrepor_elemento_exemplo.png">

***

### Formatando links

Podemos estilizar os links do nosso site. Os links possuem 4 estados: visitado, não visitado, hover e ativo. <br>
Formatamos os links visitados da seguinte maneira:

```css
a:visited {
    color: #c0c0c0;
}
```

Para os links não visitados, fazemos assim:

```css
a:link {
    color: #b9c941;
}
```

O hover é a formatação que aparece quando passamos o mouse em cima do link, ela pode ser feita da seguinte maneira:

```css
a:hover {
    color: #fff;
    background: #6d790f;
}
```

O link ativo aparece quando clicamos e seguramos o mouse em cima do link. Podemos formatá-lo assim:

```css
a:active {
    color: red;
}
```

#### Resultado

<img src="Prints Exemplos\formatando_links_exemplo.png">

***