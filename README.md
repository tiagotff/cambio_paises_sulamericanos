# Soluções para Obtenção de Dados de Câmbio de países Sulamericanos

## Contexto

Uma limitação significativa foi identificada ao tentar obter dados de câmbio usando a API do Bacen, que oferece suporte apenas para um número limitado de valores e não inclui informações sobre as moedas da Argentina, Chile, Colômbia e Uruguai. Para superar essa limitação e garantir acesso completo aos dados necessários, foram desenvolvidas duas soluções alternativas.

## Motivação

A falta de dados de câmbio completos e atualizados para moedas específicas representa um desafio para análises financeiras e relatórios. Para resolver este problema, foram propostas duas abordagens que não dependem da API do Bacen:

1. **Web Scraping com Beautiful Soup**: Utiliza web scraping para coletar dados diretamente de sites financeiros, superando as limitações da API do Bacen.
2. **YFinance**: Aproveita a biblioteca YFinance para acessar dados financeiros do Yahoo Finance, fornecendo uma alternativa viável e sem limitações de dados.

Ambas as soluções são implementadas em Python e permitem a exportação dos dados para arquivos CSV no Google Drive, que podem ser facilmente integrados ao PowerBI para análise e visualização.

## Soluções Disponíveis

### 1. Web Scraping com Beautiful Soup

- **Descrição**: Obtém dados de câmbio de moedas de sites financeiros por meio de web scraping.
- **Requisitos**: Instalação das bibliotecas Beautiful Soup e Requests.
- **Funcionalidade**: O script lê os dados e salva um arquivo CSV no Google Drive com as taxas de câmbio.

### 2. YFinance

- **Descrição**: Usa a biblioteca YFinance para obter dados de câmbio diretamente do Yahoo Finance.
- **Requisitos**: Instalação da biblioteca YFinance.
- **Funcionalidade**: O script acessa as taxas de câmbio e salva um arquivo CSV no Google Drive. A biblioteca YFinance não possui limitações de dados como a API do Bacen.
