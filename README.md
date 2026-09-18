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
* 1 - O valor médio das contas é 98,93 reais.
* 2 - Domingo é o dia que tem o maior ticket médio.
* 3 - Observando o Box Plot é possível constatar que há outliers em todos os dias observados, com valores superando os 200 reais.
* 4 - Observando a matriz de correlação é possível perceber que há uma correlação positiva entre gorjeta e o total da conta com valor 0.68, ou seja, há uma correlação moderada/forte, quando o valor da conta sobe, o valor da gorjeta também tende a subir.
* 5 - Olhando para o último gráfico é possível perceber também que não há diferença significativa entre a gorjeta de fumantes e não fumantes.

## 📈 Visualizações e Justificativas de Decisão

1.  **Histograma da Conta:** Mostra a concentração dos valores das contas.
    *   *Decisão:* Definir faixas de preço, combos e promoções para o cliente médio.
2.  **Média da Conta por Dia:** Identifica os dias com maior ticket médio.
    *   *Decisão:* Reforçar equipe e estoque nos dias mais rentáveis (Sábado e Domingo).
3.  **Boxplot da Conta por Dia:** Mostra dispersão, mediana e outliers.
    *   *Decisão:* Investigar contas muito altas (acima de R$ 200) para entender o que esses clientes consomem e tentar replicar o comportamento.
4.  **Dispersão Conta x Gorjeta:** Mostra que contas maiores geram gorjetas maiores.
    *   *Decisão:* Treinar a equipe para fazer *upsell* (oferecer entradas, sobremesas), pois isso aumenta a conta e, consequentemente, a gorjeta.
5.  **Mapa de Calor (Correlação):** Mostra que a conta é o fator que mais impacta a gorjeta (0.68).
    *   *Decisão:* Focar em estratégias de aumento de ticket médio, pois o tamanho da mesa tem menor impacto na gorjeta.
6.  **Média de Gasto por Período (Almoço vs Jantar):** Compara o ticket médio entre os períodos.
    *   *Decisão:* Se o jantar tiver um ticket médio superior, investir em pratos mais elaborados e vinhos para esse período. Se o almoço for mais rentável, criar combos executivos.
7.  **Média de Gorjeta por Fumante:** Compara a gorjeta média entre fumantes e não fumantes.
    *   *Decisão:* Como não há diferença significativa, a gerência não precisa criar estratégias de atendimento segmentadas para fumantes.


Bibliografia Básica:

* AMADEU, C. V. (Org). Banco de dados. São Paulo: Pearson, 2015.
* FÁVERO, L. P. et al. Análise de dados: modelagem multivariada para tomada de decisões. Rio de Janeiro: Elsevier, 2009.
* MACHADO, F. N. R. Banco de dados: projeto e implementação. São Paulo: Saraiva, 2014.
* GÉRON, Aurélien. Mãos à obra: aprendizado de máquina com Scikit-Learn, Keras & TensorFlow: conceitos, ferramentas e técnicas para a construção de sistemas inteligentes. Rio de Janeiro: Alta Books, 2021. 609 p. ISBN 9788550815480.

  Bibliografia Complementar:
  
* ELMASRI, R.; NAVATHE, S. B. Sistemas de banco de dados. São Paulo: Pearson, 2018.
* HURWITZ, J. et al. Big Data para leigos. Rio de Janeiro: Alta Books, 2015.
* MEDEIROS, L. F. de. Inteligência artificial aplicada: uma abordagem introdutória. Curitiba: Intersaberes, 2018.
* VALDATI, Aline de Brittos. Inteligência artificial - IA. São Paulo: Contentus, 2020.
* VARGAS, Ricardo. Gerenciamento de projetos: estabelecendo diferenciais competitivos. 6. ed. Rio de Janeiro: Brasport, 2018.
* PMI, PROJECT MANAGEMENT INSTITUTE. Um guia do conjunto de conhecimentos do gerenciamento de projetos (PMBOK - Project Management Body of Knowledge). 6. ed. São Paulo: Ed. PMI, 2017.
