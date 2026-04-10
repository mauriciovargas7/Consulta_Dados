# 🚀 Consulta Inteligente de Dados com IA (SQL + NLP)

![Status](https://img.shields.io/badge/status-em%20desenvolvimento-yellow) ![Python](https://img.shields.io/badge/python-3.11-blue) ![AI](https://img.shields.io/badge/AI-OpenAI-orange) ![License](https://img.shields.io/badge/license-MIT-green)

Sistema em desenvolvimento que permite realizar consultas em banco de dados utilizando **linguagem natural**, convertendo automaticamente perguntas em **queries SQL** através de Inteligência Artificial.

---

## 🧠 Visão Geral

Este projeto está sendo desenvolvido com o objetivo de **automatizar análises de dados** e reduzir a dependência de consultas manuais em SQL.

A ideia é permitir que qualquer usuário consiga:

- Fazer perguntas como:  
  👉 "Qual a média de valor realizado?"  
  👉 "Total por mês?"  

- E obter respostas diretamente do banco de dados, sem precisar escrever SQL manualmente.

---

## 🚧 Status do Projeto

🟡 **EM DESENVOLVIMENTO**

Atualmente o projeto está em fase de construção e testes, com algumas funcionalidades já implementadas:

✔ Conexão com banco de dados (SQL Server)  
✔ Leitura de dados com Pandas  
✔ Estrutura inicial de interpretação com IA  
✔ Testes com PandasAI  

🚧 Em andamento:

- Integração completa com OpenAI  
- Geração confiável de SQL via linguagem natural  
- Tratamento de erros e validação de queries  
- Estruturação do código  

---

## 🎬 Demonstração

*(Em breve — será adicionado um GIF ou vídeo com o funcionamento do sistema)*

---

## ⚙️ Tecnologias Utilizadas

- Python  
- Pandas → manipulação de dados  
- PyODBC → conexão com SQL Server  
- OpenAI API → geração automática de SQL  
- PandasAI → análise inteligente de DataFrames  
- Excel → configuração dinâmica do ambiente  

---

## 🏗️ Arquitetura

O sistema segue o fluxo:

1. Entrada em linguagem natural  
2. Interpretação via IA (OpenAI / PandasAI)  
3. Conversão para SQL  
4. Execução no banco de dados  
5. Retorno estruturado  

---

## 🔄 Funcionamento

### 1. 🔌 Conexão com Banco de Dados

As configurações são carregadas via arquivo `config.xlsx`:

```python
df_config = pd.read_excel("config.xlsx")