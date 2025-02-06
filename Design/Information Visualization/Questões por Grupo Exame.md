### **Grupo de Perguntas 1: Questões Genéricas sobre Visualização de Informação, Percepção, Modelos de Visualização, Aplicações, etc.**

1. **O que entende por visualização de informação e qual o seu principal objetivo?**  
    A visualização de informação é a representação gráfica e visual de conjuntos de dados, geralmente grandes, de forma a torná-los mais acessíveis ao entendimento, expandindo o nosso conhecimento e permitindo a sua análise e exploração. O objetivo principal é facilitar a compreensão dos dados através da codificação visual das variáveis em variáveis visuais, representando as relações entre elas.
    
2. **Como é que a codificação visual de variáveis de dados em variáveis visuais contribui para a visualização de informação?**  
    A codificação visual mapeia atributos dos dados em canais visuais, como posição, forma, tamanho, cor, valor, orientação e textura. Esta transformação permite que os dados sejam percebidos visualmente, facilitando a identificação de padrões, relações e tendências. As implantações (ponto, linha, área) são utilizadas para representar os dados.
    
3. **O que é o conceito de "Ink Ratio" e qual a sua importância na visualização de informação?**  
    O "Ink Ratio" refere-se à maximização da quantidade de informação mostrada numa visualização, através da otimização do uso de pixels informativos. O objetivo é que a proporção de tinta utilizada no gráfico represente a maior quantidade de informação possível, diferenciando-se dos pixels que não acrescentam nada de informativo. É a proporção da quantidade do gráfico que não pode ser apagada sem haver perda de informação.
    
4. **O que é a semiologia gráfica e qual a sua importância no contexto da visualização de informação?**  
    A semiologia gráfica é o estudo dos signos, símbolos e seus significados. No contexto da visualização de informação, é fundamental para compreender como os elementos gráficos (marcas visuais, canais visuais) são percebidos e interpretados. Jacques Bertin foi o primeiro a teorizar as bases para o uso de elementos gráficos. As leituras dos seus significados podem variar consoante vários aspetos, como culturas, idades e género.
    
5. **Quais são as variáveis visuais e como podem ser usadas para representar diferentes tipos de dados?**  
    As variáveis visuais são atributos visuais que podem ser utilizados para codificar dados, incluindo posição X/Y, forma, tamanho, textura, cor, valor (claro/escuro) e orientação. Cada uma destas variáveis pode ser mais ou menos adequada para representar diferentes tipos de dados, dependendo das suas propriedades percetuais (quantitativo, ordenado, associativo, seletivo).
    
6. **Explique as propriedades percetuais das variáveis visuais (Quantitativo, Ordenado, Associativo, Seletivo) e dê exemplos.**
    
    - **Quantitativo:** A variável permite uma leitura numérica ao se fazer mudanças no seu valor. Exemplo: tamanho de uma barra.
    - **Ordenado:** Permite a perceção de ordem nos diferentes valores da variável. Exemplo: escala de cores do mais claro para o mais escuro.
    - **Associativo:** A mudança na variável permite distinguir e agrupar elementos. Exemplo: usar cores diferentes para distinguir diferentes categorias.
    - **Seletivo:** Permite diferenciar/selecionar dentro de um grupo. Exemplo: distinguir diferentes tipos de peixe usando formas diferentes.
7. **Quais são os passos do processo de visualização?**  
    O processo de visualização inclui as seguintes etapas:
    
    1. Definição do domínio do problema e do target user.
    2. Tradução:
        - Data Abstraction: definir os tipos de atributos a apresentar (categóricos, quantitativos).
        - Task Abstraction: definir porque é que o utilizador usa a visualização.
    3. Design Visual: escolher encodings visuais e interações.
    4. Implementação da Visualization Pipeline.
    5. Validação.
8. **Como é que a abstração de dados (Data Abstraction) e a abstração de tarefas (Task Abstraction) influenciam o design de visualizações?**  
    A Data Abstraction define que tipo de atributos serão apresentados (categóricos, ordinais ou quantitativos) e o seu tipo de ordenamento (sequencial, divergente, cíclico). A Task Abstraction define o motivo pelo qual o utilizador utiliza a visualização. Ambas abstrações são essenciais porque determinam a escolha das variáveis visuais e das interações mais adequadas.
    
