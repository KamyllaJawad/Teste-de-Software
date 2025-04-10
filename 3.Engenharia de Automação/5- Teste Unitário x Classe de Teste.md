## **1. O que é um Teste Unitário?**

### **Definição**:
Um **teste unitário** é um tipo de teste que verifica o funcionamento de uma **unidade individual** do código, como uma função, método ou classe. O objetivo é garantir que essa unidade funcione corretamente de forma isolada.

### **Características**:
- Foca em pequenas partes do código.
- É rápido de executar.
- Deve ser independente de outras partes do sistema.

### **Exemplo em Python**:
Suponha que temos uma função simples que soma dois números:

```python
def soma(a, b):
    return a + b
```

Um teste unitário para essa função poderia ser:

```python
import unittest

class TestSoma(unittest.TestCase):
    def test_soma_positivos(self):
        self.assertEqual(soma(2, 3), 5)  # Verifica se 2 + 3 = 5

    def test_soma_negativos(self):
        self.assertEqual(soma(-1, -1), -2)  # Verifica se -1 + (-1) = -2

if __name__ == '__main__':
    unittest.main()
```

Neste exemplo:
- A função `soma` é a **unidade** sendo testada.
- Os métodos `test_soma_positivos` e `test_soma_negativos` são os **testes unitários**.

---

## **2. O que é uma Classe de Teste?**

### **Definição**:
Uma **classe de teste** é uma estrutura que agrupa vários testes unitários (ou outros tipos de testes) relacionados. Ela serve para organizar os testes de forma lógica e modular.

### **Características**:
- Agrupa testes que verificam funcionalidades relacionadas.
- Facilita a manutenção e a execução dos testes.
- Pode conter métodos de configuração (setup) e limpeza (teardown).

### **Exemplo em Python**:
Vamos expandir o exemplo anterior para incluir uma classe de teste que agrupa testes unitários para diferentes funções matemáticas:

```python
import unittest

# Funções que serão testadas
def soma(a, b):
    return a + b

def subtracao(a, b):
    return a - b

# Classe de teste
class TestOperacoesMatematicas(unittest.TestCase):
    def test_soma_positivos(self):
        self.assertEqual(soma(2, 3), 5)  # Teste unitário para soma

    def test_soma_negativos(self):
        self.assertEqual(soma(-1, -1), -2)  # Teste unitário para soma

    def test_subtracao_positivos(self):
        self.assertEqual(subtracao(5, 3), 2)  # Teste unitário para subtração

    def test_subtracao_negativos(self):
        self.assertEqual(subtracao(-1, -1), 0)  # Teste unitário para subtração

if __name__ == '__main__':
    unittest.main()
```

Neste exemplo:
- A classe `TestOperacoesMatematicas` é uma **classe de teste**.
- Ela agrupa vários **testes unitários** (`test_soma_positivos`, `test_soma_negativos`, etc.) que verificam diferentes funcionalidades relacionadas (soma e subtração).

---

## **3. Diferença entre Classe de Teste e Teste Unitário**

| **Aspecto**            | **Teste Unitário**                          | **Classe de Teste**                          |
|------------------------|---------------------------------------------|---------------------------------------------|
| **O que é?**           | Um teste individual que verifica uma unidade do código. | Uma estrutura que agrupa vários testes unitários ou outros tipos de testes. |
| **Escopo**             | Pequeno (uma função, método ou classe).     | Mais amplo (agrupa testes relacionados).    |
| **Organização**        | Não organiza outros testes.                 | Organiza testes de forma lógica e modular.  |
| **Exemplo**            | `test_soma_positivos`.                      | `TestOperacoesMatematicas`.                 |


