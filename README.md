# FIAP - Faculdade de Informática e Administração Paulista

<p align="center">
<a href= "https://www.fiap.com.br/"><img src="assets/logo-fiap.png" alt="FIAP - Faculdade de Informática e Admnistração Paulista" border="0" width=40% height=40%></a>
</p>

<br>

# FarmTech na era da cloud computing

## Nome do grupo

Rumo ao NEXT!

## 👨‍🎓 Integrantes:

- Felipe Livino dos Santos (RM 563187)
- Daniel Veiga Rodrigues de Faria (RM 561410)
- Tomas Haru Sakugawa Becker (RM 564147)
- Daniel Tavares de Lima Freitas (RM 562625)
- Gabriel Konno Carrozza (RM 564468)

## 👩‍🏫 Professores:

### Tutor(a)

- Leonardo Ruiz Orabona

### Coordenador(a)

- ANDRÉ GODOI CHIOVATO

## 📜 Descrição

*Este repositório contém o código e os artefatos desenvolvidos na Fase 5 do projeto acadêmico FarmTech Solutions, cujo objetivo é aplicar técnicas de Machine Learning para prever o rendimento de safras agrícolas a partir de variáveis climáticas e de solo. A base de dados utilizada, disponível no arquivo crop_yield.csv, inclui informações como cultura, precipitação, umidade específica, umidade relativa, temperatura a 2 metros e o rendimento em toneladas por hectare.

A solução proposta envolve inicialmente uma análise exploratória dos dados, seguida pela aplicação de métodos de aprendizado não supervisionado, como clusterização, para identificar tendências de produtividade entre culturas e possíveis cenários discrepantes (outliers). Em paralelo, foram desenvolvidos cinco modelos preditivos baseados em algoritmos de regressão supervisionada distintos, que permitem estimar o rendimento das safras a partir das condições fornecidas. Os modelos foram avaliados de acordo com métricas adequadas ao problema, possibilitando a comparação de desempenho e a identificação de pontos fortes e limitações da abordagem.

Todo o fluxo de trabalho foi documentado em um notebook Jupyter, que organiza o processo em células de código Python comentadas e células de markdown explicativas, garantindo a reprodutibilidade e clareza da solução. Como complemento, foi produzido um vídeo de demonstração, com até cinco minutos de duração, apresentando a execução prática do notebook e os principais resultados obtidos.*

Análise e Modelagem de Dados (Notebook Jupyter)

Este repositório apresenta uma solução de **análise exploratória** e **modelagem preditiva** aplicada a dados com variáveis como temperatura, umidade, precipitação e cultura (crop), visando compreender padrões e **estimar o rendimento (yield)**. 
O propósito deste README é oferecer uma visão introdutória da solução e **conduzir você diretamente ao Jupyter Notebook**, onde está todo o passo a passo executável e a descrição completa.

> 🔎 **Onde está o passo a passo?**  
> Todo o fluxo detalhado — da exploração de dados ao treinamento e à avaliação — está no arquivo **`_pbl_fase4.ipynb`**. Abra-o e execute as células na sequência indicada.

---

## 🎯 Objetivos
- Organizar e explorar o conjunto de dados (EDA).
- Preparar os dados para modelagem (limpeza, normalização/escala, divisão em treino e teste).
- Investigar estrutura de grupos/segmentos (clusterização) quando relevante.
- Treinar e comparar múltiplos modelos de regressão.
- Avaliar desempenho com métricas adequadas (ex.: **MAE** e **R²**).
- Selecionar o melhor modelo e registrar aprendizados/insights.

---

## 🧭 Visão Geral do Fluxo (alto nível)
1. **Ingestão e inspeção** do dataset (tipos, valores ausentes, estatísticas descritivas).
2. **EDA**: análise de distribuição, correlação e possíveis outliers.
3. **Pré-processamento**: seleção de features, normalização (quando necessário) e **train/test split**.
4. **Clusterização (K-Means)**: investigação exploratória de grupos (opcional/explicativo).
5. **Modelagem**: 
   - Regressão Linear  
   - Árvore de Decisão  
   - **Random Forest** *(modelo campeão no notebook)*  
   - SVR  
   - Gradient Boosting
6. **Avaliação**: comparação de métricas e escolha do modelo.
7. **Conclusões**: interpretação e próximos passos.

> 💡 Observação: os detalhes, gráficos e justificativas de cada etapa estão no notebook.

---

## 🧩 Tecnologias e Bibliotecas
- **Python 3.10+**
- **Jupyter Notebook / JupyterLab**
- **pandas**, **scikit-learn**, **matplotlib**, **seaborn**

Sugestão de `requirements.txt` minimalista:
```
pandas
scikit-learn
matplotlib
seaborn
jupyter
```
(Ajuste versões conforme seu ambiente.)

---

