# breast-cancer

## Comparação: Random Forest vs Árvore de Decisão

### 1. Matriz de Confusão

A matriz de confusão é uma ferramenta poderosa para visualizar o desempenho do modelo em termos de classificações corretas e incorretas. Ela apresenta uma visão detalhada dos **verdadeiros positivos (TP)**, **falsos positivos (FP)**, **verdadeiros negativos (TN)** e **falsos negativos (FN)**.

- **Árvore de Decisão**:  
  A matriz de confusão da Árvore de Decisão mostrou um número maior de erros em termos de **falsos positivos** e **falsos negativos** em comparação ao modelo Random Forest. Isso indica que a Árvore de Decisão tem uma tendência a classificar incorretamente alguns casos de tumores benignos como malignos e vice-versa.

- **Random Forest**:  
  A matriz de confusão do modelo Random Forest apresentou um desempenho superior, com menos erros de classificação. Houve uma menor quantidade de falsos positivos e falsos negativos, o que significa que o modelo Random Forest conseguiu diferenciar melhor entre os tumores benignos e malignos. Isso pode ser atribuído ao fato de que o Random Forest combina múltiplas árvores de decisão, resultando em uma classificação mais robusta.

### 2. Acurácia

A acurácia é uma métrica que mede a proporção de previsões corretas sobre o total de previsões feitas. Neste exercício:

- **Árvore de Decisão**:  
  O modelo de Árvore de Decisão apresentou uma acurácia menor, devido à sua natureza de ser mais propenso ao **overfitting**. Ele tende a se ajustar aos dados de treino de forma muito específica, o que prejudica sua capacidade de generalizar bem em novos dados de teste. Isso pode levar a erros em classificações de novos exemplos.

- **Random Forest**:  
  O modelo Random Forest apresentou uma **acurácia significativamente maior**. Isso acontece porque o Random Forest é um conjunto de várias árvores de decisão independentes, cada uma com pequenas variações. Ao combinar os resultados de várias árvores (por meio de votação), o modelo corrige os erros das árvores individuais, tornando a previsão mais precisa e menos suscetível ao overfitting.

### 3. Por que o Random Forest foi melhor?

O modelo **Random Forest** geralmente tem um desempenho superior em comparação à Árvore de Decisão por vários motivos:

- **Redução de Variância**:  
  Enquanto uma única árvore de decisão pode ser altamente sensível aos dados de treino e produzir resultados erráticos para diferentes amostras, o Random Forest constrói várias árvores a partir de diferentes subconjuntos dos dados. Esse processo de combinação (bagging) reduz a variância e melhora a robustez das previsões.

- **Generalização Melhor**:  
  Como o Random Forest utiliza o conceito de agregação de múltiplas árvores, ele tem melhor capacidade de generalizar os dados de teste. Ele tende a evitar o problema de **overfitting**, que é comum em árvores de decisão individuais, tornando-o mais eficaz na previsão de novos exemplos.

- **Robustez contra Ruído**:  
  O Random Forest é menos propenso a ser influenciado por ruído nos dados, porque o impacto de uma amostra ruidosa é minimizado quando o resultado é baseado em várias árvores diferentes.

---

### Conclusão

- **Matriz de Confusão**:  
  O Random Forest apresentou menos erros de classificação (falsos positivos e falsos negativos) em comparação à Árvore de Decisão, o que indica uma melhor capacidade de diferenciar entre tumores benignos e malignos.

- **Acurácia**:  
  O modelo Random Forest foi mais preciso, resultando em uma maior acurácia devido à sua abordagem de múltiplas árvores, que corrige os erros de previsões individuais.

Em resumo, o **Random Forest** superou a **Árvore de Decisão** em termos de desempenho, tanto na matriz de confusão quanto na acurácia geral.
