# Curso CSS3
> Este repositório contém o que eu estou aprendendo no curso de CSS3. Nele possui exemplos de comandos e também projetos para praticá-los.


## Introdução
O CSS3 é a terceira versão do CSS (Folha de Estilo em Cascata), que tem como função definir estilos para páginas web. Com ele, podemso customizar elementos HTML, como adicionar imagens, backgrounds, fontes, cores, entre muitos outros.

## Conteúdo
No CSS3 podemos realizar as formatações de três maneiras:
* External Style Sheet
* Internal Style Sheet
* Inline Style 

No Inline Style, aplicamos a formatação diretamente no elemento, na Internal Style Sheet, colocamos o estilo dentro do código, enquanto no External Style Sheet, criamos um arquivo só para as formatações(recomendado).

### Inline Style

```
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
#### Resultado:
<img src="Prints Exemplos\inline_exemplo.png">


### Seletores

Podemos utilizar seletores para a estilização, a estrutura deles é formada pela tag HTML que desejamos formatar e as propriedades que desejamos estilizar.

Exemplo(Internal Style Sheet):

```
<style type="text/css">
    p {
        color: red;
    }
    h1 {
        color: blue;
    }
</style>
```
#### Resultado:
<img src="Prints Exemplos\seletores_exemplo.png">

### Classes e IDs
Um Id é um identificador, utilizamos para definir a estilização de um único intem. Por outro lado, temos as Classes, que podem ser usadas para estilizar vários elementos. 

Exemplos:
```
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
```
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
#### Resultado:
<img src="Prints Exemplos\classes_ids_exemplo.png">

### Div e Span
A Div é uma divisão que pode ser utilizada para agrupar elementos. Por padrão, ela é um elemento do tipo block, ou seja, ocupa toda a largura da tela.
Já o Span, agrupa os elementos linha por linha, não ocupando a tela toda.

```
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
```
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

#### Resultado:
<img src="Prints Exemplos\div_span_exemplo.png">