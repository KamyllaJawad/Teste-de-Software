# Práticas de Desenvolvimento de Software e Testes

Desenvolver software não é só codar, é pensar, planejar, testar e comunicar. Essas abordagens nos ajudam a fazer isso com excelência.
No desenvolvimento de software, escrever código funcional **não é o suficiente**. É preciso garantir que esse código:
- faz o que o cliente espera,
- se comporta corretamente em diferentes situações,
- é fácil de entender, testar e manter.
- 
Com o tempo, surgiram várias **abordagens e metodologias** que nos ajudam a melhorar a **qualidade**, a **organização** e a **colaboração** durante o desenvolvimento.

Cada uma dessas abordagens tem um **propósito específico**, e entender quando e como usá-las é fundamental para se tornar um desenvolvedor completo e preparado para projetos reais.

As siglas que você verá a seguir são comuns no mundo do desenvolvimento de software e podem ser usadas em diferentes contextos, como **engenharia de software**, **testes automatizados** e **desenvolvimento ágil**.

---

## 📌 1. **TDD - Test-Driven Development (Desenvolvimento Orientado a Testes)**

### ✅ O que é:
TDD é uma técnica de desenvolvimento onde **os testes são escritos antes do código funcional**. O ciclo é:  
**Red ➡️ Green ➡️ Refactor**:
1. Escreva um teste que falhe (Red)
2. Implemente o código apenas o suficiente para passar o teste (Green)
3. Refatore o código mantendo os testes verdes (Refactor)

### 🕐 Quando utilizar:
- Ao desenvolver **módulos críticos**, como sistemas bancários, médicos, financeiros.
- Quando se busca **alta cobertura de testes**.
- Projetos com **equipe madura** em testes automatizados.

### 🧪 Exemplo (Python + PyTest):
```python
# test_calculadora.py
def test_soma():
    assert soma(2, 3) == 5

# calculadora.py
def soma(a, b):
    return a + b
```

### 🧠 Boas práticas:
- Testes devem ser **rápidos, isolados e independentes**.
- Nomeie os testes de forma **descritiva**.
- Escreva o menor código possível para passar o teste.

---

## 📌 2. **BDD - Behavior-Driven Development (Desenvolvimento Orientado por Comportamento)**

### ✅ O que é:
BDD é uma evolução do TDD, onde o foco está em **descrever o comportamento do sistema em linguagem natural**, geralmente usando o formato `Gherkin` (Given-When-Then).

### 🕐 Quando utilizar:
- Ideal para **projetos colaborativos** entre desenvolvedores, QA e Product Owners.
- Sistemas onde a **regra de negócio** precisa ser compreendida por todos.

### 📋 Exemplo (JavaScript + Cucumber + Gherkin):
```gherkin
Feature: Login
  Scenario: Usuário insere credenciais válidas
    Given o usuário está na página de login
    When ele insere usuário "joao" e senha "123"
    Then ele deve ser redirecionado para o dashboard
```

### 🧠 Boas práticas:
- Use **linguagem clara e compartilhada**.
- Mantenha os cenários curtos e **orientados ao negócio**.
- Integre com ferramentas de automação de testes.

---

## 📌 3. **DDD - Domain-Driven Design (Design Orientado ao Domínio)**

### ✅ O que é:
DDD é uma abordagem para **modelar sistemas complexos baseados na lógica de negócio**, focando na **linguagem ubíqua** e **separação de responsabilidades** entre as camadas.

### 🕐 Quando utilizar:
- Projetos grandes e complexos com regras de negócio sofisticadas.
- Equipes com forte colaboração entre desenvolvedores e especialistas do domínio.

### 💻 Exemplo (Java + Spring):
```java
// Agregado
public class Pedido {
    private List<Item> itens;

    public void adicionarItem(Item item) {
        itens.add(item);
    }
}
```

### 🧠 Boas práticas:
- Separe bem **Entidades, Objetos de Valor e Agregados**.
- Trabalhe em **camadas**: Aplicação, Domínio, Infraestrutura.
- Use a **linguagem do negócio** no código.

---

