# projeto-integrador-7-trimestre
1ª Entrega do Projeto Integrador - Ciência de dados aplicado a situações de mercado

Integrante: Paulo Augusto Silva Amorim

Tema: Análise de consumo e gorjetas em um restaurante.

Escopo: analisar padrões de consumo, dias de maior movimento e comportamento de gorjetas para apoiar decisões gerenciais de precificação, escala da equipe e campanhas de atendimento.

Perguntas do negócio:
* 1 - Qual é o valor médio das contas?
* 2 - Qual dia da semana tem o maior ticket médio? (o valor médio que cada cliente gasta em uma compra)
* 3 - Existem contas com valores muito fora do normal? (outliers)
* 4 - O valor da gorjeta está relacionado ao valor total da conta?
* 5 - Fumantes e não fumantes dão gorjetas diferentes?

Base de dados escolhida: https://raw.githubusercontent.com/mwaskom/seaborn-data/master/tips.csv

Link do Colab: https://colab.research.google.com/github/paulogkl/projeto-integrador-7-trimestre/blob/main/CERTO_projeto_integrador_7_trimestre.ipynb

Primeiro, respondendo às perguntas: 
1 - O valor médio das contas é 98,93 reais.
2 - Domingo é o dia que tem o maior ticket médio.
3 - Observando o Box Plot é possível constatar que há outliers em todos os dias observados, com valores superando os 200 reais.
4 - Observando a matriz de correlação é possível perceber que há uma correlação positiva entre gorjeta e o total da conta com valor 0.68, ou seja, há uma correlação moderada/forte, quando o valor da conta sobe, o valor da gorjeta também tende a subir.
5 - Olhando para o último gráfico é possível perceber também que não diferença significativa entre a gorjeta de fumantes e não fumantes.

Agora extraindo mais algumas informações:
 - Há uma correlação positiva entre o tamanho da mesa e a gorjeta;
 - Tickets médios no valor de 200 reais ou mais são raros;
 - Os dias com contas mais altas são sábado e domingo, indicando que o restaurante pode fazer um menu ou promoções diferenciadas, aumentando o lucro;
 - Como a média das contas é 98 reais, fazer pratos e promoções específicos para essa faixa de preço é uma boa ideia.


Bibliografia

* AMADEU, C. V. (Org). Banco de dados. São Paulo: Pearson, 2015.
* FÁVERO, L. P. et al. Análise de dados: modelagem multivariada para tomada de decisões. Rio de Janeiro: Elsevier, 2009.
* MACHADO, F. N. R. Banco de dados: projeto e implementação. São Paulo: Saraiva, 2014.
* GÉRON, Aurélien. Mãos à obra: aprendizado de máquina com Scikit-Learn, Keras & TensorFlow: conceitos, ferramentas e técnicas para a construção de sistemas inteligentes. Rio de Janeiro: Alta Books, 2021. 609 p. ISBN 9788550815480.
