# Aula 9 – Introdução ao DOM

## O que é DOM?
D - Document
O - Object
M - Model

É um conjunto de objetos dentro do navegador que dá acesso aos componentes internos do website.

## Árvore DOM
```
├── window (parent)
│   ├── location (child)
│   ├── document
|   │   └── html
|   │       ├── head
|   │       │   ├── meta
|   │       │   └── title
|   │       └── body
|   │           ├── h1
|   │           ├── p
|   │           ├── p
|   │           └── div
│   └── history
```

## Selecionando elementos
- Por ID -> `getElementById()`
- Por tag -> `getElementsByTagName()`
- Por nome -> `getElementsByName()`
- Por classe -> `getElementsByClassName()`
- Por seletor -> `querySelector()` || `querySelectorAll()`

> O `querySelector` é recente, portando alguns navegadores podem não ter suporte a ele.

## Perguntas
- Qual a diferença entre `innerText` e `innerHTML`?
> `innerText` retorna o texto sem tags, `innerHTML` retorna o texto com tags.