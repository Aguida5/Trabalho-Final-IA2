# Trabalho-Final-IA2

Este trabalho visa o uso de CNN (Convolucional Neural Network) para identificação de imagens diversas classificadas e rotuladas de pintas de pele que serão avaliadas pela rede sendo câncer benigno ou câncer maligno. Foi usado Data Set de imagens do endereço: https://www.isic-archive.com e salvo em um diretório local.

Foi construido um modelo que usa imagens de pintas de pele como entrada e produz a probabilidade prevista para cada uma das categorias (nesse caso, ela terá 5 saídas).

No código foram usados várias funções,  como por exemplo:

ReLU - Unidade Linear Retificada

Função de ativação cuja principal vantagem sobre outras funções de ativação é que esta função não ativa todos os neurónios da rede ao mesmo tempo. Caso uma entrada da rede seja negativa, essa entrada é convertida em 0 e o neurônio não é ativado.

Foram importados todos os pacotes necessários e, também usada a biblioteca FastAI V1 que fornece várias funções que permitem a construção de uma rede neural fácil e eficiente. A biblioteca FastAI V1 fica no topo Pytorch 1.0. Nesse quesito pode-se utilizar como alternativa o Tensorflow. 

O caderno inicia com os seguintes comandos:

%reload_ext autoreload
%autoreload 2
%matplotlib inline

Que garantem que quaisquer edições nas bibliotecas que forem feitas sejam recarregadas automaticamente, e também que quaisquer gráficos ou imagens exibidas sejam mostrados neste caderno.

Foi rodada Resnet34 que é uma rede residual de 34 camadas e posteriormente foi rodada a rede resnet50 com 50 camadas.
O resnet50 geralmente funciona melhor porque é uma rede mais profunda com mais parâmetros. 
O objetivo foi conseguir um melhor desempenho da rede. 
Os dados foram normalizados e foi medida a acurácia do modelo intermediária e final do modelo. Chegando a uma acurácia de 90%.

