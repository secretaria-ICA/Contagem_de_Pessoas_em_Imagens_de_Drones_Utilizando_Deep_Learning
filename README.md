# Contagem de pessoas utilizando deep learning e imagens aéreas
#### Aluno: [Mateus Furlin Bampi](https://github.com/MateusBampi).
#### Orientador: [Manoela Kohler](https://github.com/manoelakohler).

---

Trabalho apresentado ao curso [BI MASTER](https://ica.puc-rio.ai/bi-master) como pré-requisito para conclusão de curso e obtenção de crédito na disciplina "Projetos de Sistemas Inteligentes de Apoio à Decisão".

---

### Resumo

O projeto, desenvolvido em Python, consistiu em criar um modelo de deep learning para a detecção e contagem de pessoas. Para o treinamento, utilizou-se um banco de dados com 2000 frames de um vídeo de uma webcam em um shopping center. As imagens já estavam rotuladas com o número de pessoas dentro da imagem.

A rede neural sequencial utilizou o otimizador Adam e as função de ativação Relu e foi dividida em duas partes: 
  
  1. Uma rede convolucional, com duas camadas convolucionais para extrair informações das imagens, duas camadas de maxpooling como forma de reduzir o tamanho das informações, uma camada de dropout para melhor a performance do modelo e uma camada de flattening para passar as informações para a parte full dense da rede neural;

  2. A rede full dense consistiu em duas camadas, uma com 128 neurônios para aprender o que se passa na imagem, e uma com um neurônio para dar o resultado final.

O treinamento foi bem sucedido e foi capaz de realizar inferências em imagens que nunca havia visto dentro deste mesmo dataset como demonstram as figuras abaixo.

![thumbnail_image (1)](https://user-images.githubusercontent.com/84750991/126877818-6657956e-fbda-4f2a-b713-461a07dd5c73.png)

![thumbnail_image](https://user-images.githubusercontent.com/84750991/126877782-326ee0d8-6180-4786-94d5-18278ded8aaf.png)

Em seguida, realizamos inferências em imagens capturadas por drones e verificamos que de maneira geral, o comportamento foi bem satisfatório em certos ambientes. Porém, em algumas das inferências, o modelo teve uma performance muito ruim, o que provavelmente pode ser explicado pela base de treinamento que foi utilizada com pouca variedade de ambientes. Algumas das inferências são demonstradas abaixo:

![Inferencia 1 teste](https://user-images.githubusercontent.com/84750991/126880357-e700f87b-be4e-4d30-bf70-053e69659a88.png) ![Inferência 2 teste](https://user-images.githubusercontent.com/84750991/126880367-c8c84b23-ac33-4f7f-b432-b977425940b4.png)

![Inferência 3 teste](https://user-images.githubusercontent.com/84750991/126880406-ca08a6dd-a05f-458f-a0cb-e842e4348b56.png) ![Inferencia 4 teste](https://user-images.githubusercontent.com/84750991/126880413-cb6b8609-6e72-4cc8-8497-49f813ebf6ed.png)

![Inferencia 5 teste](https://user-images.githubusercontent.com/84750991/126880451-20bed006-6b4f-4140-9ec6-71c6c67f3595.png) ![Inferencia 6 teste](https://user-images.githubusercontent.com/84750991/126880478-7eec2449-e5f8-41d6-a940-67c94ff7bb08.png)


---

Matrícula: 192.110.164

Pontifícia Universidade Católica do Rio de Janeiro

Curso de Pós Graduação *Business Intelligence Master*
