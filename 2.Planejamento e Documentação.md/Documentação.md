## **1. Test Plan (Plano de Teste)**

### **O que é?**
O **Plano de Teste** é um documento que descreve a estratégia, os recursos, o cronograma e os critérios para a execução dos testes. Ele é essencial para garantir que os testes sejam realizados de forma organizada e eficiente.

### **Modelo Baseado na ISO/IEC 29119**:

```
Título: Plano de Teste para [Nome do Projeto/Sistema]
Versão: [Versão do documento]
Autor: [Nome do autor]
Data: [Data de criação]

1. Introdução:
   - Objetivo: [Descreva o objetivo do plano de teste].
   - Escopo: [O que será testado e o que não será testado].
   - Referências: [Liste documentos de requisitos, normas, etc.].

2. Estratégia de Teste:
   - Níveis de Teste: [Unitário, Integração, Sistema, Aceitação].
   - Tipos de Teste: [Funcional, Desempenho, Segurança, etc.].
   - Critérios de Entrada: [Condições para iniciar os testes].
   - Critérios de Saída: [Condições para encerrar os testes].

3. Recursos:
   - Equipe: [Liste os membros da equipe de teste].
   - Ferramentas: [Liste as ferramentas de teste que serão utilizadas].
   - Ambiente: [Descreva o ambiente de teste (hardware, software, dados)].

4. Cronograma:
   - Datas de Início e Término: [Datas previstas para início e fim dos testes].
   - Marcos: [Liste os marcos importantes, como conclusão de fases de teste].

5. Riscos e Mitigação:
   - Riscos: [Liste os riscos identificados].
   - Mitigação: [Descreva as ações para mitigar os riscos].

6. Critérios de Aceitação:
   - [Descreva as condições para considerar os testes concluídos com sucesso].
```

### **Exemplo de Plano de Teste**:
```
Título: Plano de Teste para Sistema de Cadastro de Usuários
Versão: 1.0
Autor: João Silva
Data: 10/10/2023

1. Introdução:
   - Objetivo: Validar o sistema de cadastro de usuários.
   - Escopo: Testar funcionalidades de cadastro, edição e exclusão de usuários.
   - Referências: Documento de Requisitos v2.0, ISO/IEC 29119.

2. Estratégia de Teste:
   - Níveis de Teste: Teste de Sistema e Teste de Aceitação.
   - Tipos de Teste: Teste Funcional e Teste de Usabilidade.
   - Critérios de Entrada: Ambiente de teste configurado, casos de teste aprovados.
   - Critérios de Saída: Todos os casos de teste executados, defeitos críticos resolvidos.

3. Recursos:
   - Equipe: 2 testadores.
   - Ferramentas: Selenium, Jira.
   - Ambiente: Servidor Linux, banco de dados MySQL.

4. Cronograma:
   - Início: 01/10/2023.
   - Término: 15/10/2023.
   - Marcos: Conclusão dos testes de sistema em 10/10/2023.

5. Riscos e Mitigação:
   - Riscos: Atraso na entrega do ambiente de teste.
   - Mitigação: Preparar ambiente de teste com antecedência.

6. Critérios de Aceitação:
   - Todos os casos de teste devem ser aprovados.
   - Defeitos críticos devem ser resolvidos.
```

---

## **2. Test Case (Caso de Teste)**

### **O que é?**
O **Caso de Teste** descreve um cenário específico que será testado, com entradas, ações e resultados esperados.

### **Modelo Baseado na ISO/IEC 29119**:

```
ID do Caso de Teste: [Identificador único]
Descrição: [O que está sendo testado]
Pré-condições: [O que precisa estar pronto antes do teste]
Passos:
  1. [Passo 1]
  2. [Passo 2]
  3. [Passo 3]
Resultado Esperado: [O que o sistema deve fazer]
Resultado Obtido: [Preencher após execução]
Status: [Aprovado/Reprovado]
```

### **Exemplo de Caso de Teste**:
```
ID do Caso de Teste: TC001
Descrição: Cadastro de usuário com dados válidos.
Pré-condições: Sistema deve estar acessível.
Passos:
  1. Acessar a tela de cadastro.
  2. Preencher nome: "João Silva", email: "joao@exemplo.com", senha: "123456".
  3. Clicar em "Cadastrar".
Resultado Esperado: Mensagem "Cadastro realizado com sucesso".
Resultado Obtido: [Preencher após execução].
Status: [Preencher após execução].
```

