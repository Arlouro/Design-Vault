**1. Introdução à Visualização de Informação (1_VI_Intro.pdf)**

- **Âmbito da Visualização:Visualização Científica (SciVis):** Dados geométricos, problemas 3D (e.g., dados volumétricos).
- **Visualização Geográfica (GeoVis):** Dados geográficos, fenómenos geográficos. Técnicas bem estabelecidas.
- **Visualização de Informação (InfoVis):** Dados abstratos. Necessidade de criar ou desenhar técnicas adequadamente. Estética cuidada.
- **Análise Visual (VA):** Combinação de DataVis com data mining. Análise de algoritmos de ML.
- **Importância dos Grafos:** São essenciais para comunicar informação quantitativa devido à capacidade do sistema cognitivo-visual para perceber padrões geométricos.
- "Padrões e relações quantitativas nos dados são facilmente revelados por grafos devido ao enorme poder do sistema cognitivo-visual para perceber padrões geométricos."
- O sistema visual consegue sumarizar grandes quantidades de informação, identificar características distintivas e focar em detalhes.
- **Objetivos da Visualização:**Lidar com grandes volumes de dados.
- Superar limitações humanas de cognição e memória, e limitações computacionais de tempo de processamento e memória.
- Otimizar o espaço de _display_ para codificar a informação de forma eficaz.
- "A representação externa substitui a cognição pela percepção."
- Facilitar a análise e memorização da informação.
- Revelar informação.
- **Exemplos Históricos e Casos de Uso:**Visualização da dívida dos EUA para comparar o crescimento das despesas e receitas.
- Pirâmide populacional 3D.
- Horários de comboios, como um "calculador gráfico" para determinar os comboios mais rápidos e os pontos de intersecção.
- Diagrama do metro de Londres, com um foco na sequência das estações e não na sua posição geográfica exata.
- Visualização da internet, mostrando os caminhos de conectividade de IPs.
- Nuvens de tags ("word clouds") para resumir grandes volumes de texto.

**2. Processo e Design de Dados (2_VI_Process_DataDesign.pdf)**

- **Processo de Visualização:**As variáveis gráficas podem ser remapeadas.
- O _view_ pode ser movido (panning).
- **Pipeline da Visualização:Desempenho Computacional:** Eficiência no processamento de dados.
- **Interatividade:** Combinação do desempenho computacional e da interação do utilizador.
- **Funcionalidade:** Focada na experiência do utilizador.
- **Validação:**É um processo que depende do contexto.
- Pode ser difícil.
- Usa um modelo "nested" com quatro níveis de problemas de design.
- Resolve ameaças imediatas vs. a longo prazo.

**3. Demonstração com HTML, CSS, JavaScript e SVG (2_VI_demo.pdf)**

- **Tecnologias Web:HTML (Hypertext Markup Language):** Define a estrutura do conteúdo usando _tags_ e atributos. Os arquivos HTML são arquivos de texto simples.
- **CSS (Cascading Style Sheets):** Define a apresentação e o estilo dos elementos HTML usando seletores e propriedades.
- Um exemplo de sintaxe CSS é: selector {property: value;}.
- **JavaScript:** Linguagem de _scripting_ para manipular o DOM (Document Object Model) e criar interatividade.
- Tipos de valores: números, strings (onde \ tem um significado especial), booleanos, operadores lógicos (&&, ||), operadores ternários (condição ? seVerdade : seFalso), valores nulos e indefinidos.
- Variáveis com var, let, e const (com diferentes escopos, possibilidades de atualização e declaração).
- Arrays para guardar coleções de dados.
- Estruturas de controlo: if, else if, else.
- **SVG (Scalable Vector Graphics):** Formato para gráficos vetoriais, permitindo desenhar formas como retângulos, círculos, elipses, linhas e texto, diretamente no navegador.
- g tag para agrupar elementos, com atributos.
- **D3.js:** Biblioteca JavaScript para manipulação de dados e criação de visualizações.
- Ex: .data(dataset).enter().append("p").text(function(d) { return "O output: " + d; }) e .style(“color”, function(d) { if (d > 15) { return “red”; } else { return “black”; } });
- Mostra como encadear métodos, carregar dados e usar dados para criar elementos visuais.

**4. Estatísticas com D3.js (3_VI_demo_statistics.pdf)**

