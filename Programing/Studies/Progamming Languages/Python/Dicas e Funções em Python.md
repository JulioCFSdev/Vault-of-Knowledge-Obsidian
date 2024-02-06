
- ord() - retorna um numero inteiro representação a posição do elemento na tabela ASCII.
- list() - transforma um elemento em uma lista de elementos
- chr() - inverso do chr(), retorna o elemento  corresponde a posição da tabela ASCII.
- list.reverse() - Não retorna nd, mas inverte a lista;
- abs(x) - retorna o valor absoluto de x;
- int(x) - da pra usar pra pegar apenas o inteiro do valor float e. g. 3.5 para 3;
- usar um for x,y in enumerate(list) consegue fazer um loop que fornece o conteúdo da lista sendo y e a posição desse conteúdo sendo X;
- Conseguimos concatenar todos os elementos de uma lista em uma string só usando  ''.join(list);
- Try except é o Try catch é bom usar pra ser uma quebra de while para pegar todos os dados de um arquivo até acabar. 
 ```python
	while is_inputing:
        try:
            current_input = str(input())
        except EOFError as e:
            break
 ```