## Adicionando outras fonts com CSS

vamos aprender um pouco como adicionar outras fonts ao nosso projeto, vai ser um explicaçao simples e objetiva pois o processo também nao é dos nais complexos,

podemos importar fontes diretamente do site `Google Fonts` e como eu disse é bem simples fazer isso tudo que precisamos é ir no site escolher um fonta e clica no botao de usar fonte e ele vai criar um comando de import para voce colar no seu `CSS`

exemplo
```css
@import url('https://fonts.googleapis.com/css2?family=Kaushan+Script&display=swap');

```
aqui temos um exemplo de uma fonte simples importada, porem temos fontes com varios estilos dentro do google imagem, e nos podemos escolher quais estilos queremos ou nao importar

aqui vai um exemplo de font com todos os seus estilhos importados

```css
@import url('https://fonts.googleapis.com/css2?family=Kaushan+Script&family=Work+Sans:ital,wght@0,100;0,200;0,300;0,400;0,500;0,600;0,700;0,800;0,900;1,100;1,200;1,300;1,400;1,500;1,600;1,700;1,800;1,900&display=swap');

```
note que o comando de import ficou bem maior do que o do  nosso primeiro import, pois aqui temos a font `Work Sans` junto com todos os seus possiveis estilos

---
### fontes externas

e se nao tivermos a fontes que queremos ou que nosso cliente queira usar no google fonts, como fazemos para colocar esse font no nosso codigo? para resolver esse problema iremos usar um seletor especial no css chamado `@font-face` dentro dele iremos importar a fonte e definir o nome da sua  familia

vamos ao exemplo
```css
 @font-face {
    font-family: 'Love' ;
    src: url('fonts/love story ttf.ttf') format(truetype);
```
aqui ja temos todo o import pronto e funcionando. Onde temos o nosso `fonnt-family` dentro do nosso seletor é onde vamos definir como a fonte vai ser conhecida para usarmos ela no nosso css, nesse caso o nome da familia da fonte 
e `love`, logo quando formos atribuir esse font a estilizaçao do nosso `body,h1,` ou `p` , iremos usar o parametro  `font-family: 'Love';`

o segundo parametro, nosso ` src: url();` é onde iremos linkar a nossa font, que foi baixada esta dentro da past `fonts` na pasta principal do nosso code, entao para linkarmos nossa fonte, temos que indicara o nosso codigo a pasta em que o code está e o nome exato do seu arquivo e a sua extensao, deixando o codigo assim:
```css
src: url('fonts/love story ttf.ttf')
```
por ultimo mas nao menos importante, temos o nosso `format()` que vai nos fazer definir o tipo do arquivo nesse caso usaremos o `truetype` que é o format para os arquivos com a extensao `.ttf`, deixando o codigo final comop vimos la encima

depois da font importada podemos atribuir normalmente ao nosso conteudo
```css
h1 {
    font-family: 'Love', Times, serif;
    font-weight: normal;
}
```

```html
<!--Nota, aqui estao os outros tipos de type, para o nosso format().
tipos de format()
- opentype (otf)
- truetype (ttf)
- embedded-opnetype
- trutype-aat (apple advanced typograph)
- svg
-->
```