- **Dados e Estatísticas:**Uso de ficheiros CSV para importar dados.
- Funções D3.js para cálculos estatísticos:
- d3.mean(data, d => d.Milk); (calcular a média da coluna "Milk").
- d3.min(data, d => d.Milk); (calcular o mínimo da coluna "Milk").
- d3.max(data, d => d.Milk); (calcular o máximo da coluna "Milk").
- Transformação de dados com d3.rollup para agrupar dados e calcular contagens.
- Ex: d3.rollup(data, d => d.length, d => d.Year, d => d.Awards);
- Os dados são processados e transformados antes de serem apresentados visualmente.

**5. Pré-Processamento de Dados (3_VI_preprocessing.pdf)**

- **Redução de Assimetria (Skewness):**Uso de escalas logarítmicas para realçar os valores menores e a sua evolução (ex: 10k, 20k, 30k, 40k, 50k no eixo linear vs. 1, 10, 100, 1k, 10k, 100k no eixo log).
- **Mapeamento de Valores:**Transformar valores não numéricos em numéricos, e.g., {baixo, médio, alto} -> {0, 1, 2}.
- **Discretização (Binning):**Converter dados contínuos em valores discretos, e.g., {<40, 40-50, 50-60, >60}.
- Ex: score de crédito mapeado para {pobre, médio, bom, excelente}.
- **Agregação:**Criar novas variáveis a partir de outras, e.g., BMI = kg/m2.
- **Tipos de Variáveis:Categóricas:Nominal:** Sem ordem (e.g., tipo de bicicleta, etnia).
- **Ordinal:** Com ordem (e.g., grau de doença, opinião).
- **Quantitativas:Discretas:** Número finito de valores (e.g., idade, número de irmãos).
- **Contínuas:** Número infinito de valores possíveis (e.g., temperatura, tempo).
- **Níveis de Medição:Nominal:** Categorias sem ordem.
- **Ordinal:** Categorias com ordem.
- **Intervalar:** Distâncias significativas, mas sem zero verdadeiro (e.g., temperatura em Fahrenheit, testes de IQ).
- **Rácio:** Distâncias significativas com zero verdadeiro (e.g., renda, altura).
- **Estatística:**Ciência de coletar, combinar e resumir dados.
- **Descritiva:** Descreve características de uma amostra ou população.
- **Inferencial:** Faz inferências sobre uma população a partir de uma amostra.
- **Forma da Distribuição:Unimodal:** Simétrica ou assimétrica.
- **Tendência Central:Média:** Soma dos valores dividida pelo número de valores.
- **Mediana:** Valor do meio num conjunto ordenado.
- A média e a mediana são medidas válidas de tendência central, mas em diferentes condições, algumas tornam-se mais apropriadas do que outras. Se a diferença entre a média e a mediana é grande, os dados são assimétricos, e a mediana é a medida mais apropriada.
- **Quartis:**Q1 e Q3 para identificar a distribuição.
- **Box Plot:**Representação gráfica dos quartis, para mostrar a distribuição e detetar _outliers_.
- **Variabilidade:**Medidas de dispersão dos dados.
- **Amplitude:** Diferença entre o máximo e o mínimo.
- **Desvio Médio:** Desvio de cada ponto em relação à média.
- **Variância:** Média dos desvios ao quadrado.
- **Desvio Padrão:** Raiz quadrada da variância.

**6. Escalas e Eixos em D3.js (4_VI_demo_scales.pdf)**

- **Eixos em D3.js:** Funções para gerar elementos visuais, como eixos horizontais e verticais.
- d3.axisTop(), d3.axisBottom(), d3.axisLeft(), d3.axisRight().
- Utilização de .scale() para associar um eixo a uma escala.
- .ticks() para definir o número de _ticks_.
- .tickValues() para definir os valores específicos dos _ticks_.
- .tickFormat() para formatar os valores dos _ticks_.
- d3.format() para formatar valores numéricos (ex: d3.format(‘.1%’)).
- **Escalas em D3.js:**Transformam valores de um domínio de entrada para um alcance de saída.
- Ex: scaleX.domain([100, 500]).range([10, 350]);.
- **Escalas Lineares:** d3.scaleLinear()
- **Escalas de Potência:** d3.scalePow().exponent(3)
- **Escalas Ordinais:** d3.scaleOrdinal()
- Exemplos de mapeamento: contínuo para contínuo, contínuo para discreto, discreto para discreto.
- Uso de d3.schemeCategory10 para esquemas de cores.

