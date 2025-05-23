# Fine-Tuning SQL Generator 🚀

[![Python](https://img.shields.io/badge/python-3.8%2B-blue.svg)](https://www.python.org/)

Um projeto para ajuste fino (*fine-tuning*) de um modelo de linguagem natural para geração automática de queries SQL a partir de comandos em português, utilizando a biblioteca [Unsloth](https://github.com/unslothai/unsloth).

---

## ✨ Visão Geral

O **Fine-Tuning SQL Generator** visa treinar um modelo LLM capaz de interpretar comandos em linguagem natural (PT-BR) e convertê-los para SQL, democratizando o acesso a bancos de dados e reduzindo barreiras técnicas para usuários de diferentes perfis.

---

## 📚 Tecnologias Utilizadas

* [Python 3.8+](https://www.python.org/)
* [Unsloth](https://github.com/unslothai/unsloth)
* [PyTorch](https://pytorch.org/)
* [Transformers (Hugging Face)](https://huggingface.co/docs/transformers/index)
* Outras dependências: `accelerate`, `bitsandbytes`, `trl`, `peft`, `xformers`, `triton`

---

## ⚡ Instalação e Uso

### 1. Clone o repositório

```bash
git clone https://github.com/Joaovmir/finetuning_sql_generator.git
cd finetuning_sql_generator
```

### 2. Instale as dependências

No Google Colab, basta executar as primeiras células do notebook.

Para rodar localmente, utilize:

```bash
pip install unsloth torch xformers trl peft accelerate bitsandbytes triton
```

### 3. Execute o Notebook

Abra o arquivo `finetuning_sql_generator.ipynb` em seu ambiente preferido (Jupyter, VS Code ou Colab) e execute célula por célula.

---

## 💡 Exemplo de Uso

Após o *fine-tuning*, gere queries SQL a partir de instruções em português:

**Entrada:**

> Liste todos os pedidos feitos em março de 2024 pelo cliente João.

**Saída esperada:**

```sql
SELECT * FROM pedidos WHERE cliente = 'João' AND data_pedido BETWEEN '2024-03-01' AND '2024-03-31';
```

---

## 📁 Estrutura do Projeto

```
finetuning_sql_generator/
├── finetuning_sql_generator.ipynb
├── README.md
```

