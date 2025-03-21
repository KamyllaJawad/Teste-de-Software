# Níveis de Teste

Os níveis de teste são etapas no processo de teste que correspondem a diferentes fases do desenvolvimento de software. Cada nível tem um foco específico e objetivos distintos, garantindo que o software seja testado de forma abrangente e sistemática.


![...](../assets/Teste-de-software-1920x1306-1-1536x1045.png)

### **1. O que são Níveis de Teste?**
Os níveis de teste são classificações que organizam o processo de teste em fases, cada uma com um escopo e objetivo específico. Eles são aplicados ao longo do ciclo de vida do desenvolvimento de software (SDLC) e ajudam a garantir que todas as partes do sistema sejam testadas adequadamente.

Os principais níveis de teste são:
1. **Teste Unitário (Unit Testing)**
2. **Teste de Integração (Integration Testing)**
3. **Teste de Sistema (System Testing)**
4. **Teste de Aceitação (Acceptance Testing)**

---

### **2. Teste Unitário (Unit Testing)**

#### **O que é?**
- O teste unitário é o primeiro nível de teste e foca em **verificar a menor unidade testável do software**, como funções, métodos ou classes.
- É realizado pelos desenvolvedores durante a fase de codificação.

#### **Objetivos**:
- Verificar se cada unidade do código funciona conforme o esperado.
- Identificar defeitos no nível mais básico do software.

#### **Características**:
- **Escopo**: Pequeno e específico (uma função ou método).
- **Responsabilidade**: Desenvolvedores.
- **Ferramentas**: Frameworks como JUnit (Java), NUnit (.NET), pytest (Python), etc.
- **Abordagem**: Testes de caixa branca (white-box), onde o testador conhece a estrutura interna do código.

#### **Exemplo**:
- Testar uma função que calcula a soma de dois números para garantir que ela retorne o resultado correto.

---

### **3. Teste de Integração (Integration Testing)**

#### **O que é?**
- O teste de integração verifica a **interação entre diferentes módulos ou componentes** do software para garantir que eles funcionem corretamente quando combinados.
- Pode ser feito de forma incremental (módulo por módulo) ou big bang (todos os módulos de uma vez).

#### **Objetivos**:
- Identificar problemas na comunicação entre módulos.
- Garantir que os componentes integrados funcionem como um todo.

#### **Características**:
- **Escopo**: Módulos ou componentes interconectados.
- **Responsabilidade**: Desenvolvedores ou testadores.
- **Ferramentas**: Frameworks como TestNG, Selenium (para integração de interfaces), etc.
- **Abordagem**: Testes de caixa preta (black-box) ou caixa cinza (gray-box).

#### **Exemplo**:
- Testar a integração entre um módulo de autenticação e um módulo de banco de dados para garantir que o login funcione corretamente.

---

### **4. Teste de Sistema (System Testing)**

#### **O que é?**
- O teste de sistema avalia o **software completo e integrado** para garantir que ele atenda aos requisitos especificados.
- É realizado em um ambiente que simula o ambiente de produção.

#### **Objetivos**:
- Verificar o comportamento do sistema como um todo.
- Validar funcionalidades, desempenho, segurança e usabilidade.

#### **Características**:
- **Escopo**: Sistema completo.
- **Responsabilidade**: Equipe de teste.
- **Ferramentas**: Ferramentas de teste de desempenho (JMeter, LoadRunner), ferramentas de teste de segurança (OWASP ZAP), etc.
- **Abordagem**: Testes de caixa preta (black-box), onde o testador não precisa conhecer a estrutura interna do código.

#### **Exemplo**:
- Testar um sistema de e-commerce para garantir que todas as funcionalidades (carrinho de compras, pagamento, etc.) funcionem corretamente.

---

### **5. Teste de Aceitação (Acceptance Testing)**

#### **O que é?**
- O teste de aceitação é o último nível de teste e é focado em **validar se o software atende às necessidades do usuário final** e está pronto para ser liberado.
- Pode ser dividido em:
  - **Teste de Aceitação do Usuário (UAT - User Acceptance Testing)**: Realizado pelos usuários finais.
  - **Teste de Aceitação de Negócios (BAT - Business Acceptance Testing)**: Focado em garantir que o software atenda aos requisitos de negócios.

#### **Objetivos**:
- Garantir que o software esteja alinhado com as expectativas do usuário e dos stakeholders.
- Validar se o software está pronto para ser implantado em produção.

#### **Características**:
- **Escopo**: Sistema completo, com foco em requisitos de negócios e usabilidade.
- **Responsabilidade**: Usuários finais, stakeholders ou equipe de teste.
- **Ferramentas**: Ferramentas de automação como Selenium, Cucumber, etc.
- **Abordagem**: Testes de caixa preta (black-box).

#### **Exemplo**:
- Testar um sistema de gestão de estoque para garantir que ele atenda às necessidades da equipe de logística e aos processos de negócios da empresa.

---

### **6. Comparação entre os Níveis de Teste**

| **Nível de Teste**       | **Escopo**                  | **Responsabilidade**       | **Foco**                                   |
|--------------------------|-----------------------------|----------------------------|--------------------------------------------|
| **Teste Unitário**        | Funções/métodos individuais | Desenvolvedores            | Funcionalidade interna do código           |
| **Teste de Integração**   | Interação entre módulos     | Desenvolvedores/Testadores | Comunicação entre componentes              |
| **Teste de Sistema**      | Sistema completo            | Equipe de teste            | Requisitos funcionais e não funcionais     |
| **Teste de Aceitação**    | Sistema completo            | Usuários/Stakeholders      | Alinhamento com necessidades do usuário    |

---

### **7. Importância dos Níveis de Teste**
- **Abordagem Sistemática**: Garante que todas as partes do software sejam testadas de forma organizada.
- **Detecção Precoce de Defeitos**: Problemas são identificados em estágios iniciais, reduzindo custos e esforços.
- **Qualidade do Software**: Cada nível contribui para a melhoria da qualidade do produto final.
- **Confiança**: Aumenta a confiança dos stakeholders no software.