**7. Princípios de Visualização (4_VI_principles.pdf)**

- **Fator de Mentira (Lie Factor):** Mede a distorção entre o efeito visual e o efeito nos dados.
- Fator igual a 1 indica representação precisa.
- Maior que 1.05: sobrestima o efeito.
- Menor que 0.95: subestima o efeito.
- O foco não é apenas nos efeitos mostrados, mas como eles são percebidos.
- **Junk Útil:** Gráficos com elementos decorativos podem melhorar a memorização e o valor percebido.
- Estudos mostraram melhor recordação em gráficos com elementos visuais atraentes.
- Os participantes acharam esses gráficos mais fáceis de lembrar, mais atrativos e mais prazerosos.

**8. Formas (Paths) em D3.js (5_VI_demo_path.pdf)**

- **Bibliotecas de Visualização:**D3.js (grafos, redes, mapas)
- Chart.js (gráficos)
- ApexCharts (gráficos)
- ECharts (gráficos)
- Plotly (Python/R, gráficos, mapas)
- **Paths:**Construção de formas com d3.line().
- .x(d => scaleX(d.x_value)) e .y(d => scaleY(d.y_value)) para definir as coordenadas.
- Uso de .datum(data) para associar dados a um path.
- Uso de .attr('d', line) para desenhar o path.

**9. Semiologia Gráfica (5_VI_semiology.pdf)**

- **Semiologia:** Estudo dos sinais e culturas que os usam.
- Um sinal representa algo diferente de si próprio (mapeamento entre dados e visualização).
- Diferentes pessoas interpretam sinais de formas distintas.
- **Jacques Bertin:** Teórico e cartógrafo francês, autor de "Semiologie Graphique" (1967).
- Propôs uma base teórica para o uso de elementos gráficos.
- As dimensões visuais têm propriedades relacionadas com o número de instâncias e o tipo de dimensão.
- O modo como valores de dados são mapeados em estruturas visuais.
- **Codificação Visual:**Mapeamento de dados em marcas visuais e de atributos de dados em canais visuais.
- **Marcas (Marks):Ponto:** Zero-dimensional (0D), representa um local sem comprimento.
- **Linha:** Uma-dimensional (1D), conexão entre dois pontos com comprimento.
- **Área:** Duas-dimensional (2D), tamanho mensurável no plano.
- **Relações entre Marcas:** Similaridade, ordem e proporção.
- **Construções Polares:** Versão circular de elevações retilineares, onde a quantidade é representada por áreas.
- **Canais Visuais (Visual Variables):** Propriedades dos símbolos que controlam a sua aparência.
- São processados pré-atentivamente, i.e., "vistos" perceptualmente e não "entendidos" cognitivamente.
- **Tamanho:** Dissociativo
- **Valor:** Brilho, dissociativo.
- **Textura:** Associativo
- **Cor:** Associativo
- **Orientação:** Associativo
- **Forma:** Associativo
- **Canais de Identidade:** O que ou onde algo está.
- **Canais de Magnitude:** Quanto de algo existe.
- **Níveis de Organização:Qualitativo:** Associativo e seletivo
- **Ordenado:**
- **Quantitativo:**
- **Propriedades Perceptuais:Associativo (≣):** Permite diferenciar elementos em grupos (e.g., mamíferos vs peixes).
- **Seletivo (≠):** Permite selecionar um elemento de um grupo (e.g., diferenciar peixes).
- **Ordenado (O):** Mudanças percebidas como ordenadas.
- **Quantitativo (Q):** Leitura numérica obtida das mudanças.
- **Discriminabilidade:** Número de "bins" disponíveis em cada canal.
- O número de "bins" deve corresponder ao número de "bins" do atributo codificado.
- **Separabilidade:Canais Separables:** Possível analisar individualmente.
- **Canais Integrais:** Dois canais vistos de forma holística.
- **Perceção Visual:Estágio 1:** Processamento paralelo, rápido e pré-atentivo.
- **Estágio 2:** Processamento de padrões em memória.
- **Estágio 3:** Processamento sequencial e orientado a objetivos.
- **Leis de Gestalt:Proximidade:** Grupar elementos próximos.
- **Semelhança:** Grupar elementos similares.
- **Conexão:** Grupar elementos conectados.
- **Continuidade:** Elementos alinhados são vistos como pertencentes ao mesmo grupo.
- **Fechamento:** Tendência a fechar contornos e ver contornos fechados como objetos.
- **Figura e Fundo:** Identificar alguns elementos como figura e o resto como fundo.
- **Perceção Relativa:** Steven's law – tendência a subestimar ou superestimar certos atributos visuais.

