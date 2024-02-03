# Machine Learning no Azure ML Studio

## Laboratório realizado no MS Azure sobre criação e treinamento de modelos de IA

Link oficial disponível [aqui]('https://microsoftlearning.github.io/mslearn-ai-fundamentals/Instructions/Labs/01-machine-learning.html')

Os passos para se chegar ao uso de um modelo treinado no Azure Machine Learning Studio (supondo que voce já tenha uma conta na plataforma MS Azure):

1. No portal MS Azure voce precisa criar uma nova maquina virtual utilizando uma imagem de Machine Learning já provida pela própria Microsoft.

![Machine Learning image](/assets/azure_ml.png)

> Os demais passos a partir de agora são realizados no portal Azure Machine Learning Studio com a mesma conta utilizada no passo anterior [Azure ML Studio]('https://ml.azure.com')
2. Utilize o Machine Learning Automatizado para treinar um modelo baseado em um ddataset já previsto na documentação.

3. O método utilizado será o de regressão pois queremos um resultado mais direcionado a uma informação, usando-se para isso o aprendizado supervisionado.

4. O ML Studio irá utilizar alguns algoritmos de aprendizado para definir os que apresentam melhores resultados entre as informações de treino e teste.

> As métricas de treinamento do modelo, como a assertividade, dopode ser conferida também no ML Studio:
![Model metrics](/assets/metrics.png)


5. Uma vez definido o melhor algoritmo voce pode publicar como serviço e criar o eendpoint que será responsavel por receber os dados de entrada para que o modelo faça a predição pretendida.

6. Neste caso o modelo foi utilizado para se fazer previsão de aluguel de bicicletas baseados em dados históricos. Quando inserimos dados futuros o modelo responde algo neste formato, podendo então ser tratado em qualquer integração necessária.
![Model result](/assets/ml_result.png)


