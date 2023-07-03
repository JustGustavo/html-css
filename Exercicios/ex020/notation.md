## Pseudo classes

vamos falar um pouco sobre pseudoclasses de forma simples e objetiva

como  vimos no decorres das aulas aprendemos que quando queremos chamar um id ou class no css usamos o `#` e o `.`
para utilizarmos de uma pseud-classe no css vamos usar os
dois pontos `:`

vamos usr de exemplo o `hover` que é uma pseud-classe que faz com que aja uma intereçao quando passamos o mouse na are determinada pelo hover

no exemplo também usaremos as `div` porém aprenderemos sobre elas mais para frente

exemplo na pratica
```css
div:hover {
    color: red;
}
```
essa linha de codigo que escrevemos esta definindo que dentro da nosa `div` tera a pseudoclasse hover, que indica que todo elemendo dentro de nossa `div` ira mudar a cor para vermelho quando passarmos o mouse por cima dela

outra coisa que podemos fazer, que também sera explicado melhor mais a frente nas aulas, é criar um display interativo, como por exemplo , fazer aparecer um conteudo na tela que estava escondido quando colocamos o mouse encima de uma determinada are do conteudo, tudo isso usando da pseudo-classe `hover`
```html
<body>
    <h1>Exemplo de hover</h1>
    <p>Passe o mouse sobre o texto abaixo</p>
    <div>
        passe o mouse aqui
        <p>TEXTO ESCONDIDO...</p>
    </div>
    <p>Fim do Exemplo</p>

</body>
```
```css
div > p {
    display: none;
}
div:hover > p {
    display: block;
    color: white;
    background-color: red;
    width: 300px;

    /*APENAS LEMRANDOQ QUE ALGUNS ELEMENTOS DESSE CODIGO NOS SO IREMOS APRENDER MAIS A FRENTE EM NOSSAS AULAS, USAREMOS AQUI APENAS COMO INTUITO DE EXPLICAÇAO*/
}
```
note que em nosso HTML, temos um paragrafo escrito `texto escondido`, esse é o conteudo que queremos mostrar na tela quando o usuario passar o mouse por cima da frase `passe o mouse aqui`. Agora vamos explicar como isso tudo ira funcionar em nosso codigo css

note que temos um seletor definido assim `div > p` esse seletor indica que queremos estilizar ou definir parametros APENAS para a tag p que esta dentro de nossa div e nao para todas as tags p como também logo abaixo temos a configuraçao da interaçao, que também esta definiar APENAS para nossa tag P dentro da div

```css
div > p {
    display: none;
}

```
esste comando esta indicando que o conteudo da nossa tag p dentro da nossa div, nao deve ser mostrado, ou seja simplesmente ele nao existira na tela do usuario

```css
div:hover > p {
    display: block;
    color: white;
    background-color: red;
    width: 300px;
}
```
ja essa segunda linha, esta definindo um `hover` para nossa tag p, e logo abaixo esta indicando que ela deve mostrar o conteudo na tela, ou seja quando o usuario passar o mouse por cima do `PASSE O MOUSE AQUI` nossa tag p que esta configurada para nao ser mostrada inicialmente , ira mostrar seu conteudo na tela

aprendemos  também usar a pseudoclasse ` active e visited` e a funçao deles é, quando usamos a pseudoclasse `active` nos possibilitamos a estilizaçao ou  interaçao de uma parte do conteudo quando ela estiver ativa, no caso do exemplo que usamos na aula que foram links, o `active` ira funcionar quando clicarmos no link

exemplo
```css
a:active {
    color: yellow;
}
``` 
quando clicarmos no nosso link ele ira ficar amarelo por um momento antes de nos levar para o site do link

temos tbm o `visited` que nos posibilita editar , no caso do exemplo, os links do site que ja visitamos, note que quando ja visitamos um site o link dele fica destacado em violeta, nesse nosso caso iremos usar o `visited` para mudara  cor dos links de sites visitados para `darkred`

```css
a:visited {
    color: darkred;
}
```
---

## Pseudo Elementos

de forma rustica, é uma outra forma de acrescentar elementos ou conteudo ao nosso site,

no caso do exemplo vamos usar o `after` e o `before` para explicar os `pseudo elementos` que diferente das `pseudo classes` eles sao representado pelo uso do 2 pontos 2 vezes `::`

exemplo na pratica
```css
a::before {
    content: '⇒';
}

a::after {
    content: '⇐';
}
```

aqui ja temos escrito os 2 pseudo elementos que explicaremos, basicamente o `before` juntamente com o parametro `content` ira adicionar algo ANTES do nosso link no caso do exemplo.
e o `after` junto com o `content` ira adicionar algo depois do link

que também, no caso do nosso exemplo será uma seta de cada lado