# DeepLearning_CNNs_DataSet-Mnist

## Introdução

Este repositório contém um notebook extensivo que aborda de forma minuciosa o processo de **criação, treinamento e avaliação** de um modelo de rede neural convolucional (CNN) utilizando o conjunto de dados **MNIST**. **Todas as explicações, detalhes e resumos mais completos sobre o código e suas etapas, estão incluídas no notebook**, escritas de forma clara e estruturada após cada célula de código correspondente. Abaixo, você encontrará apenas uma visão geral das principais etapas, apresentada de maneira resumida:

##  Imports
Os pacotes e bibliotecas necessários são importados, incluindo TensorFlow/Keras, NumPy, Pandas e Matplotlib.

## 0. Carregar e Preprocessar o Conjunto de Dados MNIST
O conjunto de dados Fashion MNIST é carregado e preprocessado, preparando as imagens e rótulos para serem usados no treinamento e avaliação do modelo.

## 1. Tratar as Imagens
Nesta etapa, as imagens são preparadas para o treinamento do modelo. Isso inclui o pré-processamento necessário, como a normalização. O objetivo é garantir que as imagens estejam no formato e intervalo corretos para otimizar e melhorar o desempenho do modelo durante o treinamento.

### `1.1 Normalizar as Imagens para o Intervalo [0, 1]:`
Antes de treinar um modelo de rede neural, é comum normalizar as imagens para o intervalo **[0, 1]**. Isso garante que os valores dos pixels estejam dentro de uma faixa padrão, melhorando a eficiência e a convergência do treinamento.

### `1.2 Converter Rótulos para One-hot Encoding:`
Os rótulos são convertidos para uma representação one-hot, o que é necessário para a função de perda `categorical_crossentropy`. 

- **`Observação:`** A etapa de **Converter Rótulos para One-hot Encoding** é **`opcional`** se a função de perda for **sparse_categorical_crossentropy**, que aceita rótulos diretamente como números inteiros.


## 2. Definir a Arquitetura do Modelo
Definição e construção da arquitetura do modelo neural convolucional (CNN). Esta etapa envolve a seleção e configuração das camadas, e a sua organização para otimizar o processamento e análise dos dados. O objetivo é criar uma estrutura eficaz que permita ao modelo extrair características relevantes e realizar a tarefa desejada com precisão.

### `2.1 Exibir Resumo da Arquitetura`
O resumo da arquitetura do modelo é exibido para verificar a estrutura da rede.

## 3. Compilar o Modelo
O modelo é compilado definindo a função de perda, o otimizador e as métricas a serem monitoradas durante o treinamento. Isso configura o modelo para o processo de ajuste dos parâmetros durante o treinamento.

## 4. Treinar o Modelo
O modelo é treinado com os dados processados, ajustando seus parâmetros ao longo de várias épocas para minimizar a função de perda. Após o treinamento, o desempenho é avaliado com o conjunto de validação e o modelo é testado com o conjunto de teste para verificar sua capacidade de generalização.

### `5.1 Resumo da Arquitetura após Compilar e Treinar`
O resumo da arquitetura do modelo é exibido usando o método **`summary()`**. Esse método mostra a lista de camadas, a forma dos dados em cada camada, e o número total de parâmetros treináveis e não treináveis, permitindo verificar a estrutura e a configuração do modelo.

### `5.2 Plotar Gráficos para Avaliar a Evolução do Treinamento`
Nesta etapa, gráficos são gerados para visualizar a evolução do treinamento, incluindo curvas de perda e precisão. Esses gráficos ajudam a monitorar o progresso do modelo, identificando possíveis problemas como overfitting ou underfitting e facilitando ajustes no processo de treinamento.

## 6. Fazer Predições com o Modelo Treinado para Calcular as Métricas
O modelo treinado é aplicado para fazer previsões no conjunto de teste. A partir dessas previsões, são obtidos os resultados necessários para calcular as métricas de desempenho do modelo.

### `6.1 Calcular as Principais Métricas de Avaliação`
São calculadas as métricas **Acurácia, Precisão, Recall e F1-Score** para avaliar o desempenho do modelo.

## 7. Salvar o Modelo em um Arquivo ".keras"
O modelo treinado é salvo em um arquivo ***`.keras`*** para reutilização futura.

## Conclusão

Este resumo fornece uma visão geral das etapas presentes no notebook. O foco principal é a criação e o treinamento de um modelo CNN para a classificação do conjunto de dados MNIST, abordando preprocessamento, avaliação de desempenho e salvamento do modelo. 

***Para explicações detalhadas e um entendimento mais aprofundado sobre CNNs, consulte o código no notebook, onde todas as informações são apresentadas de forma clara e completa.***

## Autor

**Lucas Benício Gusmão da Silva**

Idealizador, criador e desenvolvedor deste projeto.

``Todos os Direitos Reservados``
