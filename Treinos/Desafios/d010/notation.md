### Variaveis em css

aprendemos usar variaveis em css para organizar melhor nosso codigo e deixalo mais facilmente editavel

para declararmos uma variavel em css usamos o `--` dentro do parametro `:root`
```css
:root {
--cor0:#c5ebd6;
--cor1:#83e1ad;
--cor3:#3ddc84;
--cor4:#2fa866;
--cor5:#1a5c37;
--cor6:#063d1e;

--font-padrao: Arial, Verdana, Helvetica, sans-serif;
--font-destaque: 'Bebas Neue', cursive;
--font-android: 'Android', cursive;
}
```
acima esta o exemplo das variaveis que fizemos para o desafio do capitulo 2,

so para relembrarmos também criamos um seletor global que ira editar globalmente todo meu site, que é o `*{}`
```css
*{
    margin: 0px;
    padding: 0px;
}
```
usamos isso para definir que tudo no nosso site nao ira ter padding nem margin por padrao,