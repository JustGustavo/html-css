Aprendenmos o uso do `Border, Padding, Margin, e o outline`, só para refrescar a memoria , o `Border` é a borda que fica em volta do nosso box, o `padding` é o preenchimento ou espaço do border para dentro, e o `Margin` é espaço do border para fora, e também temos o `Outline` que é um tracejado que fica em volta do nosso border e dentro do nosso margin
```css
<style>
    h1 {
        background-color: lightgrey;
        height: 300px;
        width: 300px;
        border-width: 10px;
        border-style: solid;
        border-color: darkslategray;

        padding-top: 10px;
        padding-right: 10px;
        padding-bottom: 10px;
        padding-left: 10px;
        
        margin-top: 20px;
        margin-right: 20px;
        margin-bottom: 40px;
        margin-left: 20px;

        outline-width: 5px;
        outline-style: dashed;
        outline-color: salmon;

    }
    a{
        border-width: 10px;
        border-style: solid;
        border-color: red;

        padding-top: 10px;
        padding-right: 10px;
        padding-bottom: 10px;
        padding-left: 10px;
    }
</style>
```
esse é o CSS que fizemos na aula como explicaçao dos nossos `box-models`, note que , existe uma ordem na hora de declara cada direçao seja do padding ou margin, primeiro começamos com o `top` depois `right` vamos para o `bottom` e terminamos no `left`

agora vamos aprender simplificar essas configuraçoes usa `shorthands`
```css
<style>
h1{
border: 10px solid darkslategray;
outline: 5px dashed salmon;
padding: 10px 10px 10px 10px; 
margin: 20px 20px 40px 20px;
}

</style>
```
note que declaramos em apenas 4 linhas as mesmas configuraçoes vistas acimas, seguindo a ordem também que vimos acima,

também podemos colocar apennas 1 ou 2 valores na hora de declarar o padding ou margin

com apenas um valor por exemplo `10px` todos os lados  teram o mesmo  tamanho

se declaramos 2 valores, por exemplo `10px` e `20px`, ele esta declarando para o `top` e o`right`, porem nao ira modificar apenas o top e o right, no caso de 2 valores apenas, ele ira atribuir o primeiro tamanho declarao para o top e o bottom e o segundo valor para o right e o left

aprendemos também que para centralizar um box, temos que atribuir o valor `auto` no parametro `margin`, mas e se quisermos apenas centralizar 2 lados e quisermos que os outros tenham o valor que atribuimos? aprendemos também que isso é possivel

```css
<style>
h1{
    margin: 20px auto 40px auto;
}
</style>
```
agora teremos nosso  `left` e `right` centralizados com margin auto, e nosso `top` e `bottom` terao o valor de `20px` e `40px`

---

### Grouping Tags

Fomos introduzidos ao uso de `tags agrupadas`, ou `grouping tags` em html, que sao basicamente divs especiais, o uso das divs nao se tornou errado ainda pode ser usado normalmente, porem temos tags que funcionam do mesmo jeito e deixam nosso conteudo mais organizado 

basicamente as grouping tags que aprendemos ate agora foram `header, main, footer` essas principais basicamente sao, cabeçalho, conteudo principal e rodapé, junto a elas também aprendemos o uso do `nav, section, article, aside` que basicamente sao tagas que indicam nosso, are de NAVegaçao, nossa seçao, nosso artigom, e nosso "artigo secundario"

elas funcionam como divs, e ppodem ser usadas uma dentro das outras sem problemas, podem ser atribuidas id/class também a elas sem problemas

---

### box-shadow & border-radius

no finalzinho das aulas aprendemos a utilizaçao do `box-shadow` e do `border-radius`, que basicamente sao parametros em css que usamos para adicionar sombras ao noss conteudo e arredondamente das bordas

começando pelo box shadow que podemos configurar com mais facilidade pelo devtools como aprendemos na aula ou podemos usar seu comando padrao no css 

```css
box-shadow: 4px 4px 9px 0px black

```
aqui estamos indicando seus  `espaçamento,` o seu, `espalhamento`, o sua nitidez/borramento `blur` e no final estamos indicando sua cor, vale ressaltar que a sombra nao precisa ser extravagante ou exagerada , prefere-se uma sombra discreta e transparente, visto que o usuario ira nota-la mesmo ela nao estando extramemente destacada

vamos falar sobre o border raius, basicamente ele arredonda as bordas do local que ele foi puxado,
seu comando fica assim
```css
border-radius: 10px ;
border-radius: 10px 20px 30px 40px;
border-radius: 10px 0px;

```
note que adicionamos 3 tipos de border-radius, essas saos as 3 formas que podemos atribuir um border-radius ao nosso codigo, que é o primeiro, arredondando todos os lados igualmente, o segundo arredondando os lados cada um com um valor desejado
e o terceiro usando apenas 2 valores que ira atribuir 1 valor para 2 lados e o outro valor para os 2 lados restantes do arredondamento, possibilitando assim, variaçoes de arredondamento

