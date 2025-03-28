# **Atividade Prática de Teste de Software - Planejamento e Documentação**

## **Objetivo da Atividade:**
Desenvolver habilidades fundamentais em planejamento, execução e documentação de testes manuais, com foco especial na qualidade da documentação.

## **Duração:**
2-3 horas

## **Materiais Necessários:**
- Computador com acesso à internet
- Navegador web (Chrome, Firefox ou Edge)
- Editor de texto (Word, Google Docs ou Bloco de Notas)
- Ferramenta para captura de tela (tecla "Print Screen" ou ferramenta de captura do Windows/Mac)

---

## **Passo a Passo da Atividade:**

### **1. Escolha do Sistema para Testar**
Acesse o site [Cantinho das QAs](https://www.cantinhodasqas.com.br/sites-para-praticar) e selecione UM dos seguintes sistemas simples para praticar:
- ![Sistemas para Testar](../assets/Captura%20de%20tela%202025-03-25%20000830.png)
- ![Sistemas para Testar](../assets/Captura%20de%20tela%202025-03-25%20000851.png)

### **2. Planejamento Básico de Testes**
Complete a tabela abaixo no seu documento:

| Item | Descrição |
|------|-----------|
| Sistema escolhido: | [Nome do sistema] |
| Funcionalidade a testar: | [Ex: Login, Cadastro de usuário] |
| Objetivo do teste: | [O que você quer verificar?] |
| Ambiente de teste: | [Navegador, versão, sistema operacional] |

### **3. Criação de Casos de Teste Simples**
Crie 3 casos de teste usando o modelo abaixo para a funcionalidade escolhida:

**Modelo de Caso de Teste:**

```markdown
### Caso de Teste 1
**Descrição:** [O que será testado?]  
**Pré-condições:** [O que precisa estar pronto antes?]  
**Passos:**
1. [Passo 1]
2. [Passo 2] 
3. [Passo 3]
**Resultado esperado:** [O que deve acontecer?]
```

**Exemplo Prático (para login):**
```markdown
### Caso de Teste 1
**Descrição:** Login com credenciais válidas  
**Pré-condições:** Usuário já cadastrado  
**Passos:**
1. Acessar a página de login
2. Inserir email válido
3. Inserir senha válida
4. Clicar em "Entrar"  
**Resultado esperado:** Sistema redireciona para página inicial
```

### **4. Execução dos Testes**
Execute cada caso de teste e registre:

| Caso de Teste | Resultado Obtido | Status (✔/✖) | Evidência (print) |
|---------------|------------------|--------------|-------------------|
| CT1 | [Descreva o que aconteceu] | [✔ ou ✖] | [Nome do arquivo] |
| CT2 | ... | ... | ... |

### **5. Relatório de Defeitos (se encontrar problemas)**
Para cada falha encontrada, preencha:

```markdown
**Defeito encontrado em:** [Data]  
**Local:** [Onde ocorreu?]  
**Descrição:** [O que aconteceu de errado?]  
**Passos para reproduzir:**
1. [Passo 1]
2. [Passo 2]
**Gravidade:** ( ) Baixa ( ) Média ( ) Alta  
**Evidência:** [Anexe print]  
```

### **6. Conclusão**
Responda em 3-5 frases:
1. O que você aprendeu com esta atividade?
2. Qual parte foi mais desafiadora?
3. Como você poderia melhorar seus testes na próxima vez?

---

## **Critérios de Avaliação Simplificados:**

| Critério | Pontos |
|----------|--------|
| Completude dos casos de teste (3 casos) | 30 |
| Clareza na descrição dos passos | 20 |
| Qualidade das evidências (prints) | 20 |
| Detalhamento dos defeitos encontrados | 20 |
| Reflexão na conclusão | 10 |

**Total:** 100 pontos

---

## **Dicas para Boa Documentação:**
1. Seja específico nos passos ("Clicar no botão X" em vez de "Clicar no botão")
2. Nomeie os arquivos de evidência de forma organizada (ex: "CT1-login-valido.jpg")
3. Use linguagem simples e objetiva
4. Revise seu trabalho antes de enviar

> "Documentar bem é tão importante quanto executar os testes - é assim que comunicamos nossos achados!" 

**Pronto para começar?** Escolha seu sistema e mãos à obra! 🚀