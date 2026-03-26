# MODELO PREDITIVO PARA CLASSIFICAÇÃO DE AVALIAÇÕES DE CLIENTES DA AMAZON

## Descrição do Projeto
Este projeto foi desenvolvido como parte da disciplina de Projeto Aplicado II, do curso de Tecnologia em Ciência de Dados da Universidade Presbiteriana Mackenzie.
O objetivo principal do estudo é desenvolver um modelo preditivo capaz de classificar automaticamente avaliações de clientes da Amazon como positivas ou negativas, com base no texto escrito pelos usuários.
O projeto está inserido no contexto de análise de sentimentos (NLP), sendo aplicado ao segmento de produtos alimentícios da Amazon (Amazon Fine Foods). A proposta busca entender padrões linguísticos nas avaliações e automatizar uma tarefa que, manualmente, seria inviável devido ao grande volume de dados.
##
## Problema Preditivo 
O problema do projeto consiste em:
Classificar avaliações de produtos como positivas ou negativas com base no texto.
Critérios adotados:
- Score ≥ 4 → Positivo (1)
- Score ≤ 2 → Negativo (0)
- Score = 3 → Removido da análise
##
## Metodologia
A solução será baseada em técnicas de Machine Learning supervisionado, com foco em classificação binária utilizando regressão logística.
O projeto segue as seguintes etapas:

- Análise exploratória dos dados (EDA)
- Tratamento e limpeza dos dados
- Pré-processamento textual
- Vetorização com TF-IDF
- Treinamento do modelo
- Avaliação com métricas
  
Essas etapas estão alinhadas com os requisitos da Etapa 2 do projeto, que incluem análise, tratamento e definição do método analítico.
##
## Estrutura dos Dados
Principais colunas utilizadas:
- Text → texto da avaliação (feature principal)
- Summary → resumo da avaliação
- Score → variável alvo (binarizada)

Outras colunas foram utilizadas apenas como apoio ou descartadas durante o tratamento.
##
## Análise Exploratória
Foram realizadas análises como:
- Distribuição das notas (scores)
- Separação entre avaliações positivas e negativas
- Frequência de palavras
- Tamanho dos textos
  
Essa etapa permite compreender padrões nos dados antes da modelagem.
##
## Tratamento dos Dados
O tratamento inclui:
- Remoção de avaliações neutras
- Limpeza do texto (pontuação, HTML, caracteres especiais)
- Conversão para minúsculo
- Remoção de stopwords
- Tokenização
- Vetorização com TF-IDF
##
## Modelo
Modelo utilizado:
- Regressão Logística
Divisão dos dados:
80% treino
20% teste
##
## Métricas de Avaliação
O desempenho do modelo será avaliado com:
- Acurácia
- Precisão
- Recall
- F1-score
- Matriz de confusão
  
Essas métricas seguem os critérios definidos na disciplina.
##
## Objetivo do Projeto
Desenvolver um modelo capaz de:
- Classificar automaticamente avaliações de clientes
- Atingir acurácia ≥ 80%
- Gerar insights sobre padrões de linguagem em avaliações
#
## Integrantes do grupo:
- @Allana691
- @Erikabenesi
- @nicolemoreira082-ponto
- @Tawanynsantos
