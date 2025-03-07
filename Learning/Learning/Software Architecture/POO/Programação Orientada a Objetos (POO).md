## Índice  
1. [Introdução](#introdução-poo)  
2. [Princípios](#princípios-poo)  
   - [Encapsulamento](#encapsulamento)  
   - [Herança](#herança)  
   - [Polimorfismo](#polimorfismo)  
   - [Abstração](#abstração)  
3. [Vantagens](#vantagens-poo)  
4. [Assuntos Correlacionados](#assuntos-correlacionados)

---

## **Introdução**

A Programação Orientada a Objetos (POO) é um paradigma de programação baseado no conceito de **objetos**, que são instâncias de **classes**. As classes contêm **atributos** (dados) e **métodos** (comportamentos). A POO visa melhorar a modularidade, reutilização e manutenção do código.

## **Princípios**

### **Encapsulamento**

O **encapsulamento** consiste em esconder os detalhes internos de uma classe e expor apenas as funcionalidades necessárias através de métodos públicos. Isso aumenta a segurança e permite que o código seja modificado sem afetar outros sistemas.

O **encapsulamento** **restringe o acesso direto aos atributos de uma classe** usando modificadores de acesso (`private`, `protected`, `public`) e **controla a forma como esses atributos são manipulados** por meio de métodos (getters, setters e regras de negócio). Isso protege os dados, evita modificações indevidas e mantém a integridade do sistema.

### **Herança**

A **herança** permite que uma classe herde características e comportamentos de outra. Isso facilita a reutilização de código e a criação de hierarquias de classes. Uma subclasse pode adicionar ou modificar comportamentos herdados.

Herança permite que uma classe (filha) **reutilize atributos e métodos** de outra classe (pai) usando a palavra-chave **`extends`**.

A classe filha pode:

1. Usar atributos e métodos da classe pai.
2. Adicionar seus próprios métodos.
3. Sobrescrever métodos da classe pai (polimorfismo).

Isso facilita a **reutilização de código** e a **organização do programa**.

### **Polimorfismo**

O **polimorfismo** permite que objetos de diferentes classes sejam tratados como objetos de uma classe comum. Isso é possível devido à herança e interfaces, permitindo que diferentes tipos de objetos implementem o mesmo método de maneiras diferentes.

- **Sobrecarga**(Overload): O **mesmo nome de método**, mas você **modifica a forma de usá-lo**. Em Java, isso é feito alterando a quantidade ou tipo de parâmetros que o método aceita.  
    **Exemplo**: Uma **máquina de café** que pode fazer diferentes tipos de café com base em quantos ingredientes você fornece.
    
- **Sobrescrita**(Override): Você **mantém o nome do método**, mas **modifica completamente o comportamento** do método na subclasse. Em Java, isso é feito na subclasse, alterando o método herdado da classe pai.  
    **Exemplo**: Um **cachorro** que "latia" ao invés de fazer um som qualquer, alterando o comportamento de um método herdado da classe `Animal`.

### **Abstração**

A **abstração** é o processo de esconder a complexidade dos detalhes e mostrar apenas o essencial. Isso permite que os desenvolvedores se concentrem no que é relevante e deleguem os detalhes ao sistema.

- **Abstração** permite que você **esconda detalhes complexos** e mostre **apenas o essencial**, fornecendo uma interface para interação com o sistema.
- **Exemplo prático**: Uma **classe abstrata `Pagamento`** define o comportamento básico de pagamento, mas as subclasses definem como cada tipo de pagamento é processado.
## **Vantagens**

- **Modularidade**: O código é organizado em classes e objetos, facilitando o entendimento e a manutenção.
- **Reusabilidade**: Com a herança, é possível reutilizar código de maneira eficiente.
- **Escalabilidade**: A POO facilita a expansão de sistemas sem impactos negativos nos componentes existentes.
- **Manutenibilidade**: Alterações em uma classe ou objeto afetam menos o sistema como um todo.

---

## **Assuntos Correlacionados**

- [[Princípios SOLID]]: Os princípios SOLID são fundamentais para a boa prática de design de software orientado a objetos. 
- [[Model-View-Controller]]: O padrão MVC pode ser implementado utilizando POO, promovendo uma boa separação de responsabilidades. 
- [[Arquitetura Orientada a Serviços]]: A arquitetura orientada a serviços(SOA) pode ser construída utilizando princípios de POO para criar serviços reutilizáveis e modulares.  
