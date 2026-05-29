# AASE-Aprendizagem-Automatica-em-Sistemas-Empresariais

Este repositório contém um projeto académico desenvolvido no âmbito da unidade curricular de Aprendizagem Automática em Sistemas Empresariais.

O projeto tem como objetivo desenvolver modelos de Machine Learning capazes de estimar a gama de preço de telemóveis com base nas suas características técnicas, tais como bateria, memória interna, RAM, resolução do ecrã, peso, número de núcleos do processador, conectividade e outras variáveis relevantes.

## Objetivo do projeto

O principal objetivo de negócio consiste em permitir a estimativa da gama de preço de um telemóvel com base nas suas características, apoiando a tomada de decisão na definição de preços.

O objetivo de Data Mining consiste em desenvolver modelos preditivos capazes de classificar os telemóveis em diferentes categorias de preço, utilizando técnicas de aprendizagem automática.

## Metodologia

O projeto segue a metodologia CRISP-DM, contemplando as seguintes fases:

- Business Understanding;
- Data Understanding;
- Data Preparation;
- Modeling;
- Evaluation.

## Dataset

O dataset utilizado contém características técnicas de telemóveis e a respetiva gama de preço.

Entre os atributos analisados encontram-se:

- `battery_power` — capacidade da bateria;
- `clock_speed` — velocidade do processador;
- `dual_sim` — suporte para dois cartões SIM;
- `fc` — megapíxeis da câmara frontal;
- `four_g` — compatibilidade com rede 4G;
- `int_memory` — memória interna;
- `mobile_wt` — peso do telemóvel;
- `n_cores` — número de núcleos do processador;
- `px_height` — resolução vertical do ecrã;
- `px_width` — resolução horizontal do ecrã;
- `ram` — memória RAM;
- `touch_screen` — existência de ecrã tátil;
- `wifi` — compatibilidade com Wi-Fi;
- `price_range` — gama de preço.

## Técnicas de Machine Learning

Foram testadas várias técnicas de modelação, nomeadamente:

- Decision Tree;
- Random Forest;
- Naive Bayes;
- Redes Neuronais;
- Support Vector Machine.

Os modelos foram desenvolvidos e avaliados com recurso ao RapidMiner.

## Cenários analisados

Foram criados quatro cenários de análise:

- Cenário 1 — todas as variáveis com outliers;
- Cenário 2 — variáveis com maior correlação com a variável target;
- Cenário 3 — todas as variáveis sem outliers;
- Cenário 4 — variáveis mais relevantes e sem outliers.

## Resultados

Após a avaliação dos modelos, as Redes Neuronais apresentaram o melhor desempenho global, especialmente no cenário 4.

O cenário 4 obteve os melhores resultados nas métricas avaliadas, com destaque para o F1-score, demonstrando uma elevada capacidade de classificação da gama de preço dos telemóveis.

## Visualização

Foi também criada uma dashboard em Tableau para apoiar a análise e visualização dos dados relacionados com a estimativa da gama de preço dos telemóveis.

## Estrutura do repositório

```text
.
├── dashboard-estimativa-preco-telemoveis.twb
├── final2_final.csv
├── decision-tree.rmp
├── naive-bayes.rmp
├── redes-neuronais.rmp
├── random-forest.rmp
├── svm.rmp
├── relatorio.pdf
└── README.md

Ferramentas utilizadas
RapidMiner;
Tableau;
Python;
Jupyter Notebook;
Talend;
Microsoft Excel.
Como consultar o projeto

Para consultar o projeto:

Abrir o relatório relatorio.pdf;
Abrir os ficheiros .rmp no RapidMiner para visualizar os modelos;
Abrir o ficheiro .twb no Tableau para visualizar a dashboard (é possível que seja necessario alterar os atributos de tempo para Data);
Consultar o dataset no ficheiro final2_final.csv.

Autoria
Projeto académico desenvolvido no âmbito da unidade curricular de Aprendizagem Automática em Sistemas Empresariais.
