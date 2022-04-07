# Aula 05 - Variáveis e tipos primitivos

## Comentários

```javascript
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
```javascript
var nome = 'Maria';
'Eu estou aprendendo ' + nome + '!';
```

> Template string
```javascript
var nome = 'Maria';
`Eu estou aprendendo ${nome}!`;
```

> Atributos de string
- .length
- .toUpperCase()
- .toLowerCase()

## Formatando números

> toFixed(número)
```javascript
var numero = 10.5;
numero.toFixed(2);
```

> toLocaleString()
```javascript
var numero = 1545.5;
numero.toLocaleString('pt-BR', {style: 'currency', currency: 'BRL'});
//R$ 1.545,50
```

# Aula 07 - Operadores (parte 1)

## Arítimeticos

São operadores binários, que precisam de dois operandos. Por exemplo: 5 + 2.
> '+' | '-' | '*' | '/' | '%' | '**'

Exemplos:
```javascript
5 + 2 = 7   // Adição
5 - 2 = 3   // Subtração
5 * 2 = 10  // Multiplicação
5 / 2 = 2.5 // Divisão
5 % 2 = 1   // Módulo (Resto da divisão inteira)
5 ** 2 = 25 // Exponenciação (potência)
```

## Precedência
> ⚠ Assim como na matemática, exite prescendência de operadores. Utilize parênteses para garantir a ordem desejada.

**Ordem de precedência:**
1. `()`
2. `**`
3. `* / %`
4. `+ -`

## Auto-atribuição
Os operadores de auto-atribuição são `=`, `+=`, `-=`, `*=`, `/=`, `%=`, `**=`.

Exemplos:
```javascript
var numero = 10;
numero = numero + 5;    // Sem auto-atribuição
console.log(numero);    // 15
numero += 5;            // Com auto-atribuição
console.log(numero);    // 20
```

## Incremento e decremento
Os operadores de incremento e decremento são `++` e `--`.

> Existem dois tipos de incrementos e decrementos, os `pós` e os `pré`.

Exemplos:
```javascript
var numero = 10;
numero++; // Pós incremento
numero--; // Pós decremento

++numero; // Pré incremento
--numero; // Pré decremento
```

- Atribuição
- Relacionais
- Lógicos
- Ternários