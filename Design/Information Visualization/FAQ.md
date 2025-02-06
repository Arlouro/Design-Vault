### 1. Quais são os principais tipos de visualização de dados e como se diferenciam?

Existem quatro principais tipos de visualização: 
- **Visualização Científica (SciVis)**, que lida com dados volumétricos e problemas em 3D, com geometria pré-definida; 
- **Visualização Geográfica (GeoVis)**, que se concentra em dados geográficos usando técnicas bem estabelecidas; 
- **Visualização de Informação (InfoVis)**, que trabalha com dados abstratos e requer um design cuidadoso e estética apurada;
- **Visual Analytics (VA)**, que combina DataVis com _data mining_, focando na análise de algoritmos de _machine learning_ e seus resultados. 
A principal diferença reside no tipo de dado com o qual lidam e a abordagem usada.

### 2. Por que a visualização de dados é importante e quais os seus benefícios?

A visualização de dados é crucial para lidar com grandes volumes de informação, ultrapassando as limitações da capacidade humana de cognição, memória e também as limitações computacionais. Permite revelar padrões, relações quantitativas e detalhes específicos nos dados através do sistema cognitivo-visual, amplificando a cognição ao substituir o pensamento abstrato pela perceção visual. Além disso, facilita a análise e a memorização, e pode revelar informações que seriam difíceis de identificar usando apenas métodos estatísticos.

### 3. Como são construídas e caracterizadas as redes (ou grafos) em visualização de dados?

As redes são estruturas formadas por **nós** (elementos) e **arestas** (conexões). As arestas podem ser **direcionadas** ou **não direcionadas**, indicando a direção da interação entre os nós. Elas também podem ser **ponderadas**, expressando a força da conexão. Cada nó tem um **grau** que indica o número de conexões, e pode ter um **grau de entrada** (conexões para o nó) e um **grau de saída** (conexões do nó). A **centralidade** de um nó indica a sua importância na rede. As redes podem ser também do tipo **bipartite**, como leitores e livros.

### 4. Quais as principais transformações e pré-processamentos que podem ser aplicados aos dados antes da visualização?

Os dados podem passar por várias transformações. Para reduzir a assimetria (_skewness_) dos dados, podem ser usadas transformações logarítmicas. Valores discretos podem substituir categorias, como {baixo, médio, alto} por {0, 1, 2}. Os dados contínuos podem ser discretizados em categorias, como intervalos de peso. A **agregação** é usada para calcular valores derivados. A normalização dos dados também é um passo importante, bem como a transformação de dados qualitativos (nominais e ordinais) para dados numéricos.

### 5. Quais são os tipos de variáveis usadas em visualização de dados e como se diferenciam os níveis de medição?

Existem dois tipos principais de variáveis: **categóricas** (nominais e ordinais) e **quantitativas** (discretas e contínuas). As variáveis **nominais** são categorias sem ordem, como tipo de bicicleta, enquanto as **ordinais** têm uma ordem, como nível de doença. As variáveis **quantitativas discretas** têm valores numéricos separados, como número de filhos, e as **contínuas** têm um intervalo infinito de valores, como tempo ou temperatura. Os níveis de medição incluem **nominal**, **ordinal**, **intervalar** (com distâncias significativas, mas sem zero verdadeiro) e **rácio** (com zero verdadeiro e razões possíveis).

### 6. Quais os elementos visuais fundamentais usados na visualização de dados (semiologia gráfica) e como podem ser utilizados?

Os elementos visuais fundamentais incluem **pontos** (0D), **linhas** (1D) e **áreas** (2D), que são usados como _marcas_. Os **canais visuais** controlam a aparência destas marcas, e incluem **tamanho**, **valor** (brilho), **textura**, **cor**, **orientação** e **forma**. Existem canais de **identidade** (o que/onde) e de **magnitude** (quanto). Os níveis de organização da perceção incluem **qualitativo**, **ordenado** e **quantitativo**. Os princípios da _Gestalt_ (proximidade, semelhança, conexão, fecho, figura-fundo) guiam a forma como os elementos visuais são agrupados e percebidos.

