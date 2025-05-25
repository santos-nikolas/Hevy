# Análise Interativa de Progresso de Treinos - Hevy Data Visualizer

![Badge de Licença](https://img.shields.io/badge/license-MIT-blue.svg) <!-- Opcional: Escolha uma licença -->
![Python Version](https://img.shields.io/badge/python-3.8+-blue.svg) <!-- Opcional: Versão do Python -->

Uma ferramenta para visualizar e analisar seu progresso em treinos de musculação, utilizando dados exportados do popular aplicativo Hevy. Este projeto transforma seus dados brutos em gráficos interativos, permitindo uma compreensão clara da sua evolução ao longo do tempo.

<!-- Opcional: Adicione um screenshot ou GIF do resultado final aqui -->
<!-- ![Screenshot da Aplicação](link_para_seu_screenshot.png) -->

## ✨ Sobre o Projeto

Muitos de nós utilizamos aplicativos como o Hevy para registrar nossos treinos, mas nem sempre é fácil visualizar o progresso de forma consolidada e interativa diretamente no app. Este projeto nasceu da necessidade de ter uma visão mais analítica e personalizável sobre os dados de treino, focando na progressão de carga e repetições em exercícios específicos dentro de diferentes rotinas.

A aplicação gera uma página web local e interativa onde você pode:
*   Selecionar uma rotina de treino específica.
*   Escolher um exercício dentro dessa rotina.
*   Visualizar o progresso para diferentes períodos (últimos 30, 60 ou 90 dias).
*   Filtrar por tipo de série (Top Set/Falha, Séries de Trabalho específicas, ou Todas as Séries).

## 🚀 Funcionalidades

*   **Carregamento de Dados:** Importa e processa arquivos CSV exportados do Hevy.
*   **Processamento Inteligente:** Limpa os dados, converte datas e identifica séries de trabalho.
*   **Visualização Dinâmica:** Gera gráficos de linha interativos (Peso vs. Data) com Plotly, mostrando repetições nos pontos de dados.
*   **Interface Intuitiva:** Página HTML com seletores para filtrar os dados e atualizar os gráficos automaticamente.
*   **Design Responsivo:** A interface se adapta a diferentes tamanhos de tela para uma boa experiência em desktops e dispositivos móveis.
*   **Tudo Local:** O processamento e a visualização ocorrem inteiramente no seu computador, sem necessidade de enviar seus dados para servidores externos.

## 🛠️ Tecnologias Utilizadas

*   **Python 3:** Linguagem de programação principal.
    *   **Pandas:** Para manipulação e análise eficiente dos dados.
    *   **Plotly:** Para a criação dos gráficos interativos.
*   **HTML5:** Para a estrutura da página web.
*   **CSS3:** Para estilização e design responsivo da interface.
*   **JavaScript (Vanilla):** Para a interatividade da página, manipulação do DOM e comunicação com os dados dos gráficos Plotly.
*   **Jupyter Notebook:** Utilizado para o desenvolvimento, exploração de dados e documentação do processo (o arquivo `.ipynb` no repositório).

## 📋 Pré-requisitos

Antes de começar, você precisará ter o Python instalado em seu sistema. Recomenda-se Python 3.8 ou superior. Você também precisará das seguintes bibliotecas Python:

*   pandas
*   plotly
*   numpy (geralmente uma dependência do pandas)

Você pode instalá-las usando pip:
```bash
pip install pandas plotly numpy
