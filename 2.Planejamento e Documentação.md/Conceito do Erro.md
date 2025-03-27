## **1️⃣ O que é um Bug?**  
Um **bug** é um erro ou defeito no código de um software que causa um comportamento inesperado ou incorreto. Ele ocorre devido a problemas na programação, lógica ou implementação.  

📌 **Exemplo de bug:**  
- Um botão de "Adicionar ao carrinho" em um e-commerce não adiciona o produto corretamente.  
- Um aplicativo de banco exibe um saldo incorreto porque um cálculo matemático foi feito de forma errada no código.  

**Bugs são sempre falhas técnicas do código-fonte!**  

---

## **2️⃣ O que são Falhas?**  
Uma **falha** é qualquer defeito que afeta o funcionamento correto do software, podendo ser causada por bugs, erros de design, má implementação ou até mesmo problemas externos, como falha de hardware ou rede.  

📌 **Exemplo de falha:**  
- O site de um banco fica inacessível porque os servidores não suportam muitos acessos simultâneos (falha de infraestrutura).  
- Um aplicativo de mensagens exibe textos desalinhados porque o design não foi adaptado para telas menores (falha de usabilidade).  

🔹 **Diferença principal:**  
- **Bug** = Erro de programação no código-fonte.  
- **Falha** = Problema percebido no funcionamento do software, podendo ou não ser causado por um bug.  

---

## **3️⃣ Classificação das Falhas**  
Podemos classificar falhas em várias categorias. Aqui estão algumas das principais:  

### **🔹 1. Falha Funcional**  
O sistema não faz o que deveria fazer.  

📌 **Exemplo:**  
- Um formulário de cadastro não salva as informações do usuário após o preenchimento.  
- Um aplicativo de delivery não exibe o status correto do pedido.  

💡 **Causa:** Geralmente causada por bugs no código.  

---

### **🔹 2. Falha de Desempenho (Performance)**  
O software funciona, mas é lento ou consome muitos recursos.  

📌 **Exemplo:**  
- Um aplicativo de e-commerce demora 10 segundos para carregar os produtos.  
- Um site trava quando muitas pessoas tentam acessá-lo ao mesmo tempo.  

💡 **Causa:** Problemas na otimização do código ou infraestrutura insuficiente.  

---

### **🔹 3. Falha de Usabilidade**  
O sistema é difícil de usar, confuso ou não segue boas práticas de design.  

📌 **Exemplo:**  
- Um botão de "Confirmar" e um de "Cancelar" têm cores muito parecidas, confundindo o usuário.  
- Um site de agendamento não deixa claro quais datas estão disponíveis.  

💡 **Causa:** Má concepção da interface ou falta de testes com usuários.  

---

### **🔹 4. Falha de Segurança**  
O sistema permite acessos indevidos, exposição de dados ou outras vulnerabilidades.  

📌 **Exemplo:**  
- Um usuário consegue acessar dados bancários de outro cliente.  
- Um site não criptografa as senhas dos usuários corretamente.  

💡 **Causa:** Falta de medidas de segurança na implementação.  

---

### **🔹 5. Falha de Compatibilidade**  
O software funciona em um ambiente, mas apresenta problemas em outros dispositivos, navegadores ou sistemas operacionais.  

📌 **Exemplo:**  
- Um site funciona bem no Google Chrome, mas quebra no Firefox.  
- Um aplicativo não roda corretamente em celulares mais antigos.  

💡 **Causa:** Testes insuficientes em diferentes plataformas.  

---

### **🔹 6. Falha de Confiabilidade e Estabilidade**  
O sistema apresenta erros imprevisíveis ou para de funcionar sem motivo aparente.  

📌 **Exemplo:**  
- Um jogo de celular fecha sozinho depois de alguns minutos de uso.  
- Um software de contabilidade gera relatórios corrompidos.  

💡 **Causa:** Problemas na arquitetura do software, uso incorreto de memória, entre outros.  

---

## **4️⃣ Tabelinha de Memorização:**  

| Tipo | O que é | Exemplo |
|------|--------|---------|
| **Bug** | Erro no código-fonte que causa um comportamento inesperado. | Um cálculo errado exibe um saldo bancário incorreto. |
| **Falha Funcional** | O sistema não faz o que deveria. | Um botão de "enviar mensagem" que não funciona. |
| **Falha de Desempenho** | O sistema é lento ou trava. | Um site demora para carregar produtos. |
| **Falha de Usabilidade** | O sistema é difícil de usar. | Ícones confusos em um aplicativo. |
| **Falha de Segurança** | O sistema é vulnerável a ataques. | Senhas armazenadas sem criptografia. |
| **Falha de Compatibilidade** | O software não funciona em todos os ambientes. | Um site quebra em determinados navegadores. |
| **Falha de Confiabilidade** | O sistema se comporta de forma imprevisível. | Um jogo que fecha sozinho do nada. |

---

## **Sendo assim...**  
- **Todo bug é uma falha, mas nem toda falha é um bug.**  
- As falhas podem ser causadas por bugs no código, mas também podem surgir devido a infraestrutura inadequada, má concepção do sistema ou falta de testes adequados.  
- Para garantir qualidade, é essencial aplicar diferentes tipos de testes para identificar e corrigir esses problemas antes que o software seja lançado.  

---

# Criação de Relatos de Defeitos (Bug Reports) Estruturados