### 7. Quais são os principais tipos de escalas usadas em D3.js e como funcionam?

Em D3.js, as **escalas** são usadas para mapear dados brutos para atributos visuais. Existem escalas **lineares** (d3.scaleLinear()), **potências** (d3.scalePow()) para mapear valores contínuos para outros contínuos. Há ainda escalas **ordinais** (d3.scaleOrdinal()), que mapeiam valores discretos para outros valores discretos, como cores de um esquema predefinido. As escalas recebem um domínio (domain()) que mapeia para um _range_ (range()) visual. As funções d3.axisTop(), d3.axisBottom(), d3.axisLeft() e d3.axisRight() criam eixos que usam estas escalas para apresentar os seus _ticks_ de forma visual.

### 8. Quais são as diferentes tarefas analíticas em visualização de dados e como o _clustering_ contribui para essas tarefas?

As tarefas analíticas incluem **encontrar extremos**, **ordenar**, **encontrar intervalo** e outras. O _clustering_ é útil para agrupar dados com base em semelhanças, usando métodos **hierárquicos** (aglomerativos e divisivos) e **particionais** (K-means, DBSCAN). O _clustering_ é aplicado em diversas áreas como _marketing_, biologia e bibliotecas, ajudando a dar estrutura aos dados e a identificar padrões. Os métodos de _clustering_ usam medidas de distância como a **Euclidiana**, a **Manhattan** e **Hamming** para agrupar os dados.

---

1. **O que é visualização de informação e qual o seu propósito fundamental?**
	A visualização de informação é a representação gráfica e visual de conjuntos de dados, especialmente grandes conjuntos, com o objetivo de tornar esses dados mais acessíveis ao entendimento, facilitar a análise e exploração, e expandir o nosso conhecimento sobre os mesmos. Esta representação é feita através da codificação das variáveis dos dados em variáveis visuais, expondo as relações e valores entre elas. O objetivo principal é comunicar informação complexa de forma clara e eficaz, permitindo que os utilizadores identifiquem padrões, tendências e _insights_ que poderiam ser difíceis de discernir através de tabelas ou dados brutos.
2. **Quais são as variáveis visuais e implantações mais comuns utilizadas na visualização de informação?** 
	As variáveis visuais (ou canais visuais) são os elementos que usamos para representar os dados graficamente. As mais comuns incluem: posição (X e Y), forma, tamanho, textura, cor, valor (nível de claro/escuro) e orientação. As implantações (ou marcas) referem-se à forma como as variáveis visuais são apresentadas, sendo as mais comuns o ponto, a linha e a área. A combinação de variáveis visuais e implantações permite codificar dados de forma a revelar diferentes aspetos dos mesmos.
3. **O que são propriedades percetivas e como se relacionam com a eficácia de uma visualização?**
	As propriedades percetivas referem-se à forma como o nosso sistema visual interpreta as variáveis visuais. As propriedades podem ser: quantitativo (se há leitura numérica), ordenado (se permite perceber uma ordem), associativo (se permite agrupar elementos) e seletivo (se permite selecionar elementos dentro de um grupo). A escolha das variáveis visuais e implantações adequadas, considerando as suas propriedades percetivas, é crucial para criar uma visualização eficaz. Por exemplo, usar o tamanho para representar valores quantitativos permite uma interpretação mais intuitiva do que o uso da cor para a mesma função.
4. **Qual a diferença entre _clustering_ hierárquico e particional, e qual a sua utilidade em visualização de dados?**
	O _clustering_ hierárquico constrói uma hierarquia de agrupamentos, onde cada elemento começa como um cluster separado, e sucessivamente são agregados ou divididos. O resultado é geralmente representado por um dendograma. Já o _clustering_ particional divide os dados em grupos distintos, onde cada elemento pertence a apenas um grupo. A escolha entre um ou outro depende do objetivo: o hierárquico é útil para explorar as relações hierárquicas nos dados e o particional para identificar grupos distintos sem uma estrutura hierárquica explícita. Ambos permitem identificar estruturas e padrões nos dados que podem ser visualizados.
