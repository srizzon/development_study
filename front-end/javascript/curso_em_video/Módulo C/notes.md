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

- O que significa a sigla DOM?
> DOM significa Document Object Model.

- O que são os elementos `Parent` e os elementos `Child` em uma árvore DOM?
> `Parent` é o elemento pai, `Child` é o elemento filho.

- Quais os cinco principais métodos de selecionar elementos DOM dentro do JS?
> `getElementById()`, `getElementsByTagName()`, `getElementsByName()`, `getElementsByClassName()`, `querySelector()`.

# Aula 10 - Eventos DOM

Exemplo:
```javascript
var a = window.document.getElementById('area');

a.addEventListener('click', clicar);
a.addEventListener('mouseenter', entrar);
a.addEventListener('mouseout', sair);

function clicar() {
    a.innerHTML = "Clicou!";
    a.style.backgroundColor = 'red';
}

function entrar(){
    a.innerHTML = "Entrou!";
}

function sair(){
    a.innerHTML = "Saiu!";
    a.style.backgroundColor = 'green';
}
```