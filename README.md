# Soluções para Obtenção de Dados de Câmbio

Este repositório contém duas soluções alternativas para obter dados de câmbio para moedas da Argentina, Chile, Colômbia e Uruguai. Ambas as soluções são implementadas em Python e salvam os dados em arquivos CSV no Google Drive, que podem ser importados diretamente no PowerBI.

## Soluções Disponíveis

### 1. Web Scraping com Beautiful Soup

- **Descrição**: Obtém dados de câmbio de moedas de sites financeiros por meio de web scraping.
- **Requisitos**: Instalação das bibliotecas Beautiful Soup e Requests.
- **Funcionalidade**: O script lê os dados e salva um arquivo CSV no Google Drive com as taxas de câmbio.

### 2. YFinance

- **Descrição**: Usa a biblioteca YFinance para obter dados de câmbio diretamente do Yahoo Finance.
- **Requisitos**: Instalação da biblioteca YFinance.
- **Funcionalidade**: O script acessa as taxas de câmbio e salva um arquivo CSV no Google Drive. A biblioteca YFinance não possui limitações de dados como a API do Bacen.
