# Contagem de pessoas utilizando deep learning e imagens aéreas
#### Aluno: [Mateus Furlin Bampi](https://github.com/MateusBampi).
#### Orientador: Manoela Kohler]().

---

Trabalho apresentado ao curso [BI MASTER](https://ica.puc-rio.ai/bi-master) como pré-requisito para conclusão de curso e obtenção de crédito na disciplina "Projetos de Sistemas Inteligentes de Apoio à Decisão".

---

### Resumo

O projeto, desenvolvido em Python, consistiu em criar um modelo de deep learning para a detecção e contagem de pessoas. Para o treinamento, utilizou-se um banco de dados com 2000 frames de um vídeo de uma webcam. As imagens já estavam rotuladas com o número de pessoas dentro da imagem.

A rede neural sequencial utilizou o otimizador Adam e as função de ativação Relu e foi dividida em duas partes: 
  
  1. Uma rede convolucional, com duas camadas convolucionais para extrair informações das imagens, duas camadas de maxpooling como forma de reduzir o tamanho das informações, uma camada de dropout para melhor a performance do modelo e uma camada de flattening para passar as informações para a parte full dense da rede neural;

  2. A rede full dense consistiu em duas camadas, uma com 128 neurônios para aprender o que se passa na imagem, e uma com um neurônio para dar o resultado final.

O treinamento foi bem sucedido e foi capaz de realizar inferências em imagens que nunca havia visto dentro deste mesmo dataset como demonstram as figuras abaixo.

![thumbnail_image (1)](https://user-images.githubusercontent.com/84750991/126877818-6657956e-fbda-4f2a-b713-461a07dd5c73.png)

![thumbnail_image](https://user-images.githubusercontent.com/84750991/126877782-326ee0d8-6180-4786-94d5-18278ded8aaf.png)

Em seguida, realizamos inferências em imagens capturadas por drones e verificamos que o comportamento foi bem satisfatório quando comparado ao número real como demonstram as figuras abaixo.

---

Matrícula: 192.110.164

Pontifícia Universidade Católica do Rio de Janeiro

Curso de Pós Graduação *Business Intelligence Master*