---

## **3. Test Summary Report (Relatório Final de Testes)**

### **O que é?**
O **Relatório Final de Testes** resume os resultados dos testes realizados e fornece uma avaliação geral da qualidade do software.

### **Modelo Baseado na ISO/IEC 29119**:

```
Título: Relatório Final de Testes para [Nome do Projeto/Sistema]
Versão: [Versão do documento]
Autor: [Nome do autor]
Data: [Data de criação]

1. Objetivo:
   - [Descreva o propósito do relatório].

2. Escopo:
   - [O que foi testado].

3. Resultados:
   - Total de Casos de Teste: [Número total].
   - Aprovados: [Número de casos aprovados].
   - Reprovados: [Número de casos reprovados].

4. Defeitos Críticos:
   - [Liste os defeitos críticos encontrados].

5. Conclusão:
   - [Avaliação final e recomendações].
```

### **Exemplo de Relatório Final de Testes**:
```
Título: Relatório Final de Testes para Sistema de Cadastro de Usuários
Versão: 1.0
Autor: João Silva
Data: 15/10/2023

1. Objetivo:
   - Avaliar a qualidade do sistema de cadastro de usuários.

2. Escopo:
   - Funcionalidades de cadastro, edição e exclusão de usuários.

3. Resultados:
   - Total de Casos de Teste: 50
   - Aprovados: 45
   - Reprovados: 5

4. Defeitos Críticos:
   - DEF001: Login falha com credenciais válidas.

5. Conclusão:
   - O sistema está funcional, mas requer correções nos defeitos críticos antes da liberação.
```

---

## **4. Test Execution Report (Relatório de Execução de Testes)**

### **O que é?**
O **Relatório de Execução de Testes** documenta os resultados da execução dos casos de teste.

### **Modelo Baseado na ISO/IEC 29119**:

```
Título: Relatório de Execução de Testes para [Nome do Projeto/Sistema]
Versão: [Versão do documento]
Autor: [Nome do autor]
Data: [Data de criação]

1. Resumo:
   - Total de Casos de Teste: [Número total].
   - Aprovados: [Número de casos aprovados].
   - Reprovados: [Número de casos reprovados].

2. Detalhes:
   - [Lista de casos de teste com status].

3. Defeitos Encontrados:
   - [Lista de defeitos identificados].
```

### **Exemplo de Relatório de Execução de Testes**:
```
Título: Relatório de Execução de Testes para Sistema de Cadastro de Usuários
Versão: 1.0
Autor: João Silva
Data: 15/10/2023

1. Resumo:
   - Total de Casos de Teste: 50
   - Aprovados: 45
   - Reprovados: 5

2. Detalhes:
   - TC001: Aprovado
   - TC002: Reprovado (Defeito DEF001)

3. Defeitos Encontrados:
   - DEF001: Login falha com credenciais válidas.
```

---

## **5. Bug Report (Relatório de Defeitos)**

### **O que é?**
O **Relatório de Defeitos** documenta problemas encontrados durante os testes.

### **Modelo Baseado na ISO/IEC 29119**:

```
ID do Defeito: [Identificador único]
Título: [Descrição resumida do problema]
Descrição: [Detalhes do defeito]
Passos para Reproduzir:
  1. [Passo 1]
  2. [Passo 2]
  3. [Passo 3]
Evidências: [Screenshots, logs, vídeos]
Gravidade: [Crítica, Alta, Média, Baixa]
Prioridade: [Alta, Média, Baixa]
```

### **Exemplo de Relatório de Defeitos**:
```
ID do Defeito: DEF001
Título: Login falha com credenciais válidas.
Descrição: Ao inserir email e senha válidos, o sistema exibe "Credenciais inválidas".
Passos para Reproduzir:
  1. Acessar a tela de login.
  2. Inserir email: "teste@exemplo.com", senha: "123456".
  3. Clicar em "Entrar".
Evidências: Screenshot anexado.
Gravidade: Alta.
Prioridade: Alta.
```