A **ISO/IEC 29119** é um conjunto de normas internacionais para **teste de software**, incluindo diretrizes para a **documentação de defeitos (bug reports)**. Com base nela, cada tipo de falha deve ser documentado de forma estruturada para garantir que os problemas sejam rastreados, analisados e corrigidos de maneira eficiente.  

Abaixo, temos **templates vazios** para diferentes tipos de falhas e um **exemplo preenchido**.  

---

## **📌 Template Geral de Relato de Defeito (Bug Report) – Baseado na ISO/IEC 29119**  
(Este template pode ser usado para qualquer tipo de falha.)  

### **Identificação**  
- **ID do Defeito:** [Número único do defeito]  
- **Título:** [Descrição breve e clara do problema]  
- **Categoria:** [Funcional / Performance / Usabilidade / Segurança / Compatibilidade / Confiabilidade]  
- **Gravidade:** [Baixa / Média / Alta / Crítica]  
- **Prioridade:** [Baixa / Média / Alta]  
- **Status:** [Aberto / Em andamento / Resolvido / Fechado]  

### **Descrição do Problema**  
- **Descrição Resumida:** [Breve explicação do erro]  
- **Passos para Reproduzir:**  
  1. [Passo 1]  
  2. [Passo 2]  
  3. [Passo 3]  
- **Resultado Esperado:** [O que deveria acontecer]  
- **Resultado Obtido:** [O que aconteceu de fato]  

### **Ambiente de Teste**  
- **Sistema Operacional:** [Windows/Linux/macOS, versão]  
- **Dispositivo/Navegador:** [PC, Mobile, Chrome, Firefox, etc.]  
- **Versão do Software:** [Número da versão]  
- **Conectividade:** [Wi-Fi, 4G, etc.]  
- **Outros Detalhes:** [Se necessário]  

### **Anexos**  
- [Capturas de tela / Vídeo / Logs de erro, se disponíveis]  

---

## **📌 Template de Relato de Defeito por Tipo de Falha**  

### **1️⃣ Falha Funcional**  
- **Título:** [Descrição clara do problema funcional]  
- **Descrição:** O sistema não realiza uma ação que deveria.  
- **Passos para Reproduzir:** [Lista de ações]  
- **Resultado Esperado:** [O que deveria acontecer]  
- **Resultado Obtido:** [O que acontece na prática]  
- **Impacto:** [O que essa falha impede? Ex.: não permite o cadastro de usuários]  

---

### **2️⃣ Falha de Desempenho (Performance)**  
- **Título:** [O sistema apresenta lentidão ou consumo excessivo]  
- **Descrição:** [Exemplo: A página de login demora 10 segundos para carregar]  
- **Medições:** [Se possível, inclua tempo de resposta, consumo de memória, CPU]  
- **Impacto:** [Como isso afeta o usuário? Ex.: experiência ruim, tempo de espera longo]  

---

### **3️⃣ Falha de Usabilidade**  
- **Título:** [O sistema é difícil/confuso de usar]  
- **Descrição:** [Exemplo: Botão "Confirmar" e "Cancelar" têm cores iguais, confundindo o usuário]  
- **Sugestão de Melhoria:** [O que pode ser feito para resolver?]  

---

### **4️⃣ Falha de Segurança**  
- **Título:** [Falha que compromete a segurança]  
- **Descrição:** [Exemplo: Usuários conseguem visualizar dados de outras contas]  
- **Impacto:** [Exemplo: Exposição de dados sensíveis]  
- **Recomendações:** [Exemplo: Implementar autenticação reforçada]  

---

### **5️⃣ Falha de Compatibilidade**  
- **Título:** [Problema que ocorre em um navegador/sistema específico]  
- **Descrição:** [Exemplo: O site quebra no Safari, mas funciona no Chrome]  
- **Ambiente:** [SO, navegador, versão]  
- **Impacto:** [Usuários de determinada plataforma não conseguem acessar o sistema]  

---

### **6️⃣ Falha de Confiabilidade e Estabilidade**  
- **Título:** [O sistema se comporta de forma imprevisível]  
- **Descrição:** [Exemplo: Aplicativo fecha sozinho após 5 minutos]  
- **Passos para Reproduzir:** [Se aplicável]  
- **Impacto:** [Exemplo: Usuários perdem progresso e precisam reiniciar o app]  

---

## **📌 Exemplo Preenchido** (Falha Funcional)  

### **Identificação**  
- **ID do Defeito:** #1023  
- **Título:** Erro ao adicionar produto ao carrinho no e-commerce  
- **Categoria:** Falha Funcional  
- **Gravidade:** Alta  
- **Prioridade:** Alta  
- **Status:** Aberto  

### **Descrição do Problema**  
- **Descrição Resumida:** Ao tentar adicionar um item ao carrinho, ele não aparece na página de checkout.  
- **Passos para Reproduzir:**  
  1. Acesse o site www.lojavirtual.com  
  2. Escolha qualquer produto e clique em "Adicionar ao carrinho"  
  3. Vá até a página de checkout  
- **Resultado Esperado:** O produto deveria ser exibido no carrinho.  
- **Resultado Obtido:** O carrinho aparece vazio.  

### **Ambiente de Teste**  
- **Sistema Operacional:** Windows 11  
- **Navegador:** Google Chrome 120.0.6099.224  
- **Versão do Software:** Loja Virtual v3.1.2  
- **Conectividade:** Wi-Fi 100 Mbps  

### **Anexos**  
- Captura de tela mostrando o carrinho vazio após adicionar um item.  
- Vídeo gravado reproduzindo o erro.  

