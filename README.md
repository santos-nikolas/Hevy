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
```
Se você planeja executar ou modificar o Jupyter Notebook (`.ipynb`), precisará também do Jupyter:
```bash
pip install notebook
```

## ⚙️ Como Usar

1.  **Exporte seus Dados do Hevy:**
    *   No aplicativo Hevy, vá para as configurações e procure a opção de exportar seus dados. Geralmente, isso gera um arquivo `workouts.csv`.
    *   Coloque este arquivo `workouts.csv` na mesma pasta onde você clonou ou baixou este projeto.

2.  **Execute o Notebook Python:**
    *   Clone este repositório:
        ```bash
        git clone https://github.com/santos-nikolas/Hevy.git
        cd Hevy
        ```
    *   Abra o arquivo Jupyter Notebook (`Hevy.ipynb`).
    *   Execute todas as células do notebook em ordem. A última célula irá gerar um arquivo HTML (`visualizacao_treino_profissional.html`).

3.  **Abra o Arquivo HTML:**
    *   Após a execução bem-sucedida do notebook, localize o arquivo HTML gerado na pasta do projeto.
    *   Abra este arquivo em seu navegador web preferido (Chrome, Firefox, Edge, etc.).

4.  **Interaja com a Visualização:**
    *   Use os menus suspensos para selecionar a rotina de treino, o exercício, o período de análise e o tipo de série que deseja visualizar.
    *   O gráfico será atualizado automaticamente para refletir suas seleções.

## 📈 Exemplo de Visualização

![image](https://github.com/user-attachments/assets/ec8b0e05-8a27-48a0-b96e-36e07df176ff)

O gráfico principal exibe a progressão do peso (em kg) no eixo Y ao longo do tempo (data no eixo X). Cada ponto no gráfico representa uma série realizada, com o número de repetições exibido acima do ponto. Isso permite identificar rapidamente tendências de aumento de carga, estagnação ou variações no número de repetições.

## 💡 Possíveis Melhorias e Contribuições

Este projeto é uma base sólida e há muitas maneiras de expandi-lo! Algumas ideias incluem:
*   Adicionar mais tipos de gráficos (ex: volume total, 1RM estimado).
*   Permitir a comparação de múltiplos exercícios no mesmo gráfico.
*   Implementar um backend (ex: Flask/Django) para carregar dados dinamicamente, em vez de embutir tudo no HTML/JS, especialmente útil para grandes volumes de dados ou atualizações frequentes.
*   Adicionar filtros por notas de exercício ou RPE (se disponíveis nos dados).
*   Melhorar ainda mais a interface do usuário com recursos de personalização.

Contribuições são bem-vindas! Sinta-se à vontade para abrir *issues* para sugestões ou *pull requests* com melhorias.

## 📄 Licença

Este projeto está licenciado sob a Licença MIT - veja o arquivo `LICENSE`para mais detalhes.

## 🙏 Agradecimentos

*   Ao time do [Hevy](https://www.hevy.com/) por criar um ótimo aplicativo de rastreamento de treinos e permitir a exportação de dados.
*   Às comunidades por trás do Python, Pandas e Plotly.

---
Feito com 💪 por santos-nikolas(https://github.com/santos-nikolas)
