## Fontes em CSS

Aprendemos que, a escolha de uma fonte é a parte mais importante do nosso sitre, pois se simplesmente jogarmos uma fonta qualquer pode gerar problemas para o usuario.

e dai que aprendemos sobre a anatomia das fontes e que cada uma tem sua caracteristicas

### tipos de fontes

existems 4 tipos de fontes que aprendemos
`Serifas, Sans-serif, MonoEspaçadas, HandWiriting e display`

vamos explicar como cada uma funciona

### Fontes-serifadas

As fontes serifadas, sao fontes compostas de elementos em suas letras chamadas serifas que pode ser encontradas na parte superior ou inferior de uma letra ou glifo, usada para facilitar a leitura em certas ocasioes

porem temos que ter cautela, pois em certos casos
fontes com serifas, nao vao ser tao bem vindas, e sim a proxima que explicaremos que sao as fontes sem-serifas
ou `Sans-serif`

---

### Fontes Sem serifa

Como o proprio nome ja diz, sao fontes que nao possuem serifa,
e em certas ocasioes como em locais com pouco espaços para as letras, ou que elas tenham que ser muito pequenas, a fonte `sans-serif` sera melhor para a leitura

outra caracteristica que a fonte `sans-serif` tem que as outras fontes podem ou nao ter sao a familia tipografica da fonte que consiste na forma do glifo, podendo ser as que aprendemos `Light, Normal, seminegrito, negrito, extranegrito`

---

### Fontes monoespaçadas
nao temos muito o que explicar sobre essa fonte, ela é uma fonte sem serifa que como o nome diz ela é `monoespaçada` todos os seus glifos/letras terao o mesmo tamanho e ocuparam o mesmo espaço

---

### Fontes handwriting
Sao fontes scripitadas, fontes que o computador tenta replicar para se parecer com a escrita humana

---

### Fontes Display

Fontes de festa ou que levam a um filme como por exemplo
a logo do filme jurassic park

---

### Simplifcando o nosso CSS

vamos falor um pouco de um parametro que so aprenderemos mais pra frente


como falamos sobre as familias tipograficas que nem todas as fontes tem, temos as formas de declarar ela dentro do css

exemplo
```css
h1 {
 font-family: 'Work Sans', sans-serif;
 font-weight: bolder;
 font-size: 3em;
 font-style: italic;
}
```
Basicamente aqui estamos definindo como nosso `h1`, vai ser formatado, nesse caso ele ter a font `Work sans` `Sans-serif`
que nos nao temos naturalmente no nosso computador mas que vamos aprender usa-la mais pra frente, pois nesse exemplo ela é quem aceita o tipo de estilizaçao que aplicamos a ela pois nem todas as fontes aceitam!!!

definimos que o peso dela o `font-weight` vai ser bolder ou como explicamos vai ser `negrito`, seu `font-size` vai ser 3em
ou 3x o valor padrao da letra como é na maioria das vezes, e seu `font-style` via ser italic

Como dissemos antes nao sao todas as fontes que aceitam esse tipo de formataçao por isso que nesse caso estamos usando a `Work sans`

mas o que queremos explicar mesmo é que todo esse codigo pode ser simplificado em uma unica linha. Porem temos que seguir uma ordem, nos usaremos o parametro `font:` e dentro dele nos vamos definir cada uma das formataçoes porem seguindo a seguinte ordem 1 --> `font-style` 2 --> `font-weight` 3 --> `font-size` 4 --> `font-family`
1
o codigo final ira ficar assim

```css
h1 {
    font: italic bolder 3em 'Work Sans' sans-serif;
}
```
dessa forma teremos o mesmo resultado do primeiro codigo, porem usando apenas 1 linha, temos que ter cuidado para nao colocar nada errado, pois o codigo tem que ser escrito na ordem correta que foi citada acima

```html
<!--Nota, iremos aprender mais para frente 
outras simplificaçoes de codigo, porem 
vale ressaltar que nao a simplifcaçao como
esta para tudo-->

```
---
### Alinhamento de texto com CSS

Essa vai ser uma explicaçao simples e objetiva, basicamente podemos alinha textos a direita, a esquerda, no centro, ou justificar que ira alinhar  igualmente nas duas direçoes

também temos um comando chamaod `text-ident` que ira adicionar identaçao ao começo de um paragrafo como vemos em livros ou quando escrevemos

```css
text-align: center;
text-align: justify;
text-align: left;
text-align: right;
text-indent: 20px;
```
aqui estao todos os comandos que aprendemos nessa aula







