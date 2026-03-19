🌟 Principais Funcionalidades:
Processamento ETL Inteligente: O sistema realiza a Extração, Transformação e Carga (ETL) dos dados brutos, corrigindo automaticamente variações de cabeçalho entre diferentes anos e meses (leitura flexível de linhas 3 ou 4).

Limpeza e Padronização: Algoritmo que remove acentos, espaços extras e padroniza nomes de municípios e colunas, garantindo 100% de precisão na filtragem da cidade de São Paulo.

Cache em Memória (Performance): Implementação de um "banco de dados temporário" (dicionário de DataFrames). O sistema carrega todos os anos da pasta uma única vez e permite consultas instantâneas de meses específicos sem precisar ler os arquivos do Drive novamente.

Categorização Customizada: Agrupamento técnico de mais de 20 tipos de veículos em 5 categorias gerenciais (Motocicletas, Automóveis, Ônibus, Caminhões e Outros).

🛠️ Tecnologias Utilizadas:
Python: Linguagem base.

Pandas: Manipulação de grandes volumes de dados.

Google Colab & Drive API: Ambiente de nuvem e armazenamento.

OS & Warnings: Gestão de sistema de arquivos e limpeza de logs.
