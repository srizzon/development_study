# Aula 15 - Variáveis compostas

Um array (vetor) é uma estrutura de dados que armazena vários valores em uma única variável.

```
var numeros = [0, 1, 2]
```

- A variável `numeros` é um array.
- O array é composto por elementos.
- Elemento de um vetor agrupa um espaço de memória, o valor colocado dentro dele e um índice.
- O índice é um número que representa a posição do elemento dentro do array.

Um array é uma variável que tem vários elementos, e cada elemento é composto por seu valor e tem uma chave de identificação.

Exemplo:

```javascript
let num = [5, 8, 4];
num[3] = 6;
num.push(7);
num.length; // 4
num.sort(); // [4, 5, 6, 7, 8]
num.indexOf(8); // 1
```