5. **Quais são as etapas principais no processo de visualização de informação e o que acontece em cada uma delas?**
	O processo de visualização de informação envolve as seguintes etapas:
	1. **Definição do Domínio do Problema:** 
	   Entender o problema, os utilizadores e os objetivos da visualização.
	2. **Tradução:** 
	   Esta fase inclui a abstração dos dados (definir quais dados são relevantes, seus tipos - categóricos, quantitativos -, e ordenamento) e a abstração das tarefas (definir porque é que o utilizador precisa desta visualização).
	3. **Design Visual:** 
	   Escolher as variáveis visuais, as implantações e interações (zoom, panning, linking, brushing, etc) adequadas para codificar os dados e para facilitar a interação com a visualização.
	4. **Implementação:** 
	   Transformar os dados brutos em tabelas e estruturas visuais através de um _pipeline_.
	5. **Validação:** 
	    Avaliar se a visualização alcança os seus objetivos iniciais, tendo em conta o problema, a abstração de dados, design visual e, por vezes, a eficiência algorítmica.
6. **Em que situações devemos usar a média e a mediana como medida de tendência central e quais as suas limitações?**
	A média é usada para variáveis numéricas, tanto discretas quanto contínuas, e é adequada quando os dados têm uma distribuição simétrica (não _skewed_). A sua principal limitação é a sensibilidade a valores extremos (_outliers_) que podem distorcer o seu valor. A mediana é mais robusta a _outliers_ e é preferível quando a distribuição dos dados é _skewed_ (assimétrica) ou quando há dados extremos que podem influenciar a média. A mediana representa o valor central de um conjunto de dados ordenados. Em termos mais gerais, a moda é utilizada quando queremos saber qual o valor mais frequente (útil para variáveis nominais), a mediana (para variáveis ordinais ou quantitativas _skewed_) e a média para variáveis quantitativas (distribuições não _skewed_).
7. **O que é o "Ink Ratio" defendido por Edward Tufte e como se relaciona com a eficácia de um gráfico?**
	O "Ink Ratio" ou "Data-Ink Ratio" defendido por Edward Tufte, refere-se à proporção entre a quantidade de tinta utilizada para representar dados (tinta de dados) e a quantidade total de tinta utilizada no gráfico. O objetivo é maximizar a quantidade de tinta que representa dados, minimizando a tinta que não tem relevância informativa (tinta não-dados). Uma visualização com um bom "Ink Ratio" é mais clara, concisa e eficaz, pois concentra-se na informação essencial e evita elementos visuais desnecessários que podem distrair o utilizador.
8. **Quais são os princípios da Gestalt aplicados à visualização e como podem melhorar a interpretação de um gráfico?**
	Os princípios da Gestalt, que são regras que descrevem como o nosso cérebro organiza e interpreta a informação visual, são importantes para um bom design de visualização. Os princípios incluem: **proximidade** (elementos próximos são agrupados), **continuidade** (perceção de elementos que formam uma linha ou padrão), **conectividade** (elementos ligados são percebidos como um grupo), **similaridade** (elementos similares são agrupados), **simetria** (elementos simétricos são percebidos como um todo), **destino comum** (elementos que se movem juntos são agrupados), **figura-fundo** (capacidade de separar um objeto do seu fundo) e **fechamento** (tendência a preencher espaços vazios). Aplicar estes princípios ajuda a criar visualizações mais intuitivas e fáceis de interpretar, permitindo que os utilizadores percebam a informação de forma mais eficiente e rápida. A **perceção relativa** também é importante, pois a nossa perceção de um elemento depende do seu contexto.