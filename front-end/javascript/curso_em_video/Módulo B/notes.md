# Aula 05 - Variáveis e tipos primitivos

## Comentários

```
// Comentários de uma única linha

/*
    Comentários com mais de uma linha
*/
```

## Variáveis e tipos primitivos

- Podem começar com letra, $ ou _
- Não podem começar com números
- É possível usar letras ou números
- É possível usar acentos e símbolos
- Não podem conter espaços
- Não podem ser palavras reservadas

## Dicas
- Maiúsculas e minúsculas fazem diferença
- Tente escolher nomes coerentes para as variáveis
- Evite se tornar um 'programador alfabeto' ou um 'programador contador'

> Variáveis servem para gente guardar **dados**.

### Tipos primitivos
- number (5; 18; -12; 0.5;)
    - Infinity
    - NaN
- string ("Google"; 'Javascript'; \`Maria\`;)
- boolean (true; false;)
- null
- undefined
- object
    - Array
- function

> Podemos usar o `typeof` para saber o tipo primitivo de uma variável.

<br>

# Aula 06 - Tratamento de dados

## String > Número
- Para converter uma string em um número, usamos o `Number.parseInt` ou `Number.parseFloat`.
> Number.parseInt(string)

> Number.parseFloat(string)

Com as versões mais recentes do JS podemos utilizar apenas o `Number`.
> Number(string)

## Número > String
- Para converter um número em uma string, usamos o `String(número)` ou `número.toString`.

## Formatando strings

> Concatenação
```
var nome = 'Maria';
'Eu estou aprendendo ' + nome + '!';
```

> Template string
```
var nome = 'Maria';
`Eu estou aprendendo ${nome}!`;
```

> Atributos de string
- .length
- .toUpperCase()
- .toLowerCase()

## Formatando números

> toFixed(número)
```
var numero = 10.5;
numero.toFixed(2);
```

> toLocaleString()
```
var numero = 1545.5;
numero.toLocaleString('pt-BR', {style: 'currency', currency: 'BRL'});
//R$ 1.545,50
```