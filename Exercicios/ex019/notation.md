### id e class em css

podemos atribuir uma `id` ou `class` a uma tag no nosso HTML para que essa mesma atribuiçao possa ser usada parar criar um `seletor especial` dentro do nosso CSS posibilitando estilizaçoes especificas, por exemplo quando temos mais de um H2 ou h2 em nosso conteudo e queremos estilizar cada um individualmente porem mantendo sua estilizaçao principal que seria a do seletor padraio de h1

a diferença entre nosso class e o id é que o id ele é de uso unico basicamente, vc pode adicionar varios, porem mesmo que funciona esta ERRADO segundo a documentaçao oficial da W3C.
ja o class nos podemos repeti-los em varias tags e criar

dentro do HTML eles sao definidos como class e id porem para chamarmos o class/id no css usamos o `#` para id e o `.` para
 class

 exemplos na pratica

vamos imaginar que nosso conteudo tem 3 H1, um titulo principal e 2 titulos de categoria, todos definidos com a tag h1,vamos estilizalo
 ```css
    h1 {
        font-size: 20px;
        text-align: Center;
        font-family: sans-serif;
    }
 ```
 note que , estamos estilizando diretamente nossa tag h1, entao nossas tres tags de h1 terao a mesma estlizaçao

 porem imaginemos que queremos apenas o titulo principal do nosso conteudo com aquela estilizaçao, e os titulos de categoria nos queremos de outra forma, é ai que entra o id e o class

 ```html
<h1>Criando Sites com HTML e CSS</h1>
<h1 class="categoria">Aprendendo HTML</h1>
<h1 class="categoria">Aprendendo CSS</h1>
 ```
 agora temos a class apenas os nossos titulos de categoria com um class definido, que também poderia ser um id, porem lembrando que so poderiamos colocar o id em apenas uma das tags de h1 pois o id so pode  ser usado um vez em cada documento html criado, mesmo que funcione com varios está ERRADO!!!

 Agora vamos estilizar individualmente nossas tags, nosso titulo principal ira ter a estilizaçao que definimos para o nosso seletor de h1, porem nossas tags que estao com um class definido irao ter sua propria estilizaçao

```css
.categoria {
    color: #3c805e;
    font-weight: bold;
    font-size: 10px;
    ...
}
```
note que usamos o `.` para criar nosso seletor especial `categoria` que é o nome da `class` que demos para nossas tags que queriamos estilizar fora do padrao definido para h1

também poderiamos fazer dessa forma usando id e class

 ```html
<h1 id="principal">Criando Sites com HTML e CSS</h1>
<h1 class="categoria">Aprendendo HTML</h1>
<h1 class="categoria">Aprendendo CSS</h1>
 ```

 ```css
.categoria {
    color: #3c805e;
    font-weight: bold;
    font-size: 10px;
    ...
}

#principal {
        font-size: 20px;
        text-align: Center;
        font-family: sans-serif;
    }
```
definimos um id para nosso titulo principal e continuamos usando o class no nosso titulo de categoria

também podemos usar id e class junto em uma mesma tag, por exemplo no nosso titulo , podemos colocar um class e um id
```html
<h1 id="principal" class="categoria">Criando Sites com HTML e CSS</h1>
```
nesse exemplo ele "teria" as 2 estilizaçoes tanto as definidas para o id principal como as definidas para o class categoria, porem predominariam as estilizaçoes do id , por que na hierarquia de definiçao o id foi atribuido primeiro