9. **Explique o conceito de expressividade e eficiência em visualização de informação.**
    
    - **Expressividade:** Refere-se à capacidade da visualização de representar todos os dados relevantes do dataset, tendo em conta o problema, objetivo e questões a serem respondidas. Mede a concentração de informação.
    - **Eficiência:** Refere-se à rapidez e clareza com que a visualização pode ser percecionada.
10. **Quais são os princípios de design que devem ser considerados na criação de visualizações eficazes?**  
    Os princípios de design incluem escolher o modelo de visualização adequado para o tipo de dados e objetivos; usar variáveis visuais apropriadas; considerar o uso de cores, formas, tamanhos e posicionamento; e garantir que a visualização seja fácil de entender.
    
11. **Quais são os princípios da Gestalt e como se relacionam com a perceção visual?**  
    Os princípios da Gestalt descrevem como os seres humanos organizam visualmente os elementos:
    
    - **Proximidade:** Agrupar elementos com base na proximidade espacial.
    - **Continuidade:** Perceção de unidades de elementos.
    - **Connectedness:** Elementos visuais ligados percetualmente.
    - **Semelhança:** Criação de unidades percetuais por semelhanças.
    - **Simetria:** Reflexões de elementos que parecem um todo.
    - **Common Fate:** Perceção de movimento, elementos na mesma direção.
    - **Figure and Ground:** Identificar objeto em espaços não preenchidos.
    - **Closure:** Tendência de fecharmos ligações.
    - **Relative Perception:** A perceção dos elementos é relativa ao contexto.
12. **Como funciona o modelo de perceção visual de Ware (Preattentive, Attentive, Sequential)?**  
    O modelo de Ware divide a perceção visual em três etapas:
    
    1. **Preattentive:** Visão geral e paralela, onde se encontram elementos que se destacam por tamanho, cor, orientação.
    2. **Active Attentive:** Processamento mais apurado, onde se encontram regiões e padrões simples.
    3. **Sequential Goal-directed:** Análise de partes específicas, relacionada com memória a longo tempo.

---

### **Grupo de Perguntas 2: Análise Formal de Visualizações**

