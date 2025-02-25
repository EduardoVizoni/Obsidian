## Índice
- [Introdução](#introdução)
- [Sintaxe](#sintaxe)
- [Tipos de Dados](#tipos-de-dados)
- [Controle de Fluxo](#controle-de-fluxo)
- [Funções](#funções)
- [Objetos](#objetos)
- [Arrays](#arrays)
- [Exceções](#exceções)
---

## Introdução
JavaScript é uma linguagem de programação amplamente utilizada para o desenvolvimento web, sendo executada no navegador (cliente) ou no servidor (com Node.js). Sua popularidade se deve à sua flexibilidade, ao poder de manipular interatividade em páginas web e a possibilidade de rodar em múltiplas plataformas.

- **Interpretada**: O código JavaScript é executado diretamente no ambiente de execução (navegador ou Node.js).
- **Multiplataforma**: Funciona em qualquer navegador moderno e também pode ser usado no lado do servidor com Node.js.

## Sintaxe

JavaScript é uma linguagem de sintaxe simples e baseada em C. Aqui estão alguns conceitos básicos.

### Exemplo Básico

```javascript
console.log("Hello, World!");
```
### Declaração de Variáveis

Você pode declarar variáveis de três formas em JavaScript: `var`, `let` e `const`.

```javascript
let nome = "JavaScript";
const idade = 25;
var cidade = "São Paulo";
```

### Estruturas de Controle
- **if-else**
- **switch**
- **for**
- **while**
- **do-while**

#### Exemplo de `if-else`:

```javascript
let x = 10;
if (x > 0) {
    console.log("Positivo");
} else {
    console.log("Negativo");
}
```

#### Exemplo de `for`:

```javascript
for (let i = 0; i < 5; i++) {
    console.log(i);
}
```

## Tipos de Dados

JavaScript possui tipos de dados primitivos e complexos.

### Tipos Primitivos
- **number**: Números (inteiros ou decimais).
- **string**: Sequência de caracteres.
- **boolean**: Valores verdadeiro ou falso.
- **undefined**: Valor indefinido, quando a variável não é inicializada.
- **null**: Representa a ausência de valor.

### Tipos de Dados Complexos
- **Object**: Conjunto de pares chave-valor.
- **Array**: Lista ordenada de valores.
  
```javascript
let numero = 10; // number
let nome = "JavaScript"; // string
let ativo = true; // boolean

let pessoa = { nome: "João", idade: 30 }; // object
let lista = [1, 2, 3, 4]; // array
```

## Controle de Fluxo

As estruturas de controle permitem que você altere o fluxo de execução do código.

#### Condicional `if`
```javascript
let idade = 20;
if (idade >= 18) {
    console.log("Maior de idade");
} else {
    console.log("Menor de idade");
}
```

### Laços
- **for**
- **while**
- **do-while**
  
```javascript
for (let i = 0; i < 5; i++) { console.log(i); }
```

## Funções

Funções em JavaScript são blocos de código que podem ser reutilizados. Elas podem ser declaradas de diversas maneiras.

### Definindo uma função

```javascript
function saudacao(nome) {
    console.log("Olá, " + nome);
}

saudacao("Maria");
```

### Função anônima (arrow function)

```javascript
const soma = (a, b) => a + b;
console.log(soma(5, 3));
```

## Objetos

Objetos em JavaScript são coleções de propriedades e métodos.

```javascript
let pessoa = {
    nome: "Maria",
    idade: 25,
    saudacao: function() {
        console.log("Olá, " + this.nome);
    }
};

pessoa.saudacao();
```

## Arrays

Arrays são listas ordenadas de valores.

### Criando e manipulando arrays

```javascript
let frutas = ["maçã", "banana", "laranja"];
console.log(frutas[0]); // maçã
frutas.push("manga"); // adiciona item ao final
console.log(frutas);
```

## Exceções

JavaScript possui tratamento de erros utilizando **try-catch**.

#### Exemplo de `try-catch`

```javascript
try {
    let resultado = 10 / 0;
    if (!isFinite(resultado)) {
        throw "Erro: Divisão por zero";
    }
} catch (erro) {
    console.log(erro);
}
```