**10. Tarefas e Interação (6_VI_tasks_interaction.pdf)**

- **Tarefas de Visualização:Encontrar Extremos:** Identificar valores máximos e mínimos.
- Ex: "Qual é a montanha mais alta do mundo?"
- **Ordenar:** Classificar dados por uma métrica ordinal.
- Ex: "Ordenar os carros por peso."
- **Encontrar Intervalo:** Determinar a extensão de valores de um atributo.
- **Clustering (Agrupamento):**Agrupar dados semelhantes.
- Aplicações em marketing, biologia, bibliotecas, seguros, etc.
- **Tipos de Clustering:Hierárquico:Aglomerativo:** Começa com cada elemento num _cluster_ e junta-os.
- **Divisivo:** Começa com todos os elementos num _cluster_ e divide-o.
- **Particional:** Divide os dados diretamente em _clusters_.
- **K-means:** Algoritmo popular de _clustering_ particional.
- **Fuzzy c-means:** Permite membros em múltiplos _clusters_.
- **Medidas de Similaridade/Distância:Euclidiana:** Distância em linha reta.
- **Manhattan:** Soma das diferenças absolutas nas coordenadas.
- **Hamming:** Número de valores diferentes (usado em deteção de erros).
- **Clustering Hierárquico Aglomerativo:**Começa com cada item num _cluster_, junta os mais próximos, e repete até que todos estejam num único _cluster_.
- **Linkage (Medidas de distância entre clusters):Single linkage:** Menor distância entre _clusters_.
- **Complete linkage:** Maior distância entre _clusters_.
- **Average linkage:** Distância média entre _clusters_.
- **Ward's linkage:** Minimiza a variância total dentro do _cluster_.
- **Dendrograma:** Representação visual dos _clusters_ hierárquicos.
- **Clustering Particional Baseado em Centróides (K-Means):**Centróides representam os _clusters_.
- Iterações de atribuição de objetos aos _clusters_ mais próximos e recálculo dos centróides.
- **Clustering Particional Baseado em Densidade (DBSCAN):**_Clusters_ são áreas de maior densidade.
- Pontos esparsos são considerados ruído.
- **Core points:** pontos com um número mínimo de vizinhos dentro de um raio.
- Pontos alcançáveis: formam um _cluster_.
- Pontos não alcançáveis: considerados _outliers_.
- O algoritmo DBSCAN é apresentado em pseudocódigo.

**11. Estruturas Tabulares (7_VI_tabular.pdf)**

- **Uso do Canal Espacial:** Canais X e Y (variáveis planares) para representar dados.
- É um dos canais visuais mais eficazes.
- O _layout_ define uma imagem mental dos dados.
- **Diagramas (Bertin):** Ligação entre todas as divisões de uma dimensão e as de outra.
- **Expressar Valores:**Atributos quantitativos mapeados para posições espaciais.
- Marcas: pontos, linhas, áreas ou "glyphs".
- **Scatterplot:**Duas variáveis quantitativas em X e Y.
- Usa pontos como marcas.
- Cores e tamanhos para atributos adicionais.
- Usado para tendências, _outliers_, distribuições, correlações, _clusters_.
- **Data Glyphs:** Entidades visuais para representar dados multivariados.
- Exemplo: Chernoff faces.
- Três classes de mapeamento de dados para atributos visuais.
- **Separação, Ordenação e Alinhamento:** Uso de regiões espaciais contíguas para apresentar itens com o mesmo valor.
- **Orientação de Eixos:Retilínea:** Distribuição ao longo de dois eixos perpendiculares.
- **Paralela:** Eixos paralelos entre si.
- **Radial:** Itens dispostos em torno de um círculo.
- **Layout Denso:** Marcas pequenas e densamente compactadas para obter uma visão geral com alta densidade de informação.
- Ex: SandDance (framework JavaScript da Microsoft).
- **Circos:** _Software_ para visualizações circulares com alta taxa de dados por tinta (data-to-ink).

**12. Geovisualização (8_VI_geo.pdf)**

