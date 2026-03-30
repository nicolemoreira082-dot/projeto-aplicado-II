# MODELO PREDITIVO PARA CLASSIFICAÇÃO DE AVALIAÇÕES DE CLIENTES DA AMAZON

## Descrição do Projeto
Este projeto foi desenvolvido como parte da disciplina de Projeto Aplicado II, do curso de tecnologia em Banco de Dados da Universidade Presbiteriana Mackenzie.O objetivo principal é desenvolver um modelo preditivo de *Deep Learning* capaz de classificar automaticamente avaliações de clientes da Amazon como positivas, neutras ou negativas, com base no processamento de linguagem natural (NLP).O estudo utiliza o dataset Amazon Fine Foods para entender padrões linguísticos e automatizar a análise de sentimentos em larga escala.

## Problema Preditivo
O desafio consiste em classificar a polaridade da experiência do usuário com base exclusivamente em seu relato textual.
*Critérios de Classificação (Labels):*
* *Positivo (LABEL_2):* Pontuação 4 ou 5.
* *Neutro (LABEL_1):* Pontuação 3.
* *Negativo (LABEL_0):* Pontuação 1 ou 2.

## Metodologia
A solução utiliza técnicas avançadas de *Aprendizado Profundo (Deep Learning)* através da arquitetura *Transformers*. O fluxo de trabalho compreende:
1.  [cite_start]Análise Exploratória de Dados (EDA) e visualização temporal.
2.  [cite_start]Tratamento e limpeza de dados (preservando a integridade do texto).
3.  [cite_start]Tokenização e codificação para modelos de linguagem.
4.  [cite_start]Implementação do modelo *RoBERTa* (via Hugging Face)
5.  Avaliação de desempenho multiclasse.



## Estrutura dos Dados
* *Text:* Conteúdo integral da avaliação (Feature Principal).
* *Summary:* Resumo da avaliação (Feature Secundária).
* *Score:* Variável alvo para treinamento e validação.

## Análise Exploratória (EDA)
Foram realizadas análises para identificar:
* Distribuição volumétrica das notas de 1 a 5.
* Proporção de sentimentos (Positivo, Neutro e Negativo).
* Evolução da média de avaliações por ano.
* Padrões de comprimento de texto e nuvem de palavras mais frequentes.

## Modelo: RoBERTa
Diferente de modelos estatísticos simples, o *RoBERTa* (Robustly Optimized BERT Approach) utiliza mecanismos de atenção para compreender o contexto completo das frases, incluindo negações e intensificadores.
* *Processamento:* Manutenção de stop words para garantir a precisão semântica.
* *Divisão de dados:* 80% treino / 20% teste.

## Métricas de Avaliação
O desempenho é mensurado através de:
* Acurácia (Meta >= 80%).
* Precisão (Precision).
* Sensibilidade (Recall).
* F1-Score e Matriz de Confusão.
- @nicolemoreira082-ponto
- @Tawanynsantos
