# Projeto de Perceptron

Este projeto implementa um **Perceptron** simples para resolver um problema de **classificação binária**. Ele é capaz de aprender a separar dois grupos de pontos em um plano 2D usando uma linha de decisão, destacando como esse classificador linear funciona e como ele pode ser treinado.

## Objetivo

O objetivo deste projeto é demonstrar o funcionamento de um Perceptron, um dos algoritmos mais básicos de redes neurais, aplicado a um problema de classificação simples. O Perceptron ajusta seus pesos com base nos erros durante o treinamento para classificar corretamente os pontos de entrada em duas classes.

## Estrutura do Projeto

1. **Gerar Dataset**: Pontos em duas classes são gerados aleatoriamente em torno de dois centros (um grupo de pontos vermelhos e outro grupo de pontos azuis).
   
2. **Implementação do Perceptron**: O Perceptron é implementado do zero utilizando a biblioteca `NumPy` para realizar as operações de álgebra linear. A função de ativação utilizada é a **função degrau**.

3. **Treinamento**: O Perceptron é treinado utilizando a regra de aprendizado baseada na diferença entre as previsões e os rótulos reais dos dados de treino. O ajuste dos pesos é realizado iterativamente.

4. **Avaliação**: Após o treinamento, o modelo é avaliado com base na **acurácia** para determinar o quão bem ele classificou os dados de treino.

5. **Visualização**: A fronteira de decisão aprendida pelo Perceptron é visualizada em um gráfico 2D, mostrando como ele separa as duas classes de pontos.

## Arquitetura do Perceptron

O Perceptron tem a seguinte estrutura:

- **Entradas**: Um vetor de entradas \(X = [x_1, x_2, ..., x_n]\).
- **Pesos**: Um vetor de pesos \(W = [w_1, w_2, ..., w_n]\), que é ajustado durante o treinamento.
- **Bias**: Um valor de ajuste adicional, que garante que a fronteira de decisão possa ser deslocada.
- **Função de ativação**: Função degrau que decide se a saída será 0 ou 1.
- **Regra de aprendizado**: A atualização dos pesos é feita com base no erro \(y_{\text{real}} - y_{\text{predito}}\), e a taxa de aprendizado \( \eta \).

## Visualização

O gráfico abaixo mostra a fronteira de decisão aprendida pelo Perceptron após o treinamento:

- Os pontos vermelhos representam a **Classe 1**.
- Os pontos azuis representam a **Classe 0**.
- A linha separadora corresponde à fronteira de decisão calculada pelo Perceptron.

## Conceitos Chave

- **Perceptron**: Um algoritmo de aprendizado supervisionado que ajusta pesos com base nos erros de previsão.
- **Classificação Linear**: O Perceptron separa os dados usando uma linha (ou um hiperplano, em dimensões mais altas) para distinguir entre duas classes.
- **Função de Ativação**: Utiliza-se a função degrau para definir se o neurônio deve ativar (saída 1) ou não (saída 0).
- **Atualização de Pesos**: A regra de atualização dos pesos é iterativa e depende do erro entre a previsão do modelo e o rótulo real.

## Melhoria Futura

- **Perceptron Multicamadas**: Este projeto implementa apenas um Perceptron de camada única, que é capaz de resolver apenas problemas linearmente separáveis. Um próximo passo seria explorar um Perceptron Multicamadas (MLP) com **backpropagation** para lidar com problemas mais complexos.
- **Validação Cruzada**: Adicionar técnicas de validação para garantir que o modelo generalize bem em novos dados.

## Referências

- Rosenblatt, F. (1958). The Perceptron: A Probabilistic Model for Information Storage and Organization in the Brain.
- Bishop, C. M. (1995). Neural Networks for Pattern Recognition.

---

Este projeto é uma introdução ao Perceptron e pode ser expandido para projetos mais avançados envolvendo redes neurais.