[Para mais informações sobre o banco de dados que utilizamos no projeto do ir além, visite o site cliclanco aqui.](https://www.kaggle.com/datasets/govindaramsriram/crop-yield-of-a-farm?resource=download)

*Questão 1 – Qual a solução mais barata?
Após configurarmos a calculadora com os requisitos disponibilizados (2 cpus, 1 GIB de memória, até 5 gigabit de rede, 50 GB de armazenamento, máquina Linux e custos on-demand – 100%) e levantarmos os valores para as regiões de São Paulo e Virgínia do Norte, compilamos numa tabela para melhor visualização e comparação as três instâncias disponíveis. 
Conforme observado na tabela, a instância mais barata, independente de compatibilidade, é a t4g.micro na região da Virgínia. Apesar de os valores absolutos serem baixos, proporcionalmente as instâncias localizadas em São Paulo são cerca de 50% mais caras que as da Virgínia. 

Questão 2 – Existindo restrições legais para armazenamento no exterior e uma necessidade de acesso rápido aos dados dos sensores, qual a melhor opção?
Para auxiliar a responder essa pergunta, criamos um diagrama de decisão baseado em 3 variáveis: restrições judiciais, compatibilidade com a arquitetura ARM e custos.
Portanto, existindo a restrição legal e a necessidade de uma região mais próxima para uma menor latência no acesso aos dados, somente as instâncias da região de São Paulo são elegíveis. Sendo o stack compatível com arquitetura ARM, a opção t4g.micro seria a mais barata. Porém, nós optamos pela instância t3a.micro, pois ela apresenta um custo menor que  a t3.micro e uma compatibilidade maior do que a t4g.micro.*


## 📁 Estrutura de pastas
```
challenge-fase5-FIAP/  
├── assets/                          # Imagens, diagramas e outros arquivos visuais
│  
├── calculadora_AWS/                 # Arquivos de dados utilizados no projeto
│   ├── tabela_de_precos_aws.webp    # Imagem da tabela de preços relacionada aas calculadoras da AWS
│   └── diagrama_de_decisao_aws.webp # Imagem do diagrama de decisão na análise da calculadora AWS
│
├── data/                            # Arquivos de dados utilizados no projeto
│   └── crop_yield.csv               # Dataset usado para treino do modelo
│
├── ir_alem/                         # Arquivos do projeto IR ALÉM
│   ├── data/                        # Arquivos de dados utilizados no projeto
│       └── crop_yield_data.csv      # Dataset usado para treino do modelo      
│   ├── notebooks/                   # Notebook com análise e machine learning  
│       └── main-ir-alem.ipynb       # Implementação e treino do modelo de ML "IR ALÉM"
│   ├── wokwi/                       # Arquivos do simulador Wokwi (ESP32)
│       └── diagram.json             # Diagrama do circuito
│       └── libraries.txt            # Bibliotecas necessárias
│       └── sketch.ino               # Código da simulação (Arduino)
│       └── wokwi-project.txt        # Configuração do projeto Wokwi
│   └── requirements.txt             # Imagem exportada do Diagrama ER
│
├── notebooks/                       # Notebook com análise e machine learning
│   └── pbl_fase4.ipynb              # Implementação e treino do modelo de ML entrega 1
│
├── README.md                        # Documentação do projeto
```
## 🔧 Como executar o código

*Acrescentar as informações necessárias sobre pré-requisitos (IDEs, serviços, bibliotecas etc.) e instalação básica do projeto, descrevendo eventuais versões utilizadas. Colocar um passo a passo de como o leitor pode baixar o seu código e executá-lo a partir de sua máquina ou seu repositório. Considere a explicação organizada em fase.*


## 🗃 Histórico de lançamentos

* 0.5.0 - XX/XX/2024
    * 
* 0.4.0 - XX/XX/2024
    * 
* 0.3.0 - XX/XX/2024
    * 
* 0.2.0 - XX/XX/2024
    * 
* 0.1.0 - XX/XX/2024
    *

## 📋 Licença

<img style="height:22px!important;margin-left:3px;vertical-align:text-bottom;" src="https://mirrors.creativecommons.org/presskit/icons/cc.svg?ref=chooser-v1"><img style="height:22px!important;margin-left:3px;vertical-align:text-bottom;" src="https://mirrors.creativecommons.org/presskit/icons/by.svg?ref=chooser-v1"><p xmlns:cc="http://creativecommons.org/ns#" xmlns:dct="http://purl.org/dc/terms/"><a property="dct:title" rel="cc:attributionURL" href="https://github.com/agodoi/template">MODELO GIT FIAP</a> por <a rel="cc:attributionURL dct:creator" property="cc:attributionName" href="https://fiap.com.br">Fiap</a> está licenciado sobre <a href="http://creativecommons.org/licenses/by/4.0/?ref=chooser-v1" target="_blank" rel="license noopener noreferrer" style="display:inline-block;">Attribution 4.0 International</a>.</p>


