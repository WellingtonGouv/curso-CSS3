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

<img src="Prints Exemplos\seletores_exemplo.png">