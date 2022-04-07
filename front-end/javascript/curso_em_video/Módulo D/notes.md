# Aula 11 - Condições (parte 1)

## Condições simples e compostas
Exemplo:

```javascript
if (condição) {
    // Executa algo
} else {
    // Executa algo
}
```

Uma `condição simples` é composta por uma expressão e um `operador lógico`.

Uma `condição composta` é composta por mais de uma condição simples. Exemplo: `if` e `else`.

## Condições aninhadas
Exemplo:

```javascript
if (condição1) {
    // Executa algo
} else if (condição2) {
    // Executa algo
    if (condição3) {
        // Executa algo
    } else {
        // Executa algo
    }
} else {
    // Executa algo
}
```

## Condição multipla

> **switch**

Exemplo:

```javascript
switch (condição) {
    case 'valor1':
        // Executa algo
        break; // O break é obrigatório quando utilizamos o `case`.
    case 'valor2':
        // Executa algo
        break;
    default:
        // Executa algo
        break;
}
```

Exemplo com dias da semana:
```javascript
var agora = new Date();
var diaDaSemana = agora.getDay();

switch(diaDaSemana) {
    case 0:
        console.log('Domingo');
        break;
    case 1:
        console.log('Segunda');
        break;
    case 2:
        console.log('Terça');
        break;
    case 3:
        console.log('Quarta');
        break;
    case 4:
        console.log('Quinta');
        break;
    case 5:
        console.log('Sexta');
        break;
    case 6:
        console.log('Sábado');
        break;
    default:
        console.log('Dia inválido');
}
```