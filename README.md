# Transfer Learning com VGG16 para Classificação de Gatos e Cachorros 🐱🐶

Este projeto demonstra como aplicar Transfer Learning utilizando a rede VGG16 pré-treinada para classificar imagens de gatos e cachorros. O projeto é implementado em Python utilizando TensorFlow e Keras, e é executado no ambiente Google Colab com GPU T4.

## Visão Geral
Transfer Learning é uma técnica poderosa onde um modelo pré-treinado em um grande dataset é adaptado para uma nova tarefa com um novo dataset. Neste projeto, usamos a rede VGG16, previamente treinada no ImageNet, e adaptamos para classificar imagens do dataset Cats vs Dogs.

## Estrutura do Projeto
download_dataset.py: Script para baixar e extrair o dataset Cats vs Dogs.
train_model.py: Script para criar, treinar e avaliar o modelo de Transfer Learning.
visualize_results.py: Script para visualizar os resultados do treinamento.
Pré-requisitos
Python 3.x
TensorFlow 2.x
Keras
Matplotlib
Ambiente Google Colab com GPU T4

## Instruções de Execução
1. Configuração do Ambiente
Execute o projeto no Google Colab e certifique-se de que a GPU está ativada:

Acesse Runtime > Change runtime type.
Selecione GPU na opção de Hardware accelerator.
Instale as dependências necessárias utilizando o pip install tensorflow matplotlib.

2. Baixar e Extrair o Dataset
Baixe o dataset Cats vs Dogs do !URL https://storage.googleapis.com/mledu-datasets/cats_and_dogs_filtered.zip e extraia os arquivos para o diretório especificado. Isso pode ser feito utilizando urllib.request e zipfile.

3. Treinar o Modelo
Crie o modelo de Transfer Learning utilizando a arquitetura VGG16 pré-treinada. Congele a base convolucional e adicione novas camadas densas para a classificação. Compile e treine o modelo utilizando os dados de treinamento e validação gerados pelo ImageDataGenerator.

4. Visualizar os Resultados
Após o treinamento, visualize os resultados plotando os gráficos de precisão e perda durante o treinamento e validação. Isso permitirá avaliar o desempenho do modelo.

## Resultados
Os gráficos de precisão e perda durante o treinamento e validação serão gerados, permitindo avaliar o desempenho do modelo.

## Contribuição
Contribuições são bem-vindas! Sinta-se à vontade para abrir uma issue ou enviar um pull request.

## Licença
Este projeto está licenciado sob a Licença MIT - veja o arquivo LICENSE para mais detalhes.
