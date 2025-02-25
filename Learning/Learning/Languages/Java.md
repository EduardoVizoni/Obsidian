## Índice
- [Introdução](#introdução)
- [Sintaxe](#sintaxe)
- [Tipos de Dados](#tipos-de-dados)
- [Controle de Fluxo](#controle-de-fluxo)
- [Orientação a Objetos](#orientação-a-objetos)
- [Coleções](#coleções)
- [Exceções](#exceções)
---

## Introdução
Java é uma linguagem de programação orientada a objetos, desenvolvida por James Gosling e Mike Sheridan na Sun Microsystems em 1991, que mais tarde foi adquirida pela Oracle. É uma das linguagens mais populares e amplamente utilizada para desenvolvimento de aplicativos em diferentes plataformas, desde web até dispositivos móveis.

- **Compilação para bytecode**: O código Java é compilado para bytecode, que é executado na Java Virtual Machine (JVM).
- **Portabilidade**: O slogan "Write Once, Run Anywhere" reflete a portabilidade do código Java.

## Sintaxe

Java tem uma sintaxe que se baseia em C, com algumas diferenças para facilitar a programação orientada a objetos. Aqui estão alguns pontos principais:

### Exemplo Básico

```java
public class HelloWorld {
    public static void main(String[] args) {
        System.out.println("Hello, World!");
    }
}
```

### Declaração de Variáveis

Em Java, você deve declarar o tipo da variável antes de usá-la.

```java
int x = 5; 
String texto = "Java"; 
boolean isActive = true;
```

### ### Estruturas de Controle
- **if-else**: Condicional simples.
- **switch**: Condicional de múltiplos casos.
- **for**: Laço de repetição com contador.
- **while**: Laço de repetição com condição.
- **do-while**: Laço que sempre executa pelo menos uma vez.

#### Exemplo de `if-else`:
```java
if (x > 0) {
    System.out.println("Positivo");
} else {
    System.out.println("Negativo");
}
```

#### Exemplo de `for`:
```java
for (int i = 0; i < 5; i++) { 
	System.out.println(i); }
```

#### Exemplo de `for`:
```java
for (int i = 0; i < 5; i++) { 
	System.out.println(i); }
```

## Tipos de Dados

Java possui tipos de dados primitivos e complexos.

### Tipos Primitivos
- **int**: Números inteiros.
- **double**: Números de ponto flutuante.
- **char**: Caracteres.
- **boolean**: Valores verdadeiro ou falso.

### Tipos de Dados Complexos
- **String**: Sequência de caracteres.
- **Arrays**: Coleções de valores do mesmo tipo.

```java
int[] numeros = {1, 2, 3, 4}; 
String nome = "Java";
```

## Controle de Fluxo

As estruturas de controle são usadas para modificar o fluxo de execução do programa.

#### Condicional `if`
```java
if (x > 0) {     System.out.println("Positivo"); }`
```

### Laços
- **for**
- **while**
- **do-while**

```java
for (int i = 0; i < 10; i++) {     
	System.out.println(i); }`
```

## Orientação a Objetos

Java é uma linguagem orientada a objetos, o que significa que tudo é tratado como objetos e classes. Os principais pilares são:

### Encapsulamento

A prática de esconder os detalhes de implementação e mostrar apenas os recursos essenciais de uma classe.

```java
public class Pessoa {
    private String nome;

    public String getNome() {
        return nome;
    }

    public void setNome(String nome) {
        this.nome = nome;
    }
}

```
### Herança

Permite criar uma nova classe baseada em uma classe existente.

```java
public class Estudante extends Pessoa {
    private String matricula;

    public String getMatricula() {
        return matricula;
    }

    public void setMatricula(String matricula) {
        this.matricula = matricula;
    }
}

```

### Polimorfismo

Permite que uma classe tenha diferentes implementações de um método.

```java
public class Animal {
    public void fazerSom() {
        System.out.println("Som de animal");
    }
}

public class Cachorro extends Animal {
    @Override
    public void fazerSom() {
        System.out.println("Latido");
    }
}

```

## Coleções

Java oferece várias coleções, como **List**, **Set**, **Map**, que ajudam a armazenar dados de forma eficiente.

#### Exemplo com `ArrayList` (uma implementação de `List`):

```java
import java.util.ArrayList;

public class ExemploArrayList {
    public static void main(String[] args) {
        ArrayList<String> lista = new ArrayList<>();
        lista.add("Java");
        lista.add("Python");
        lista.add("JavaScript");

        for (String linguagem : lista) {
            System.out.println(linguagem);
        }
    }
}

```

## Exceções

Exceções são usadas para capturar e tratar erros durante a execução de um programa.

#### Exemplo de `try-catch`:

```java
try {
    int resultado = 10 / 0;
} catch (ArithmeticException e) {
    System.out.println("Erro: " + e.getMessage());
} finally {
    System.out.println("Bloco finally sempre é executado");
}

```