# FIAP - Faculdade de Informática e Administração Paulista

<p align="center">
<a href= "https://www.fiap.com.br/"><img src="assets/logo-fiap.png" alt="FIAP - Faculdade de Informática e Admnistração Paulista" border="0" width=40% height=40%></a>
</p>

<br>

# FarmTech na era da cloud computing
## Nome do grupo

## 👨‍🎓 Integrantes: 
- Felipe Livino dos Santos (RM 563187)
- Daniel Veiga Rodrigues de Faria (RM 561410)
- Tomas Haru Sakugawa Becker (RM 564147)
- Daniel Tavares de Lima Freitas (RM 562625)
- Gabriel Konno Carrozza (RM 564468)


## 👩‍🏫 Professores:
### Tutor(a) 
- <a href="https://www.linkedin.com/company/inova-fusca">Nome do Tutor</a>
### Coordenador(a)
- <a href="https://www.linkedin.com/company/inova-fusca">Nome do Coordenador</a>


## 📜 Descrição

*Este repositório contém o código e os artefatos desenvolvidos na Fase 5 do projeto acadêmico FarmTech Solutions, cujo objetivo é aplicar técnicas de Machine Learning para prever o rendimento de safras agrícolas a partir de variáveis climáticas e de solo. A base de dados utilizada, disponível no arquivo crop_yield.csv, inclui informações como cultura, precipitação, umidade específica, umidade relativa, temperatura a 2 metros e o rendimento em toneladas por hectare.

A solução proposta envolve inicialmente uma análise exploratória dos dados, seguida pela aplicação de métodos de aprendizado não supervisionado, como clusterização, para identificar tendências de produtividade entre culturas e possíveis cenários discrepantes (outliers). Em paralelo, foram desenvolvidos cinco modelos preditivos baseados em algoritmos de regressão supervisionada distintos, que permitem estimar o rendimento das safras a partir das condições fornecidas. Os modelos foram avaliados de acordo com métricas adequadas ao problema, possibilitando a comparação de desempenho e a identificação de pontos fortes e limitações da abordagem.

Todo o fluxo de trabalho foi documentado em um notebook Jupyter, que organiza o processo em células de código Python comentadas e células de markdown explicativas, garantindo a reprodutibilidade e clareza da solução. Como complemento, foi produzido um vídeo de demonstração, com até cinco minutos de duração, apresentando a execução prática do notebook e os principais resultados obtidos.*

[Para mais informações sobre o banco de dados que utilizamos no projeto do ir além, visite o site cliclanco aqui.](https://www.kaggle.com/datasets/govindaramsriram/crop-yield-of-a-farm?resource=download)

*Questão 1 – Qual a solução mais barata?
Após configurarmos a calculadora com os requisitos disponibilizados (2 cpus, 1 GIB de memória, até 5 gigabit de rede, 50 GB de armazenamento, máquina Linux e custos on-demand – 100%) e levantarmos os valores para as regiões de São Paulo e Virgínia do Norte, compilamos numa tabela para melhor visualização e comparação as três instâncias disponíveis. 
Conforme observado na tabela, a instância mais barata, independente de compatibilidade, é a t4g.micro na região da Virgínia. Apesar de os valores absolutos serem baixos, proporcionalmente as instâncias localizadas em São Paulo são cerca de 50% mais caras que as da Virgínia. 

Questão 2 – Existindo restrições legais para armazenamento no exterior e uma necessidade de acesso rápido aos dados dos sensores, qual a melhor opção?
Para auxiliar a responder essa pergunta, criamos um diagrama de decisão baseado em 3 variáveis: restrições judiciais, compatibilidade com a arquitetura ARM e custos.
Portanto, existindo a restrição legal e a necessidade de uma região mais próxima para uma menor latência no acesso aos dados, somente as instâncias da região de São Paulo são elegíveis. Sendo o stack compatível com arquitetura ARM, a opção t4g.micro seria a mais barata. Porém, nós optamos pela instância t3a.micro, pois ela apresenta um custo menor que  a t3.micro e uma compatibilidade maior do que a t4g.micro.*


## 📁 Estrutura de pastas

Dentre os arquivos e pastas presentes na raiz do projeto, definem-se:

- <b>assets</b>: aqui estão os arquivos relacionados a elementos não-estruturados deste repositório, como imagens.

- <b>document</b>: aqui estão todos os documentos do projeto que as atividades poderão pedir. Na subpasta "other", adicione documentos complementares e menos importantes.

- <b>src</b>: Todo o código fonte criado para o desenvolvimento do projeto ao longo das 7 fases.

- <b>README.md</b>: arquivo que serve como guia e explicação geral sobre o projeto (o mesmo que você está lendo agora).

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


