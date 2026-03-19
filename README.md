# 🚗 Sistema de Inteligência de Frota - São Paulo (DETRAN/SENATRAN)

[![Python](https://img.shields.io/badge/Python-3.8+-3776AB?style=flat&logo=python&logoColor=white)](https://www.python.org/)
[![Pandas](https://img.shields.io/badge/Pandas-2.0+-15212B?style=flat&logo=pandas&logoColor=white)](https://pandas.pydata.org/)
[![Google Colab](https://img.shields.io/badge/Google%20Colab-F9AB00?style=flat&logo=googlecolab&logoColor=white)](https://colab.research.google.com/)

Este projeto automatiza a extração, tratamento e análise de dados de frotas veiculares do município de São Paulo. Ele transforma planilhas brutas e despadronizadas do governo em um banco de dados otimizado para consultas gerenciais instantâneas.

## 🚀 Diferenciais do Projeto

* **⚡ Cache em Memória (Data Warehouse):** Diferente de scripts comuns, este sistema realiza o carregamento dos anos selecionados para a memória RAM. Uma vez carregado, as consultas de meses específicos levam milissegundos, pois não dependem mais da leitura de arquivos no Drive.
* **🛠️ ETL Resiliente:** O algoritmo detecta automaticamente se o cabeçalho da planilha está na linha 3 ou 4, evitando quebras por mudanças de padrão do fornecedor dos dados.
* **🧹 Higienização de Dados:** Processo automático de remoção de acentos, espaços em branco e padronização de caracteres (*Sanitization*), garantindo que nomes como "SÃO PAULO" ou "SAO PAULO " sejam lidos corretamente.
* **📈 Categorização Gerencial:** Agrupa mais de 20 subcategorias de veículos em 5 grupos estratégicos: **Motocicletas, Automóveis, Ônibus, Caminhões e Outros**.

## 📂 Estrutura do Notebook (Google Colab)

O projeto foi desmembrado em células para máxima eficiência:

1.  **Configurações e Funções:** Importação de bibliotecas e definição do motor de cálculo.
2.  **Carga Automática:** Varredura automática da pasta do Drive e carregamento dos dados para a memória.
3.  **Painel de Consulta:** Interface simples para o usuário definir o ano e mês alvo.
4.  **Monitor de Resultados:** Exibição instantânea das tabelas formatadas.

## 🛠️ Tecnologias Utilizadas

* **Python 3**
* **Pandas** (Tratamento de dados)
* **OS & Warnings** (Gestão de arquivos e logs)
* **Google Drive API** (Integração de armazenamento)

## 📋 Como utilizar

1.  Suba as planilhas do DETRAN para a pasta `/onbording/Tabelas_Frota_Geral/` no seu Drive.
2.  Execute a **Célula 1** para preparar o ambiente.
3.  Execute a **Célula 2** para que o Python processe todos os anos disponíveis.
4.  Use as **Células 3 e 4** para realizar consultas rápidas por Ano ou Mês.

---
⭐ *Projeto desenvolvido para otimização de processos de onboarding e análise de dados governamentais.*
