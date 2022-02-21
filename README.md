# TI_Rede_Neural
Trabalho de Implementação - Rede Neural

Equipe: Mayron Boelling da Silva e Lucas de Liz Frutuoso;

Problema: Desenvolver uma rede neural capaz de classificar uma mão de poker. As entradas fornecidas para fazer a classificação serão naipes de cada carta(número de 1 a 4 representando(copas, espadas, ouro, paus) e o seu respectivo ranking(número de 1 a 13 representando(Ás, 2, 3, ... Dama, Rei). Uma mão de poker é classificada pela combinação de 5 cartas e seus respectivos naipes e valores, onde é possível obter as seguintes combinações: 
  1: Um Par; Duas cartas do mesmo valor;
  2: Dois Pares; Duas cartas de um mesmo valor, outras duas cartas diferentes de mesmo valor;
  3: Trinca; Três cartas do mesmo valor;
  4: Sequência; Cinco cartas em sequência;
  5: Flush; Cinco cartas do mesmo naipe.
  6: Full house; Três cartas do mesmo valor, e duas outras cartas diferentes de mesmo valor.
  7: Four of a kind; four equal ranks within five cards
  8: Straight flush; Cinco cartas em ordem numérica, todas do mesmo naipe.
  9: Royal flush; sequência de Ás, Rei, Dama, Valete e Dez, todos com o mesmo naipe.

DataSet: Será utiliza o dataset pronto: Poker Hand Data Set - https://www.kaggle.com/anupamujawane/poker-hands-dataset
  Ele fonece uma tabela com 11 colunas organizadas da seguinte forma: s1(naipe da carta1), c1(rank da carta1, s2(naipe da carta2), c2(rank da carta2), s3(naipe da carta1), c3(rank da carta3), s4(naipe da carta1), c4(rank da carta4), s5(naipe da carta5), c5(rank da carta5), class(mão de poker(0-9))
  
Tecnologia: Foi implementado na linguagem Python e Scikitlearn.

Técnica: Foi implementado uma Rede Neural Multilayer Perceptron onde a melhor combinação encontrada durante o desenvolvimento, possui 10 camadas de entrada, 2 camadas ocultas com 25 neurônio cada, um coeficiente de aprendizagem de 0.01, 400 iterações. Foi utilizado a estratégia de validação Holdout onde foi separado 2/3 do dataset para o conjunto de teste. Com esta combinação obteve-se uma acurácia de 0.9974.


Link para a apresentação: https://youtu.be/6jmMnbtJM_M



Instruções para testar: 
  1: acessar o link-> https://colab.research.google.com/drive/1OeAzC0qa5mjkKz-ShLhQ70zhXVHneC9-#scrollTo=mo2vWeUGiKBT,
  2: fazer o download do dataset: https://www.kaggle.com/anupamujawane/poker-hands-dataset
  3: importar o arquivo no colab;
  4: pode-se executar todo o código de uma vez pressionando ctrl+F9 ou executar uma célula de cada vez;