## 📌 4. **FDD - Feature-Driven Development (Desenvolvimento Orientado a Funcionalidades)**

### ✅ O que é:
FDD é uma abordagem **iterativa** baseada no desenvolvimento de **funcionalidades pequenas e bem definidas**, geralmente iniciando com **modelagem do domínio**.

### 🕐 Quando utilizar:
- Projetos grandes com **múltiplas equipes**.
- Equipes que buscam **visibilidade do progresso por funcionalidade**.

### ⚙️ Exemplo de funcionalidade:
```
Funcionalidade: Calcular frete para pedido
Descrição: Permite ao sistema calcular o frete com base no CEP do cliente e peso total do pedido.
```

### 🧠 Boas práticas:
- Divida funcionalidades em **tarefas pequenas**.
- Use um **modelo de domínio inicial** para guiar o desenvolvimento.
- Monitore o progresso por funcionalidades entregues.

---

## 📌 5. **ATDD - Acceptance Test-Driven Development (Desenvolvimento Orientado a Testes de Aceitação)**

### ✅ O que é:
É semelhante ao BDD, mas com foco em **testes de aceitação escritos em conjunto com stakeholders**, descrevendo **exatamente quando a funcionalidade estará “pronta”**.

### 🕐 Quando utilizar:
- Quando a **validação do cliente** é crítica.
- Projetos onde os critérios de aceitação são rigorosos.

### 🧪 Exemplo com Robot Framework:
```robot
*** Test Cases ***
Validar Login com Sucesso
    Dado que o usuário acessa o sistema
    Quando ele insere usuário "alex" e senha "123"
    Então ele deve ver o painel de controle
```

### 🧠 Boas práticas:
- Envolva **clientes e testadores** na criação dos testes.
- Testes devem ser **executáveis automaticamente**.
- Critérios de aceitação devem ser **claros e objetivos**.

---

## 📌 6. **STDD - Specification by Test-Driven Development**

### ✅ O que é:
STDD é um termo menos comum, mas geralmente é entendido como um **cruzamento entre TDD e Especificação Formal**, onde o **teste é usado como especificação viva**.

### 🕐 Quando utilizar:
- Ambientes com **alta confiabilidade exigida**, como sistemas aeronáuticos, bancários, medicina.
- Projetos onde testes precisam **validar conformidade com requisitos formais.**

### 📋 Exemplo (C# com SpecFlow):
```gherkin
Scenario: Transferência bancária bem-sucedida
  Given uma conta com saldo R$500
  When R$100 é transferido para outra conta
  Then o saldo deve ser R$400
```

### 🧠 Boas práticas:
- Use ferramentas que **integram testes com especificações**.
- Mantenha a **trilha de auditoria** clara entre requisito e implementação.
- Integre com **CI/CD** para validação contínua.

---

## 📊 Comparativo final:

| Abordagem | Foco Principal | Quando Usar | Exemplo de Ferramenta |
|-----------|----------------|-------------|------------------------|
| **TDD** | Código testável desde o início | Lógica complexa e crítica | PyTest, JUnit |
| **BDD** | Comportamento e regras de negócio | Projetos com forte colaboração | Cucumber, Behave |
| **DDD** | Modelagem rica do domínio | Sistemas grandes com lógica complexa | Spring, .NET |
| **FDD** | Funcionalidades visíveis e entregas constantes | Times grandes | Jira, Trello |
| **ATDD** | Critérios de aceitação claros | Softwares com testes de aceitação automatizados | Robot Framework |
| **STDD** | Testes como especificação | Ambientes críticos e normativos | SpecFlow, FitNesse |

---

Se quiser, posso te ajudar a montar isso em formato de **apresentação para aula (PowerPoint)** ou com exemplos práticos em repositório de **GitHub didático**. Deseja isso?
---

## 📦 **No fim, todos são formas de organizar e melhorar como desenvolvemos software.**

Eles ajudam a responder perguntas como:
- ✅ *O que o sistema deve fazer?*
- 🧪 *Como garantir que está funcionando corretamente?*
- 🧠 *Como organizar o código de forma inteligente?*
- 🤝 *Como garantir que desenvolvedores e clientes estão alinhados?*

