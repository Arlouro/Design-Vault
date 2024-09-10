#COMP 
## Statlist: 
0 nós filhos não adiciona nada
1 nó filhos adiciona apenas o nó filho e salta o nó StatList
2 ou mais nós filhos adiciona normalmente ou seja o nó StatList e os seus filhos

## Declaration:
No caso de ``int a, b;`` tem que aparecer: 
```
Declaration
..int
..a
Declaration
..int
..b
```
Mas cada declaration é lida no seu nó da árvore por isso há uma variável global para guardar o tipo da declaration que depois é usada.

## Precedência do PLUS:
Para o PLUS e o MINUS ex -1, +2 é usada a mesma precedência do que o NOT ou seja a precedência mais alta.

## Contagem das linhas:
Há *4 contadores* todos eles presentes no  `YY_USER_ACTION` no `uccompiller.l`
- a variável ``line`` e ``column`` para o lexer
- a variável ``line_start`` e ``column_start`` para os comments do lexer
- a variável ``line_syn`` e ``column_syn`` para a análise sintática
- o `yylocc` para passar as localizações para o yacc onde depois elas são guardadas nos nodes para usar na meta 3

## Brothers:
We created a list of children and then added them to the father node

## Return type:
O tipo de retorno de uma função é literalmente a primeira linha da tabela local dessa determinada função

## Raiz a null statement semi:
Há casos em que no statement aparece ``$$ = NULL``  por isso é que há no código ex ``if($3) bla bla bla`` para não tentar adicionar nos inválidos aka `NULL`