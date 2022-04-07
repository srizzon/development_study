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

## Operadores `Arítimeticos`

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

## Operadores de `Atribuição`
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

# Aula 08 - Operadores (parte 2)

## Operadores `Relacionais`
Os operadores relacionais são `<`, `>`, `<=`, `>=`, `==`, `!=`, `===`, `!==`.

Exemplos:
```javascript
5 > 2; // true
7 < 4; // false
8 >= 8; // true
9 <= 7; // false
5 == 5; // true
4 != 4; // false
5 === '5'; // false
5 !== '5'; // true
```

### **Operadores de identidade**
Os operadores de identidade comparam o valor e o tipo.

Exemplos:
```javascript
5 == 5; // true
5 == '5'; // true
5 === '5'; // false
5 === 5; // true
```

## Operadores de `Lógicos`
Os operadores lógicos são `!`, `&&`, `||`.

- ! significa `negação`.
    - É tratado como um operador unário. Só precisa de um operando. Exemplo: `!true`;
- && significa `conjunção`.
    - É tratado como um operador binário. Precisa de dois operandos. Exemplo: `true && false`;
- || significa `disjunção`.
    - É tratado como um operador binário. Precisa de dois operandos. Exemplo: `true || false`;

Exemplos:
```javascript
idade >= 15 && idade <= 17;         // A idade está entre 15 e 17 anos?
estado == 'RJ' || estado == 'SP';   // O estado é RJ ou SP?
salario > 1500 && sexo != 'M';      // O salario é maior que 1500 e o sexo é diferente de M (masculino)?
```

Ordem de precedência:
```javascript
1. `()` // Arietmético
2. `**` // Aritmético
3. `* / %` // Aritmético
4. `+ -` // Aritmético
5. `< > <= >= == != === !==` // Relacional
6. `!` // Lógico
7. `&&` // Lógico
8. `||` // Lógico
```

> ℹ Obs: os operadores relacionais não possuem ordem de precedência. Quem está mais a esquerda é o operador mais prioritário.

## Operadores de `Ternários`
Os operadores de ternário são `?` e `:`.

Construção:
```javascript
teste `?` true `:` false
```

Exemplo:
```javascript
var idade = 18;
var categoria = idade >= 18 ? 'adulto' : 'crianca';
console.log(categoria); // adulto
```