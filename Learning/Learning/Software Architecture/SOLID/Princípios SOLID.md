## Índice 
1. [Introdução](#introdução-solid) 
2. [Princípios](#princípios-solid) 
	- [SRP (Single Responsibility Principle)](#srp-single-responsibility-principle) 
	- [OCP (Open/Closed Principle)](#ocp-openclosed-principle) 
	- [LSP (Liskov Substitution Principle)](#lsp-liskov-substitution-principle) 
	- [ISP (Interface Segregation Principle)](#isp-interface-segregation-principle) 
	- [DIP (Dependency Inversion Principle)](#dip-dependency-inversion-principle) 
3. [Vantagens](#vantagens-solid) 
4. [Assuntos Correlacionados](#assuntos-correlacionados-solid)11

---

## **Visão Geral**

O **SOLID** é um acrônimo que representa cinco princípios essenciais para o desenvolvimento de software orientado a objetos. Eles têm como objetivo melhorar a qualidade do código, tornando-o mais modular, flexível, escalável e fácil de manter. Os princípios SOLID são amplamente aplicados em design de software, especialmente no desenvolvimento de sistemas que devem ser facilmente modificáveis ao longo do tempo.

- **SRP** (Single Responsibility Principle) - Princípio da Responsabilidade Única
- **OCP** (Open/Closed Principle) - Princípio Aberto/Fechado
- **LSP** (Liskov Substitution Principle) - Princípio da Substituição de Liskov
- **ISP** (Interface Segregation Principle) - Princípio da Segregação de Interfaces
- **DIP** (Dependency Inversion Principle) - Princípio da Inversão de Dependência

Esses princípios são essenciais para a construção de sistemas com código claro, modular e fácil de modificar, garantindo uma maior manutenibilidade e flexibilidade durante todo o ciclo de vida do software.

---

## **Princípio da Responsabilidade Única (SRP)**

O **Princípio da Responsabilidade Única** afirma que uma classe deve ter **uma única razão para mudar**, ou seja, ela deve ser responsável por **apenas uma parte do sistema**. Quando uma classe tem múltiplas responsabilidades, ela acaba se tornando mais difícil de entender, testar e modificar.

Aplicando o SRP, conseguimos separar as funcionalidades de uma aplicação em classes distintas, cada uma com um objetivo claro e focado. Assim, quando for necessário modificar ou adicionar novas funcionalidades, a mudança será limitada à classe correspondente, sem afetar outras partes do sistema.

---

## **Princípio Aberto/Fechado (OCP)**

O **Princípio Aberto/Fechado** diz que **as classes devem ser abertas para extensão, mas fechadas para modificação**. Ou seja, devemos ser capazes de adicionar novos comportamentos a uma classe existente sem alterar seu código fonte.

Este princípio incentiva a utilização de herança, interfaces e polimorfismo para adicionar novas funcionalidades, sem precisar modificar o comportamento já implementado. Com isso, o sistema se torna mais flexível e seguro, pois mudanças em uma classe não afetam outras partes do código.

---

## **Princípio da Substituição de Liskov (LSP)**

O **Princípio da Substituição de Liskov** afirma que as **subclasses devem ser substituíveis pelas suas superclasses** sem afetar o funcionamento correto do sistema. Em outras palavras, uma instância de uma classe derivada deve poder ser usada no lugar da sua classe base sem alterar o comportamento esperado.

Esse princípio garante que a hierarquia de herança esteja bem definida e que o comportamento das subclasses seja coerente com o comportamento das superclasses. Isso é fundamental para garantir que o código seja reutilizável e que o sistema funcione corretamente ao substituir uma classe por uma de sua hierarquia.

---

## **Princípio da Segregação de Interfaces (ISP)**

O **Princípio da Segregação de Interfaces** afirma que **uma classe não deve ser forçada a implementar interfaces que não usa**. Ao invés de criar interfaces grandes e genéricas, devemos criar interfaces mais específicas e coesas, adaptadas às necessidades de cada classe.

Isso ajuda a evitar a situação em que uma classe é obrigada a implementar métodos que não são relevantes para seu funcionamento, promovendo um design mais limpo e coeso. Classes com interfaces pequenas e específicas têm menos dependências e são mais fáceis de modificar sem afetar outras partes do sistema.

---

## **Princípio da Inversão de Dependência (DIP)**

O **Princípio da Inversão de Dependência** afirma que **as classes de alto nível não devem depender de classes de baixo nível**, mas ambas devem depender de abstrações (interfaces ou classes abstratas). Isso significa que, ao invés de uma classe de alto nível depender diretamente de uma implementação específica, ela deve depender de uma interface ou abstração que permita a troca de implementações sem afetar o comportamento do sistema.

Este princípio é essencial para reduzir o acoplamento entre componentes e tornar o sistema mais flexível e fácil de testar. Quando as dependências são invertidas, o código torna-se mais desacoplado e as implementações podem ser facilmente substituídas sem a necessidade de grandes mudanças no sistema.

---
## **Assuntos Correlacionados** 

- [[Programação Orientada a Objetos (POO)]]: A aplicação dos princípios SOLID é fundamental para o design orientado a objetos. 
- [[Model-View-Controller]]: SOLID ajuda na criação de sistemas mais modulares, o que é importante para a implementação do padrão MVC. 
- [[Arquitetura Orientada a Serviços]]: Aplicar os princípios SOLID em serviços ajuda a criar sistemas mais reutilizáveis e robustos.