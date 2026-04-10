# 🚀 Consulta Inteligente de Dados com IA (SQL + NLP)

Sistema em produção que permite realizar consultas em banco de dados utilizando **linguagem natural**, convertendo automaticamente perguntas em **queries SQL** através de Inteligência Artificial.

---

## 🧠 Visão Geral

Este projeto foi desenvolvido para **automatizar análises de dados** e reduzir a dependência de consultas manuais em SQL.

Com ele, é possível:

- Fazer perguntas como:  
  👉 "Qual a média de valor realizado?"  
  👉 "Total por mês?"  

- E obter respostas diretamente do banco de dados, sem escrever SQL manualmente.

---

## ⚙️ Tecnologias Utilizadas

- Python  
- Pandas → manipulação de dados  
- PyODBC → conexão com SQL Server  
- OpenAI API → geração automática de SQL  
- PandasAI → análise inteligente de DataFrames  
- Excel → configuração dinâmica do ambiente  

---

## 🔄 Funcionamento

### 1. 🔌 Conexão com Banco de Dados
As configurações são carregadas via arquivo `config.xlsx`, permitindo flexibilidade e desacoplamento do código.

```python
df_config = pd.read_excel("config.xlsx")