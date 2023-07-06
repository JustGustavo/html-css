### Centralizando video com CSS

Vamos mostrar o codigo que foi usado antes de explicar qualquer coisa, levando em conta que o seletor `.video` é da `div` que definimos para nosso video do yotube
```css
.video {
    background-color: var(--cor5);
    margin: 0px -20px 30px -20px;
    padding: 20px ;
    padding-bottom: 56.5%; 
    position: relative;
}
.video > iframe {
    position: absolute;
    top: 5%;
    left: 5%;
    width: 90%;
    height: 90% ;
}
```
o mais importante desse codigo é os nossos `position` pois pelo que entedemos é ele que faz a magica acontecer

com os dois positions definidos, o video ira ficar todo bugado no codigo, junto com nosso background, porem com o `padding-bottom` de `56%`nosso background volta ao normal, e quando definimos embaixo nossa position para `absolute` temos a possibilitade de editar noss `leftm` e `right` e tbm nos da a possibilidade de mudar seu `widht` e `heigt` que nesse caso esta em 90% para conseguirmos ver nosso background