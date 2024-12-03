# Human Activity Recognition with Smartphones

## Objetivo do Projeto

O objetivo deste projeto é aplicar técnicas de aprendizado de máquina, especificamente o algoritmo K-means, para realizar o reconhecimento de atividades humanas a partir de dados coletados por sensores de smartphones. Usando o dataset "Human Activity Recognition Using Smartphones", que contém dados de acelerômetro e giroscópio, o modelo K-means é utilizado para identificar e agrupar as atividades realizadas pelos indivíduos.

## Instruções para Executar o Código

1. **Prepare o ambiente**: Este código pode ser executado diretamente no [Google Colab](https://colab.research.google.com/), que já possui as bibliotecas necessárias pré-instaladas. Basta rodar as células sequencialmente.
   
2. **Carregar os dados**: Comece carregando o dataset no Colab, de fontes como o [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones).
   
3. **Pré-processamento**: Realize o pré-processamento dos dados, incluindo a limpeza, a remoção de valores ausentes e a normalização das variáveis. Utilize técnicas de redução de dimensionalidade (como PCA, correlação ou Random Forest) para diminuir a complexidade dos dados.

4. **Execução do K-means**: Após o pré-processamento, aplique o algoritmo K-means para realizar a clusterização. A escolha do número de clusters (K) pode ser feita usando o método do cotovelo ou o silhouette score.

5. **Avaliação**: Avalie os resultados utilizando métricas como o silhouette score e a inércia. Utilize gráficos de dispersão para visualizar os clusters formados.

6. **Visualizações**: Use PCA para reduzir a dimensionalidade e gerar gráficos que ajudem na interpretação dos clusters e na análise das atividades agrupadas.

## Principais Conclusões e Considerações sobre os Resultados Obtidos

- O número de clusters foi determinado como 3 com base na análise do método do cotovelo e do silhouette score, sendo adequado para separar as atividades em movimento, parado em pé e parado deitado.
  
- A redução de dimensionalidade foi crucial para tornar o processo de clusterização mais eficiente, reduzindo as 561 variáveis originais para 50, com base em técnicas como análise de correlação, PCA e Random Forest.

- A análise qualitativa das atividades ajudou a confirmar que os três clusters formados correspondem a atividades distintas: uma de movimento, uma de estar parado em pé e outra de estar parado deitado.

- A estabilidade dos clusters foi confirmada ao rodar o K-means várias vezes, e as 5 execuções apresentaram resultados consistentes.

## Tecnologias e Bibliotecas Utilizadas

- **Python**: Linguagem de programação principal.
- **Scikit-learn**: Bibliotecas para K-means, PCA, e métricas de avaliação.
- **Matplotlib e Seaborn**: Bibliotecas para visualização gráfica.
- **Pandas e NumPy**: Para manipulação de dados e operações matemáticas.
- **Google Colab**: Ambiente de execução.

## Como Contribuir

Sinta-se à vontade para sugerir melhorias ou corrigir problemas. Para contribuir, basta fazer um fork deste repositório e enviar um pull request com suas alterações.
