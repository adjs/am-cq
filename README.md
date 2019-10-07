# Grupo de leitura - Aprendizagem de Máquina e Computação Quântica

Este grupo de leitura tem como objetivo desenvolver o entendimento sobre aprendizagem de máquina aprimorada pela computação quântica e
desenvolver o entendimento sobre aplicações de aprendizagem de máquina.
Durante os encontros serão discutidos dois artigos. Um sobre aprendizagem de máquina clássica e o segundo sobre aprendizagem de máquina quântica.
Além da leitura dos artigos será realizado um exercício de programação para implementar um algoritmo quântico ou um algoritmo de aprendizado clássico.

Para participar do grupo de leitura é necessário participar de um encontro presencial com duração de 1 a 2 horas por semana e
2 a 4 horas para realizar a leitura dos artigos e exercícios de programação.

As referências indicadas para computação quântica são os livros [Quantum Computing for Computer Scientists](https://www.cambridge.org/core/books/quantum-computing-for-computer-scientists/8AEA723BEE5CC9F5C03FDD4BA850C711)
e [Quantum Computation and Quantum Information](https://www.amazon.com/Quantum-Computation-Information-10th-Anniversary/dp/1107002176).
As referências indicadas para Aprendizagem de Máquina são os livros [Machine Learning](https://dl.acm.org/citation.cfm?id=541177)
e o livro [Python Machine Learning](https://www.amazon.com.br/Python-Machine-Learning-scikit-learn-TensorFlow-ebook/dp/B0742K7HYF/ref=sr_1_1?__mk_pt_BR=%C3%85M%C3%85%C5%BD%C3%95%C3%91&keywords=python+machine+learning&qid=1568894841&sr=8-1).

A linguagem de programação utilizada será o Python 3. A distribuição do Python recomendada é o [Anaconda](https://www.anaconda.com/distribution/#download-section).
O Anaconda inclui a biblioteca [scikit-learn](https://scikit-learn.org/stable/) que será utilizada para aprendizagem de máquina.
Para simulação de algoritmos quânticos será utilizado o [qiskit](https://qiskit.org/).

## Semana 1
9:00 as 11:00 - 04/10/2019 - Sala E403/404

- Fawaz, Abdulah, et al. "[Training and Meta-Training Binary Neural Networks with Quantum Computing.](https://www.kdd.org/kdd2019/accepted-papers/view/training-and-meta-training-binary-neural-networks-with-quantum-computing)" Proceedings of the 25th ACM SIGKDD International Conference on Knowledge Discovery & Data Mining. ACM, 2019.
  - Diante da dificuldade em encontrar um conjunto adequado de pesos para redes neurais, o artigo propõe o uso da Computação Quântica (CQ) para representar todos os possíveis parâmetros e hiper-parâmetros de Redes Neurais Binárias (RNB), realizando também o treinamento dessas redes simultaneamente à escolha dos parâmetros
  - A prova de conceito usada no artigo faz uso de uma técnica da CQ conhecida como "amplificação de amplitude" para buscar, dentre todos os conjuntos possíveis de pesos, aquele que mais aumente a acurácia. A aplicabilidade desse método às conectividades e pesos da rede é usada para treinar RNBs
  - Ainda, os autores propõem uma adaptação ao método para permitir representar o cenário de meta-perda de várias arquiteturas de redes neurais simultaneamente, permitindo, assim, treinar e projetar, simultaneamente, uma RNB
  - A principal limitação pontuada pelos autores diz respeito à limitação do hardware quântico atual (quantidade de qubits disponíveis e restrição acerca da quantidade de portas lógicas que podem ser aplicadas). Além disso, questões como *overfitting* e a aceitação de pesos reais também são pontuadas
- Topol, Eric J. "[High-performance medicine: the convergence of human and artificial intelligence.](https://www.nature.com/articles/s41591-018-0300-7)" Nature medicine 25.1 (2019): 44.
  - O artigo analisa recentes avanços na utilização de IA (especialmente *deep learning*/CNN) em vários contextos e áreas da medicina, sendo usada por clínicos, sistemas de saúde e por pacientes.
  - Uma questão importante em uma área crítica como a de saúde, é a explicabilidade do modelo, em que é de extrema ajuda quando o algoritmo pode evidenciar (em uma imagem, por exemplo), como chegou a uma decisão. Apesar de ser conhecida como "black box", alguns estudos fazem essa abordagem, usando por exemplo *heatmaps* e gerando entradas que maximizam um valor de saída, para identificar o que é mais decisório para o algoritmo.
  - As limitações apontadas se referem primeiramente à dificuldade de comparação de resultados entre pesquisas, por diferenças nas metodologias. Também se discute o uso de ROC e AUC como métricas chave para avaliação, dado que desconsideram valores reais de probabilidade e pode levar a confusão quanto a sensibilidade e especificidade (que são de interesse clínico). Além disso, os estudos em geral não possuem validação em ambiente clínico real, contexto no qual será provado a real performance e utilidade (algo que é um desafio na comunidade de aprendizagem de máquina em geral).
  - Apesar de não ser destacado, o problema de [reprodutibilidade em IA](https://www.nature.com/articles/s41746-019-0079-z) pode ser observado, pois na maioria das referências não são divulgados hiper-parâmetros, código e bases de dados, inviabilizando a reprodução dos resultados.
- [opcional] [Otimização baseada no gradiente](semana01/otimizacao_gradiente.ipynb)

## Semana 2
9:00 as 11:00 - 18/10/2019 - Sala

- Grant, E., Benedetti, M., Cao, S., Hallam, A., Lockhart, J., Stojevic, V., ... & Severini, S. (2018). Hierarchical quantum classifiers. [npj Quantum Information, 4(1), 65](https://www.nature.com/articles/s41534-018-0116-9).
- Richa Agarwal; Oliver Diaz; Xavier Lladó; Moi Hoon Yap; Robert Martí. [Automatic mass detection in mammograms using deep convolutional neural networks]
(https://www.spiedigitallibrary.org/journals/Journal-of-Medical-Imaging/volume-6/issue-3/031409/Automatic-mass-detection-in-mammograms-using-deep-convolutional-neural-networks/10.1117/1.JMI.6.3.031409.full?SSO=1).
- [tutorial] Qiskit
- [opcional] Multilayer perceptron