![bar-graph.jpeg](https://www.kaggleusercontent.com/kf/216615941/eyJhbGciOiJkaXIiLCJlbmMiOiJBMTI4Q0JDLUhTMjU2In0..a-gmsVL6-9Of8v70E_IrTQ.Yf4qk7xA6s11tq93VLHgdpFIvdvAJhpQ67bA24oQlI8rBuO2M52Zl3xRIfBRzjH5FiOx5-aIfNegRxV_UuPkAMXCm_Ej05Br6xDJ3rC2Q38pNRV9K47-3xmUWdBhaxNU8J2Mg4mDDRtb73m-kkV2ZkHH_5JwJ131dT2cpofD5O4YveMWPu_AZGf7svZ1AyMqCEArNoDMKC6vNkTVSMamHLv98LHpkyaDtvLHeiXYFfvQp32BA-3JPfguCg3OeW7unMhEZfyPSYgwfEVBOuvjoA80H1tXF2j7pQpWXgpq-xFsh2oqxMUv3-gi0QdQaF4_ByHXADl8VTsh7N2PH1S6QvTr_QWTLwuHnV_d_nmO3IYHsKj1HUr9MssaXMApkiGx98wi40sQXgQdq10L2bnJ7ri7gQ24SjMJuVxj3VTm15b1m_3mp-OipRvJ9WtouekE95L6S87ViSULsC7r2jfzBNp4wwO4_GLXYC9rFbYC3kH6bDYlGwWNY_pojDZ3ZQivXN2_QYhcrlIby48zo36GkrCVQKh77J38BX_A9mdRgACoRzT02JwyCbe7Y9KRLX00TAbqcxDbvw_rz3yRIH498CylzXg4pp5LUTRfZRzXBdXAzMjOQqWoy0rc79PbHY2mWDhOpOEw3iLfUns5-AdjPS6HpHTcCfhBUQ-bjr9_RsglJSBnX_Hnto7-ZfRUgzCn.8Mc7vBjGlKbl-u4gcoUk-w/__results___files/__results___8_0.png)

1. **Dado um gráfico específico (por exemplo, um gráfico de barras, um scatter plot, um heatmap), identifique as variáveis visuais usadas e os seus atributos.**  
    *Identifique as variáveis visuais (posição, cor, tamanho, forma, etc.) presentes no gráfico e descreva como cada variável é usada para representar os dados.*
	**Variáveis Visuais Usadas**
	- **Posição:** 
		- **Representação:** O eixo Y é usado para listar os nomes das empresas, organizando-as em uma ordem que reflete os valores do eixo X;
		- **Atributo:** A posição vertical indica a categoria da empresa.
	- **Tamanho (Comprimento da Barra):**
		- **Representação:** O comprimento da barra horizontal representa o valor da receita em milhões de dólares (USD);
		- **Atributo:** Valores maiores têm barras mais longas, facilitando comparações entre empresas.
	- **Cor:**
		- **Representação:** Gradiente de cor (do azul mais escuro para o mais claro) reflete a magnitude da receita. Barras com receitas maiores são mais escuras;
		- **Atributo:** A intensidade da cor serve como um reforço visual para destacar as diferenças nos valores.
	- **Valor:**
		- Os valores são mais elevados nas barras mais escuras e maiores, enquanto são mais baixos nas barras mais claras e menores, variando dependentemente do tamanho e cor; 

2. **Analisando a visualização apresentada, descreva as implantações (marcas) usadas (ponto, linha, área) e as suas propriedades percetuais (quantitativo, ordenado, etc.).**  
	 *Descreva se os dados são representados por pontos, linhas ou áreas e as propriedades percetuais de cada implantação, explicando se são adequadas para os dados representados.*
	 
3. **Para a visualização apresentada, determine qual é a relação entre os elementos visuais (Semelhança, Ordem, Proporção).**  
	*Analise as relações visuais entre os elementos do gráfico, como semelhança (elementos semelhantes agrupados), ordem (elementos dispostos sequencialmente) e proporção (elementos que representam quantidades relativas).*
    
4. **Com base na visualização apresentada, descreva o tipo de dado representado e se os canais visuais foram utilizados adequadamente (por exemplo, posição, cor, tamanho).**  
	 *Identifique se os dados são categóricos, ordinais ou quantitativos e avalie se as variáveis visuais foram bem escolhidas e utilizadas para representar esse tipo de dados.*
    
5. **Avalie a expressividade e eficácia da visualização dada, considerando o tipo de dados e o objetivo da visualização.**  
	*Avalie se a visualização representa todos os dados relevantes (expressividade) e se a informação é clara e fácil de entender (eficiência), considerando o tipo de dados e o objetivo pretendido.*
    
6. **Usando o exemplo do gráfico de Minard, descreva as variáveis visuais e suas propriedades.**  
    *Analise o gráfico de Minard, identificando as variáveis visuais usadas (posição X/Y, área, cor, tamanho) e suas propriedades (quantitativas, seletivas e ordenadas).*
    

---

### **Grupo de Perguntas 3: Questões sobre Estatística Descritiva**

1. **Defina média, mediana e moda e explique as diferenças entre elas.**  
    - **Média:** Soma de todos os valores dividida pelo número de valores.
    - **Mediana:** Valor central de um conjunto de dados ordenados.
    - **Moda:** Valor que aparece com maior frequência.  
        A média é sensível a valores extremos, enquanto a mediana não é afetada por eles. A moda representa o valor mais comum.
2. **Em que situações é mais apropriado usar a média e quando é preferível usar a mediana?**  
    A média é mais apropriada para dados com distribuição normal e sem valores extremos. A mediana é preferível quando os dados são assimétricos ou têm outliers, pois não é afetada por eles.
    
3. **O que são quartis e como são calculados?**  
    Quartis são valores que dividem um conjunto de dados ordenados em quatro partes iguais.
    - Q1 (1º quartil): 25% dos dados.
    - Q2 (2º quartil): 50% (é a mediana).
    - Q3 (3º quartil): 75% dos dados.  
        Os quartis são calculados usando fórmulas específicas para conjuntos de dados pares e ímpares.
4. **Como pode identificar a frequência de um dado em diferentes tipos de visualizações (dot plot, histograma, tabela de frequências)?**  
    - **Dot Plot:** Cada ponto representa uma observação; a frequência é visualizada pelo número de pontos em cada valor.
    - **Histograma:** A frequência é representada pela altura das barras.
    - **Tabela de frequências:** A frequência é diretamente listada na tabela para cada valor.
5. **Explique a diferença entre uma distribuição de frequência agrupada e não agrupada.**  
    - **Distribuição Agrupada:** Os dados são organizados em classes de intervalos de valores.
    - **Distribuição Não Agrupada:** A frequência de cada valor é apresentada individualmente.
6. **Descreva como os outliers podem afetar a análise estatística e como podem ser tratados.**  
	Outliers são valores extremos que podem distorcer a média e outras estatísticas descritivas. Podem ser tratados removendo-os, transformando os dados ou usando métodos estatísticos robustos.
7. **O que são dados contínuos e discretos e como podem influenciar a escolha das visualizações?**  
    - **Dados Contínuos:** Podem assumir qualquer valor dentro de um intervalo (ex.: temperatura); frequentemente visualizados com gráficos de linhas ou áreas.
    - **Dados Discretos:** Assumem valores fixos, sem casas decimais (ex.: número de irmãos); frequentemente visualizados com gráficos de barras ou pontos.  
        A escolha da visualização deve ser adequada ao tipo de dado.

---

### **Grupo de Perguntas 4: Exercício de Clustering**

1. **Explique as diferenças entre clustering hierárquico e particional.**  
    O clustering hierárquico constrói uma hierarquia de clusters, onde os clusters podem estar contidos dentro de outros clusters. O clustering particional divide os dados em clusters sem hierarquia.
    
2. **Descreva o processo de construção de um dendrograma em clustering hierárquico.**  
    Um dendrograma é um diagrama em árvore que mostra a hierarquia de clusters. É construído unindo os pontos de dados e os clusters em etapas, com base na sua similaridade.
    
3. **Desenhe um esquema de uma rede ou árvore, explicando o que entende pelas suas propriedades percetuais.**  
    Deve incluir um desenho de uma rede ou árvore, destacando as propriedades percetuais como a hierarquia, conexões e agrupamentos visuais.
    

---

### **Grupo de Perguntas 5: Análise Crítica de Visualização**

![bad-3D-BarGraph](https://www.jotform.com/blog/wp-content/uploads/2022/12/image-1-3.png)

1. **Dado um gráfico, identifique os seus pontos fortes e fracos.**  
	*Analise os aspetos positivos e negativos da visualização, considerando a sua expressividade, eficiência e adequação aos dados.*
    
2. **Quais os problemas de determinado gráfico?**  
	*Identifique problemas específicos como o uso incorreto de variáveis visuais, dificuldade em compreender a informação e má utilização do espaço.*
    
3. **Sugira alternativas de visualização para um gráfico específico, justificando a sua escolha e desenhando a sua solução.**  
	*Proponha uma visualização diferente, explicando o motivo da escolha, como melhora a clareza e a eficácia da informação, e desenhe a solução proposta.*
    
4. **O que está mal com determinada visualização?**  
	*Identifique os problemas da visualização, como a falta de clareza, escolha inadequada de variáveis visuais ou má utilização do espaço.*
    
5. **Como melhoraria esta visualização, tendo em conta o objetivo?**  
    *Proponha melhorias com base no objetivo da visualização, como escolher uma visualização mais adequada, ajustar as variáveis visuais ou adicionar interatividade.* 
    