## Questionário (Respostas Curtas)

1. Descreva a diferença entre visualização científica (SciVis) e visualização de informação (InfoVis).
2. O que significa dizer que um grafo é "bipartido"? Dê um exemplo.
3. Explique como um _Lie Factor_ pode afetar a perceção de dados em um gráfico.
4. O que é um _tag cloud_ e qual a sua utilidade na visualização de informação?
5. Diferencie entre variáveis categóricas (nominais e ordinais) e variáveis quantitativas (discretas e contínuas).
6. Defina o conceito de "escala de intervalo" em relação aos níveis de medição.
7. Explique como funciona a técnica de _binning_ (discretização) de dados.
8. Descreva a função dos canais visuais em termos de codificação de dados, citando pelo menos três exemplos.
9. O que são os princípios de _Gestalt_ e como eles influenciam a perceção visual?
10. Explique o que é o algoritmo DBSCAN na análise de _clustering_.

## Chave de Respostas

1. SciVis lida com dados geométricos (volumétricos) em espaço 3D, enquanto InfoVis lida com dados abstratos, com foco em estética e design. SciVis trata de problemas em 3D, GeoVis com fenômenos geográficos e InfoVis com dados abstratos.
2. Um grafo bipartido é aquele em que os nós podem ser divididos em dois grupos, com as arestas ligando apenas nós de grupos diferentes. Um exemplo é a relação entre leitores e livros.
3. O _Lie Factor_ é a razão entre o tamanho do efeito mostrado num gráfico e o tamanho do efeito nos dados. Um valor acima de 1.05 indica uma sobrevalorização, e abaixo de 0.95, uma subvalorização, afetando a perceção da informação.
4. Um _tag cloud_ (nuvem de palavras) é uma representação visual das palavras mais usadas num texto, em que o tamanho de cada palavra é proporcional à sua frequência. É utilizado para resumir e destacar os temas principais de um documento.
5. Variáveis categóricas (nominais) representam categorias sem ordem, como cores ou tipos, enquanto variáveis ordinais têm uma ordem, como níveis de educação. As variáveis quantitativas (discretas) são contagens (número de filhos) e as contínuas podem assumir qualquer valor num intervalo (peso, altura).
6. Uma escala de intervalo é aquela em que se pode calcular distâncias entre valores, mas não existe um zero verdadeiro (ex: temperatura em Celsius/Fahrenheit, pontuação de IQ). Não se pode dizer que uma temperatura de 40 graus é "o dobro" de 20.
7. O _binning_ (discretização) é o processo de conversão de dados contínuos em dados discretos, agrupando os valores em intervalos predefinidos. Ex: Agrupar pesos em faixas de peso: <40, 40-50, 50-60, >60
8. Os canais visuais são propriedades de marcas visuais (cor, tamanho, forma, posição) usados para codificar dados. Por exemplo, cor para categorias, tamanho para quantidades e posição para relações espaciais.
9. Os princípios de _Gestalt_ são leis da perceção visual que descrevem como agrupamos elementos visuais em padrões significativos (e.g. proximidade, semelhança, continuidade, fechamento e simetria).
10. DBSCAN é um algoritmo de _clustering_ que agrupa pontos densamente aglomerados, marcando _outliers_ que estão em regiões de baixa densidade. Identifica clusters com base na densidade de pontos ao invés de distâncias.

---
## Questionário

Responda às seguintes perguntas com 2-3 frases concisas.

1. O que é a visualização de informação e qual o seu principal objetivo?
2. Explique o conceito de "Ink Ratio" de Edward Tufte e por que é importante.
3. Defina o que são "variáveis visuais" e dê três exemplos de variáveis.
4. O que são "implantações" (ou "marcas") em visualização de informação? Dê exemplos.
5. Descreva as propriedades percetuais de uma variável visual (Quantitativo, Ordenado, Associativo e Seletivo).
6. Quais são os 5 passos do processo de visualização, desde a definição do problema até a validação?
7. Diferencie os dados categóricos, nominais e ordinais dos dados quantitativos discretos e contínuos.
8. Explique quando utilizar a média e quando utilizar a mediana como medidas de tendência central.
9. Descreva a diferença entre um histograma e um dot plot e em que situações são mais apropriados.
10. Explique a importância da pré-processamento de dados e quais os passos incluídos nesse processo.

## Chave de Respostas

1. A visualização de informação é a representação gráfica de dados, com o objetivo de tornar conjuntos de dados complexos mais acessíveis, expandindo o nosso conhecimento e permitindo a sua análise e exploração. Através da codificação visual das variáveis, representam-se as relações entre elas.
2. "Ink Ratio" refere-se à maximização da quantidade de informação útil numa visualização, minimizando o uso de píxeis que não acrescentam informação. É importante porque a visualização deve ser o mais eficiente possível, mostrando o máximo de dados relevantes.
3. Variáveis visuais são os atributos que usamos para codificar dados visualmente, como posição X e Y, tamanho, forma, cor, valor, orientação e textura. Elas mapeiam os dados em elementos visuais, facilitando a perceção.
4. Implantações ou marcas são os elementos gráficos que usamos para representar os dados, como pontos, linhas e áreas. São as formas físicas com as quais as variáveis visuais são implementadas.
5. Uma variável é quantitativa se a mudança na variável permitir uma leitura numérica; é ordenada se os valores mostram uma ordem; é associativa se permite agrupar elementos distintos e seletiva se permite diferenciar elementos dentro de um grupo.
6. Os 5 passos do processo de visualização são: 1) definição do domínio do problema e target user; 2) tradução dos dados em abstrações (Data Abstraction e Task Abstraction); 3) design visual (codificações e interações); 4) implementação e 5) validação do processo.
7. Dados categóricos incluem nominais, como categorias não ordenadas (ex: bicicleta ou carro) e ordinais, que apresentam uma ordem ou sequência (ex: notas insuficientes a excelente). Dados quantitativos são números, onde discretos são valores fixos e contínuos podem assumir qualquer valor num intervalo.
8. A média é usada quando os dados têm uma distribuição normal e os valores extremos não influenciam os resultados. A mediana é preferida quando a distribuição dos dados é assimétrica ou quando existem valores extremos que podem distorcer a média.
9. Um histograma agrupa os dados em classes, mostrando a frequência de cada intervalo, enquanto um dot plot apresenta cada valor individualmente como um ponto. O histograma é melhor para distribuições em grande escala, enquanto o dot plot é útil para valores individuais ou grupos pequenos.
10. O pré-processamento de dados é crucial para garantir a qualidade e a adequação dos dados para visualização. Inclui passos como recolher, selecionar, descobrir, categorizar, limpar, validar e transformar dados para compatibilizar com representações visuais.
