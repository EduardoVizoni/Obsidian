**Model-View-Controller**

---

## **Visão Geral**

O padrão **MVC (Model-View-Controller)** é um padrão arquitetural utilizado para separar as responsabilidades de uma aplicação em três componentes distintos: **Model**, **View** e **Controller**. Essa separação facilita o desenvolvimento, manutenção e escalabilidade das aplicações, tornando-as mais modulares.

O **MVC** visa desacoplar a interface do usuário (View) da lógica de negócios (Model), enquanto o **Controller** funciona como intermediário entre os dois. Esse padrão é amplamente utilizado no desenvolvimento de aplicativos web, como no caso do **Spring MVC**, **ASP.NET MVC**, entre outros.

---

## **Model**

O **Model** representa a camada de dados da aplicação, sendo responsável por armazenar, manipular e acessar as informações que serão processadas pela aplicação. Ele não tem conhecimento da interface do usuário (View), mas pode notificar o **Controller** sobre mudanças nos dados, para que ele tome as ações necessárias.

Em outras palavras, o **Model** gerencia os dados da aplicação, suas regras de negócios e interações com o banco de dados ou qualquer outra fonte de dados.

---

## **View**

A **View** é a camada responsável pela apresentação dos dados ao usuário. Ela exibe as informações que o **Model** fornece e também captura as ações do usuário, que são enviadas ao **Controller**. A **View** deve ser independente da lógica de negócios, ou seja, não deve realizar processamento de dados, apenas exibir informações.

A **View** pode ser uma página HTML, um componente gráfico de uma interface de desktop, ou qualquer outra forma de apresentação de dados, dependendo do tipo de aplicação.

---

## **Controller**

O **Controller** atua como um intermediário entre o **Model** e a **View**. Ele recebe as entradas do usuário (geralmente vindas da **View**), processa essas entradas (com base nas regras de negócios no **Model**) e atualiza a **View** com os resultados.

O **Controller** é responsável por orquestrar a interação entre o **Model** e a **View**, além de gerenciar os fluxos de controle e decidir qual **View** mostrar dependendo das ações do usuário.

---

## **Benefícios do MVC**

1. **Separação de Responsabilidades**: Ao separar a aplicação em três camadas distintas (Model, View, Controller), o padrão MVC ajuda a reduzir o acoplamento entre elas, facilitando a manutenção e extensibilidade da aplicação.
    
2. **Facilidade de Testes**: Com a separação das camadas, podemos testar o **Model** e o **Controller** de forma isolada, sem depender da interface do usuário (View), tornando os testes unitários mais fáceis de serem realizados.
    
3. **Escalabilidade**: O MVC torna o desenvolvimento mais modular, permitindo que diferentes desenvolvedores trabalhem em diferentes componentes da aplicação ao mesmo tempo. Isso facilita a expansão da aplicação no futuro.
    
4. **Manutenibilidade**: A separação das responsabilidades facilita a modificação do código. Caso seja necessário mudar a **View** (interface de usuário), não há a necessidade de alterar o **Model** ou **Controller**, e vice-versa.
    

---

## **Exemplo de Fluxo MVC**

1. O **usuário** interage com a **View** (por exemplo, clicando em um botão ou preenchendo um formulário).
2. A **View** envia a entrada do usuário para o **Controller**.
3. O **Controller** processa a entrada, possivelmente interage com o **Model** para manipular dados e, em seguida, seleciona a **View** apropriada.
4. A **View** é atualizada com os novos dados fornecidos pelo **Model** ou com os resultados da interação.

Esse fluxo permite uma interação eficiente entre a interface e a lógica de negócios, garantindo que a aplicação seja organizada e fácil de entender.

---

## **Assuntos Correlacionados** 

- [POO](#poo): MVC pode ser implementado utilizando POO, organizando o código de forma modular. 
- [[S.O.L.I.D Principle]]: Aplicar os princípios SOLID no MVC melhora a estrutura e a manutenibilidade do sistema. 
- [[S.O.A]]: O MVC pode ser utilizado dentro de uma arquitetura orientada a serviços para promover a separação de responsabilidades.