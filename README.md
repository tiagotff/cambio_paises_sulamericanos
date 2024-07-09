# Soluções para Obtenção de Dados de Câmbio de Países Sul-americanos

## Contexto

Uma limitação significativa foi identificada ao tentar obter dados de câmbio usando a API do Bacen, que oferece suporte apenas para um número limitado de valores e não inclui informações sobre as moedas da Argentina, Chile, Colômbia e Uruguai. Para superar essa limitação e garantir acesso completo aos dados necessários, foram desenvolvidas três soluções alternativas.

## Motivação

A falta de dados de câmbio completos e atualizados para moedas específicas representa um desafio para análises financeiras e relatórios. Para resolver este problema, foram propostas três abordagens que não dependem da API do Bacen:

1. **Web Scraping com Beautiful Soup**: Utiliza web scraping para coletar dados diretamente de sites financeiros, superando as limitações da API do Bacen.
2. **YFinance**: Aproveita a biblioteca YFinance para acessar dados financeiros do Yahoo Finance, fornecendo uma alternativa viável e sem limitações de dados.
3. **Bacen - Fechamento PTAX 13h**: Acessa arquivo CSV do Bacen disponível em um link dinâmico da página, extraindo os dados por web scraping e salvando dois arquivos CSV no Google Drive.

Todas as soluções foram desenvolvidas no Google Colab e permitem a exportação dos dados para arquivos CSV no Google Drive, que podem ser facilmente integrados ao PowerBI para análise e visualização.

## Soluções Disponíveis

### 1. Web Scraping com Beautiful Soup

- **Descrição**: Obtém dados de câmbio de moedas de sites financeiros por meio de web scraping.
- **Requisitos**: Instalação das bibliotecas Beautiful Soup e Requests.
- **Funcionalidade**: O script lê os dados e salva um arquivo CSV no Google Drive com as taxas de câmbio.
- **Link para o Colab**: [Solução com Beautiful Soup](https://colab.research.google.com/drive/1x_kqz1pf3QvnshXzdlF52cUsREUEvGxX?usp=sharing)

### 2. YFinance

- **Descrição**: Usa a biblioteca YFinance para obter dados de câmbio diretamente do Yahoo Finance.
- **Requisitos**: Instalação da biblioteca YFinance.
- **Funcionalidade**: O script acessa as taxas de câmbio e salva um arquivo CSV no Google Drive. A biblioteca YFinance não possui limitações de dados como a API do Bacen.
- **Link para o Colab**: [Solução com YFinance](https://colab.research.google.com/drive/1udK4yzdISaxIczA5nee33JYdrvc8UfBo?usp=sharing)

### 3. Bacen - Fechamento PTAX 13h

- **Descrição**: Acessa arquivo CSV do Bacen disponível em um link dinâmico da página, extraindo os dados por web scraping e salvando dois arquivos CSV no Google Drive: um com todos os dados extraídos ('Bacen.csv') e outro com a cotação das moedas desejadas ('Bacen_13h').
- **Requisitos**: Instalação das bibliotecas Beautiful Soup e Requests.
- **Funcionalidade**: O script lê os dados e salva dois arquivos CSV no Google Drive com as taxas de câmbio.
- **Link para o Colab**: [Solução Bacen - Fechamento PTAX 13h](https://colab.research.google.com/drive/10wYcfw-mwU3YzgKX1JCWGXmZY9xQt-sO?usp=sharing)

## Local de Armazenamento dos Arquivos CSV

Os arquivos CSV gerados pelos scripts são salvos no Google Drive. Você pode acessar a pasta onde os arquivos são armazenados através do seguinte link:

- [Pasta do Google Drive](https://drive.google.com/drive/folders/1db0frdNn7SRM_cIZh-RmFjjQjcet0FlX?usp=sharing)
