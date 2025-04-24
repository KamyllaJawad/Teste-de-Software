# 🧭 Caminho das Pedras – Etapas e Recursos Sugeridos

## 📌 1. Escolha do Projeto

Selecionar um sistema da tabela abaixo (todos gratuitos, open source e próprios para testes):

#### 🔍 **Tabela de Projetos para Testes Automatizados**

| #  | Projeto                                | Link                                                        | O que praticar                                                       | Ferramentas Sugeridas                      |
|----|----------------------------------------|-------------------------------------------------------------|------------------------------------------------------------------------|--------------------------------------------|
| 1  | TodoMVC                                | https://todomvc.com                                         | CRUD, filtros, visibilidade                                           | **Cypress**, Selenium, Robot               |
| 2  | Books To Scrape                        | https://books.toscrape.com                                  | Navegação, scraping, paginação                                       | **Selenium**, Cypress, Robot               |
| 3  | RealWorld App (frontend)               | https://github.com/gothinkster/realworld                    | Login, postagens, comentários, perfis                                | **Cypress**, Selenium                      |
| 4  | SauceDemo                              | https://www.saucedemo.com/                                  | Login, carrinho, checkout                                            | **Cypress**, Selenium, Robot               |
| 5  | OrangeHRM                              | https://github.com/orangehrm/orangehrm                      | RH, permissões, formulários                                          | **Selenium**, Robot Framework              |
| 6  | Advantage Demo Store                   | https://advantageonlineshopping.com/#/                      | Loja, busca, carrinho, login                                         | **Cypress**, Selenium                      |
| 7  | Demo Blaze                             | https://www.demoblaze.com/                                  | Compra, alertas, validação                                           | **Selenium**, Cypress, Robot               |
| 8  | Automation in Testing (Hotel)          | https://automationintesting.online/                         | Reserva de hotel, backoffice                                         | **Robot**, Selenium                        |
| 9  | The Internet (Herokuapp)               | https://the-internet.herokuapp.com/                         | Uploads, waits, alerts, autenticação                                 | **Cypress**, Selenium, Robot               |
| 10 | UI Test Automation Playground          | http://uitestingplayground.com/                             | UI dinâmica, botões, scroll                                          | **Cypress**, Selenium, Robot               |
| 11 | Appium Test App                        | https://github.com/appium/sample-code/tree/master/sample-code/apps | Elementos básicos mobile Android/iOS                         | **Appium**                                  |
| 12 | Android API Demos                      | https://github.com/appium/android-apidemos                  | Componentes nativos Android                                          | **Appium**                                  |
| 13 | Swag Labs Mobile (Sauce)               | https://github.com/saucelabs/sample-app-mobile              | App mobile de e-commerce                                             | **Appium**                                  |
| 14 | Wikipedia App                          | https://github.com/wikimedia/apps-android-wikipedia         | Busca, leitura, temas, navegação                                     | **Appium**                                  |
| 15 | Expo Go                                | https://expo.dev/client                                     | Aplicativos híbridos (React Native)                                  | **Appium** (com setup RN)                   |

---

## 🧰 2. Escolha da Ferramenta

Ferramenta adequada ao tipo de sistema:

| Tipo de Teste | Ferramentas Sugeridas |
|---------------|------------------------|
| Web (UI)      | **Cypress**, **Selenium**, **Robot Framework** |
| Mobile        | **Appium**             |
| API           | **Postman**, **Pytest**, **Robot Framework** com `RequestsLibrary` |


## 🧪 3. Planejamento dos Testes

Baseado na norma **ISO/IEC 29119-3**:
- Objetivos
- Itens de teste
- Critérios de entrada/saída
- Casos de Teste (passos, dados, resultado esperado)
- Ambiente de testes

📄 **Modelo de Plano**: [Exemplo Google Docs](https://docs.google.com/document/d/1guJpzNq59bXtFTMp0WZVRcNQe0W7gHHAlfvZyTQowEo/edit)

## 💻 4. Implementação dos Testes

Praticar com a ferramenta escolhida:
- Cypress: https://docs.cypress.io/guides/overview/why-cypress
- Selenium: https://www.selenium.dev/documentation/webdriver/
- Robot: https://robotframework.org/
- Appium: https://appium.io/docs/en/about-appium/intro/

## 📊 5. Execução e Evidências

- Prints das execuções
- Logs gerados
- Relatórios (Cypress: automático; Robot: HTML; Appium: logs + vídeo se integrado ao CI)

## 📝 6. Documentação Final

- Plano de Testes
- Casos de Teste
- Evidências (prints, logs, vídeo)
- Análise de falhas e correções
- Conclusões e aprendizados

## 🎤 7. Apresentação Final

Dicas:
- Mostre o sistema escolhido
- Explique a ferramenta usada
- Mostre os testes funcionando
- Destaque falhas encontradas e como podem ser tratadas
- Compartilhe aprendizados
