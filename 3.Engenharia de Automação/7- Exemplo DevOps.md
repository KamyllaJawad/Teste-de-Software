# Exemplo real de CI com testes automatizados usando GitHub Actions**, como se fosse para um projeto Python com `pytest`.

---

## 🗂️ Estrutura básica do projeto

```
meu_projeto/
├── app/
│   └── calculadora.py
├── tests/
│   └── test_calculadora.py
├── requirements.txt
└── .github/
    └── workflows/
        └── ci.yml
```

---

## 🧮 `app/calculadora.py`

```python
def soma(a, b):
    return a + b

def subtrai(a, b):
    return a - b
```

---

## ✅ `tests/test_calculadora.py`

```python
from app.calculadora import soma, subtrai

def test_soma():
    assert soma(3, 2) == 5

def test_subtrai():
    assert subtrai(5, 3) == 2
```

---

## 📦 `requirements.txt`

```txt
pytest
```

---

## ⚙️ `.github/workflows/ci.yml` – Pipeline no GitHub Actions

```yaml
name: CI - Testes Automatizados

on:
  push:
    branches: [ main ]
  pull_request:
    branches: [ main ]

jobs:
  rodar-testes:
    runs-on: ubuntu-latest

    steps:
    - name: Clonar o repositório
      uses: actions/checkout@v3

    - name: Instalar Python
      uses: actions/setup-python@v4
      with:
        python-version: '3.11'

    - name: Instalar dependências
      run: |
        pip install -r requirements.txt

    - name: Executar testes com Pytest
      run: |
        pytest
```

---

## 💥 O que acontece com esse exemplo?

1. Toda vez que você **der push** ou fizer um **pull request** na branch `main`, o GitHub executa:
   - Instala o Python
   - Instala as dependências (o `pytest`)
   - Executa os testes automatizados

2. Se algum teste falhar, a pipeline avisa ali mesmo no GitHub.

3. Se todos os testes passarem, você sabe que o código está funcionando corretamente — e pode seguir para o **delivery** ou **deployment** se quiser.
