
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
 - Posso acessar os elementos de uma string, usando a posição dele como se fosse uma lista.
 ```python
	phrase = 'Tpo oCder'
	print(phrase[0])
    # T
 ```

- Formar eficientes de Entrelaçar 2 listas de tamanhos diferentes
	- 1º Forma: Usando o operador + para concatenar 2 strings
 ```python
	string_splited = ['Tpo', 'oCder']
	new_phrase = ''
	max_string = max(string_splited)
	for index in range(len(max_string)):
	    if index < len(string_splited[0]):
	        new_phrase = new_phrase + string_splited[0][index]
        if index < len(string_splited[1]):
            new_phrase = new_phrase + string_splited[1][index]
    print(new_phrase)
    # TopCoder
```
- 2º Forma: Usar o método Join() com o operador Spread *
 ```python
	string_splited = ['Tpo', 'oCder']
	new_phrase = ''
	max_string = max(string_splited)
	for index in range(len(max_string)):
	    if index < len(string_splited[0]):
	        new_phrase = "".join([*new_phrase, string_splited[0][index]])
	    if index < len(string_splited[1]):
	        new_phrase = "".join([*new_phrase, string_splited[1][index]])
	
	print(new_phrase)
    # TopCoder
```

Existem um método de string/lista que retornar a substring inicial ou final de uma string:

```python
	string = '1234 34'
	numbers = input().split(" ")

    if numbers[0].endswith(numbers[1]):
        print("encaixa")
    else:
        print("nao encaixa")
    # encaixa
```