- **Mapas:** Representações gráficas do meio.
- **Cartografia:** Arte, ciência e tecnologia de fazer mapas.
- **Projeções:**Robinson projection: cada ponto tem algum nível de distorção.
- **Tipos de Dados:Pontuais:** Dados associados a locais únicos.
- **Lineares:** Dados de fluxos e movimentos.
- **De Área:** Dados de densidades, precipitação, qualidade do ar, etc.
- **Dados Espaciais:Nominal:** Responde à questão do que é representado.
- **Ordinal:** Dados com uma ordem (e.g., nível de perigo).
- **Quantitativos:** Dados numéricos
- **Discretos:** Dados associados a um local específico.
- **Contínuos:** Dados de forma contínua (e.g., temperatura em um país).
- **Atributos:Total:** Dados medidos em localizações específicas.
- **Derivados:** Dados calculados (e.g., pessoas por km2).
- **Mapas Temáticos:** Permitem entender o "onde", "o que" e "quando" dos dados espaciais.
- **Choropleth map:** Representação de dados quantitativos por área.
- Importante considerar a perceção relativa versus absoluta (Steven’s Law).
- Uso de esquemas de cores contínuos (sequencial, divergente, cíclico) ou discretos.
- **Dot map, Proportional/Graduated Symbol maps, Isarithmic and Isopleth maps, Flow/Network maps, Area and Distance cartograms, Schematic/Transit maps, Typographic maps.**

**13. Séries Temporais (9_VI_time_series.pdf)**

- **Modelagem do Tempo:Escala:** Tipos de escala temporal (ordinal, intervalos).
- **Âmbito:** Período temporal a ser analisado.
- **Disposição (Arrangement):** Forma como o tempo é organizado (linear, cíclico, ordenado, ramificado).
- **Ponto de Vista:** Perspetiva temporal (múltiplas perspetivas).
- **Disposição do Tempo:Linear:** Tempo decorre linearmente do passado para o futuro.
- **Cíclico:** Domínio composto por um conjunto de valores que se repetem (e.g., estações do ano).
- **Ordenado:** Pontos no tempo ocorrem um após o outro.
- **Ramificado (Branching):** Múltiplas linhas do tempo que divergem.
- **Múltiplas Perspetivas:** Mostrar múltiplos pontos de vista sobre o tempo.
- **Abstrações Temporais:Granularidades:** Abstrações no tempo (e.g., milissegundos, horas, dias).
- **Primitivas Temporais:Instant:** Ponto no tempo.
- **Intervalo:** Duração entre dois pontos.
- **Relações:** Relações entre instantes e intervalos.
- **Determinância:** Conhecimento completo ou incompleto sobre um ponto no tempo.
- **Dados Orientados ao Tempo:Escala:** Escala temporal dos dados.
- **Frame of Reference (Quadro de Referência):** O referencial temporal.
- **Tipo de Dados:** Contínuos ou discretos.
- **Número de Variáveis:** Univariados ou multivariados.
- **Análise Temporal:Tarefas de baixo nível:**Existência de um elemento de dados num tempo específico.
- **Tarefas de alto nível.**
- **Apresentação Visual:Coordenadas cartesianas:** Eixos X (tempo) e Y (dados).
- **Pequenos Múltiplos (Small-Multiples):** Várias visualizações lado a lado para diferentes granularidades ou variáveis.
- **Coordenadas Polares:** Tempo disposto circularmente.
- **Tamanho e Comprimento:** Marcas visuais com variação de tamanho e comprimento.
- **Matrizes:** Valores de dados codificados com brilho.
- **Layout Hierárquico:** Várias granularidades representadas em diferentes níveis.
- **GROOVE:** Modelo para dividir dados em quatro granularidades.

**14. Redes e Grafos (10_VI_trees.pdf)**

- **Tipos de Redes:** A mais comum é a "bipartite" (e.g., leitores e livros).
- **Elementos:Nós (Nodes):** Representam as entidades da rede.
- **Arestas (Edges):** Representam as ligações ou interações entre nós. Podem ser:
- **Direcionadas:** Indicam a direção da interação.
- **Não Direcionadas:** Não indicam direção.
- **Ponderadas:** Expressam a força ou importância da conexão.
- **Tipos de Dados:** Nominal, ordinal, ou quantitativo.
- **Propriedades:Grau (Degree):** Número de conexões de um nó.
- **In-degree:** Número de conexões que chegam ao nó.
- **Out-degree:** Número de conexões que saem do nó.
- **Centralidade:** Medida da importância de um nó na rede. Ex: "Quantas conexões diretas tem uma pessoa?"