---

### 🧩 Comparando com o mundo real:

Imagine que estamos construindo um **prédio**. Cada uma dessas abordagens ajuda em uma parte:

| Sigla | O que representa na construção | Função principal |
|-------|-------------------------------|------------------|
| **TDD** | Engenheiro testando estrutura antes de construir | Garante que tudo funcione **desde o começo** |
| **BDD** | Cliente descrevendo como quer usar o prédio | Foca no **comportamento esperado** |
| **DDD** | Arquiteto organizando os cômodos com lógica | Organização baseada no **domínio (negócio)** |
| **FDD** | Lista de entregas (etapas da obra) | Divide o projeto em **pequenas funcionalidades** |
| **ATDD** | Cliente testando se tudo está como pediu | Define **critério de aceitação** antes de codar |
| **STDD** | Manual técnico normativo | Testes como **especificação formal e viva** |

---

### ✅ Em resumo:

> **Todos são estratégias para desenvolver software com mais qualidade, clareza e colaboração.**

Cada um tem seu foco:
- **TDD/ATDD/BDD/STDD** focam em **testes e validação**.
- **DDD/FDD** focam em **design e organização de funcionalidades**.


Perfeito! Aqui estão **10 livros clássicos e modernos** que você pode usar como **referência sólida e embasamento teórico** para sua aula sobre TDD, BDD, DDD, FDD, ATDD e STDD. Eles cobrem desde práticas de desenvolvimento ágil até testes, arquitetura e modelagem de domínio:

---

# 📚 Refêrencias:

#### 1. **Test-Driven Development: By Example**  
**Autor:** Kent Beck  
**Tema:** Fundamentos e prática do TDD com exemplos em Java.  
📌 **Base principal para TDD**.

#### 2. **Growing Object-Oriented Software, Guided by Tests**  
**Autores:** Steve Freeman e Nat Pryce  
**Tema:** Integra testes com design orientado a objetos.  
📌 Excelente para **TDD com foco em arquitetura limpa**.

#### 3. **Specification by Example**  
**Autor:** Gojko Adzic  
**Tema:** Introduz práticas de BDD e ATDD com testes de aceitação automatizados.  
📌 **Referência central para BDD/ATDD**.

#### 4. **Domain-Driven Design: Tackling Complexity in the Heart of Software**  
**Autor:** Eric Evans  
**Tema:** Fundamentos completos de DDD.  
📌 Livro **clássico e obrigatório para DDD**.

#### 5. **Implementing Domain-Driven Design**  
**Autor:** Vaughn Vernon  
**Tema:** Aplicação prática dos conceitos de DDD com exemplos em código.  
📌 **Complemento prático ao livro do Eric Evans**.

#### 6. **BDD in Action: Behavior-driven development for the whole software lifecycle**  
**Autor:** John Ferguson Smart  
**Tema:** Aplicação de BDD em projetos reais, usando ferramentas como Cucumber, JBehave e SpecFlow.  
📌 **Didático e atual**.

#### 7. **Agile Software Development: Principles, Patterns, and Practices**  
**Autores:** Robert C. Martin e Micah Martin  
**Tema:** Princípios SOLID, TDD, design orientado a objetos e desenvolvimento ágil.  
📌 **Base teórica forte para várias boas práticas**.

#### 8. **Clean Architecture**  
**Autor:** Robert C. Martin (Uncle Bob)  
**Tema:** Arquitetura limpa, separação de responsabilidades, coesão e desacoplamento.  
📌 Apoia **DDD, FDD e testes isolados**.

#### 9. **Refactoring: Improving the Design of Existing Code**  
**Autor:** Martin Fowler  
**Tema:** Refatoração com suporte a testes automatizados (essencial em TDD).  
📌 **Complemento prático para manter o código limpo**.

#### 10. **Continuous Delivery: Reliable Software Releases through Build, Test, and Deployment Automation**  
**Autores:** Jez Humble e David Farley  
**Tema:** Automatização do ciclo de desenvolvimento com integração contínua, testes automatizados e entrega frequente.  
📌 Suporte para **ATDD, TDD e qualidade contínua**.
