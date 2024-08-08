# Credit Data Classification

Este projeto utiliza técnicas de aprendizado de máquina para classificar dados de crédito, determinando se um cliente em potencial representa um risco de crédito. O projeto emprega um classificador Random Forest para prever se um cliente pagará seu empréstimo com base em dados de treino pré-processados.

## Overview do Projeto

O conjunto de dados de crédito foi dividido em conjuntos de treinamento e teste, com cada entrada contendo 3 atributos relevantes para a avaliação de risco de crédito. A variável alvo indica se um cliente tem ou não um bom histórico de pagamento.

## Etapas do Projeto

### Importação de Bibliotecas e Carregamento de Dados

- Bibliotecas utilizadas: `pandas`, `numpy`, `matplotlib`, `sklearn`, `pickle`, `yellowbrick`.
- Os dados pré-processados são carregados de um arquivo `pickle` que contém os conjuntos de dados de treinamento e teste.

### Treinamento do Modelo

- **Random Forest Classifier**: O modelo é treinado usando o classificador Random Forest com 40 estimadores e o critério de entropia para dividir os nós.
- O modelo é ajustado utilizando o conjunto de treinamento para identificar padrões nos dados.

### Avaliação do Modelo

- **Accuracy Score**: Avaliação do desempenho do modelo em termos de precisão no conjunto de teste, com um resultado de 98,4%.
- **Confusion Matrix**: Uso do `yellowbrick` para visualizar a matriz de confusão e entender as previsões verdadeiras e falsas.
- **Classification Report**: Relatório detalhado que fornece métricas de precisão, recall e f1-score para cada classe.

## Pré-processamento de Dados

O pré-processamento dos dados foi realizado em um notebook separado chamado `BaseCredito_DataPrep`, disponível no repositório do GitHub. Este passo é crucial para transformar os dados brutos em um formato adequado para treinamento de modelos de machine learning.

## Conclusão

Este projeto demonstra a eficácia de um classificador Random Forest na avaliação de risco de crédito. A alta precisão alcançada reflete a capacidade do modelo de prever corretamente o risco de crédito, o que pode ser útil para instituições financeiras na tomada de decisões informadas sobre empréstimos.

## Requisitos

- Python 3.x
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
- Yellowbrick

## Execução do Projeto

1. Certifique-se de que todos os requisitos estão instalados.
2. Execute o notebook de pré-processamento `BaseCredito_DataPrep` para preparar os dados.
3. Carregue os dados pré-processados e treine o modelo utilizando o script principal.
4. Avalie o desempenho do modelo com o conjunto de teste e visualize os resultados.

## Referências

- [Scikit-learn Documentation](https://scikit-learn.org/stable/documentation.html)
- [Yellowbrick Documentation](https://www.scikit-yb.org/en/latest/)
