
### Pré-requisitos

- JDK instalado
- IDE escolhida
- Diretório do projeto definido


#### Anatomia da Classe

- Estrutura inicial
- Padrão de nomenclatura
- Declarando variáveis e métodos
- Indentação
- Organizando arquivos
- Java Beans

*Uma classe bem estruturada não quer guerra com ninguém - Mano Deyvin*

A escrita de código de um programa é feito através da composição de palavras pré-definidas pela linguagem com as expressões que utilizamos para determinar o nome do nosso arquivo, classes, atributos e métodos.

É muito comum mesclarmos expressões no idioma americano com o nosso vocabulário. Existem projetos que recomendam que toda a implementação do seu programa seja escrita na língua inglesa.

```java
public class MyClass {
	// OUR CODE HERE
}
```

### Padrão de nomenclatura

Quando se trata de escrever código na linguagem Java, é recomendado seguir algumas convenções de escrita. Esses padrões estão expressos nos itens abaixo:

- **Arquivo .java**: Todo arquivo .java deve começar com letra Maiúscula. Se a palavra for composta, a segunda palavra deve também ser maiúscula, exemplo:
	- Calculadora.java, CalculadoraCientifica.java
- Nome da classe no arquivo: A classe deve possuir o mesmo nome do arquivo.java, exemplo:

```java
// arquivo CalculadoraCientifica.java

public class CalculadoraCientifica {

}
```

- Nome de variável: toda variável deve ser escrita com letra minúscula, porém se a palavra for composta, a primeira letra da segunda palavra deverá ser maiúscula, exemplo: ano e anoFrabricacao . O nome dessa prática para nomear variáveis dessa forma se chama "camelCase".

> Existe uma regra adicional para variáveis quando na mesma queremos identificar que ela não sofrerá alteração de valor, exemplo: quer emos determinar que uma variável de nome **br** sempre representará "Brasil" e nunca mudará seu valor, logo, determinamos como escrita o código abaixo:

```java
public class Paises {

	
	int ano = 2024;
	// Correct
	ano = 2025;

	
	final String BR = "Brasil"
	// Wrong
	BR = "Brazil"
}
```

> Recomendações: Para declarar uma variável nós podemos utilizar caracteres, números e símbolos, porém devemos seguir algumas regras da linguagem.

- Deve conter apenas letras, __ (underline), $ ou números de 0 a 9
- Deve obrigatoriamente se iniciar por uma letra (preferencialmente), __ ou $, jamais com número
- Deve iniciar com uma letra minúscula (boa prática - ver abaixo)
- Não pode conter espaços.
- Não podemos usar palavras-chave da linguagem
- O nome deve ser único dentro de um escopo

### Declarando variáveis e métodos

Declarar uma variável em Java segue sempre a seguinte estrutura:

> Tipo NomeBemDefinido = Atribuição (opcional em alguns casos)

``` Java
public class CalculadoraCientifica {
	int fabricationYear = 2020;
	String model = "Brastemp";
	boolean itsWorking = True;
	NetworkConnection wifi;
}
```

### Variáveis

Uma variável é uma área de memória, associada a um  nome, que pode armazenar valores de um determinado tipo. Um tipo de dado define  um conjunto de valores e um conjunto de operações. Java é uma linguagem com rigidez de tipos, diferente de linguagens como JavaScript, onde declarar o tipo da variável não é obrigatório.

No Java utilizamos identificadores que representam uma referência (ponteiro) a um valor em memória, e esta referência pode ser redirecionada a outro valor, sendo portanto esta a causa do nome "variável", pois o valor pode variar.

```java
public class SampleVariables {
	public static void main(String[] args) {
	
		byte age = 123;
		short year = 2024;
		int cep = 21070333;
		long cpf = 98765432109L;
		float pi = 3.14F;
		double salary = 1275.33;
		String user = "Duke";
		char option = 'b';
		
		System.out.println("Hello World and Cooffe");
	
	}
}
```

Já as **Constantes** são valores armazenados em memória que não podem ser modificados depois de declarados. Em Java, esses valores são representados pela palavra reservada **final**, seguida do tipo.

Por convenção, Constantes são sempre escritas em **CAIXA ALTA**.

``` Java
public class SampleConstVariables {
	public static void main(String[] args) {
	
		final float PI_VALUE = 3.14F;
		
		System.out.println(PI);
	
	}
}
```


#### Operadores

- Operadores aritméticos
- Operadores unários
- Operadores relacionais
- Operadores lógicos
- Operador ternário

Os outros eu já sei, vou colocar só o ternário.

##### Ternário

O operador de condição ternária é uma forma resumida para definir uma condição e escolher por um dentre dois valores. Você deve pensar numa condição ternária como se fosse uma condição IF normal, porém, de uma forma em que toda a sua estrutura estará escrita numa única linha.

O operador ternário é representado pelos símbolos **?:** utilizados na seguinte estrutura de sintaxe:

> <Expressão Condicional> ? <Caso condição seja true> : <Caso Condição seja false>


``` Java
public class SampleTernaryOperation {
	public static void main(String[] args) {
	
		final int A = 3;
		int b = 10;
		boolean result;

		result = A==b ? true : false;
		
		System.out.println(result);
	
	}
}
```


#### Critério de nomeação de Métodos

- Deve ser nomeado como verbo.
- Seguir o padrão camelCase.

> ATENÇÂO! Não existe em Java o conceito de métodos globais. Todos os métodos devem sempre serem definidos dentro de uma classe.


``` Java
public class MathOperations {
	public static void main(String[] args) {
	
		final int A = 3;
		int b = 10;
		boolean result;

		result = A==b ? true : false;
		
		System.out.println(result);
	
	}

	public double sum(int num1, int num2){
		return num1 + num2;
	}

	public void print(String text){
		System.out.println(text);
	}

	public double divide(int divider, int dividend) throws Exception {
        try {
            if (divider == 0) {
                throw new ArithmeticException("Divisão por zero não é permitida.");
            }
            
            return (double) dividend / divider;
        } catch (ArithmeticException e) {
            throw new Exception("Erro ao dividir: " + e.getMessage());
        }
    }
}
```


#### Palavras reservadas

Objetivo: Apresentar as 52 palavras reservadas organizadas por classificação de usabilidade considerando as regras da linguagem.

- Tipos Primitivos
- Classificações
- Escopo de uso
- Palavras "opostas"

Palavras reservadas são identificadores de uma linguagem que já possuem uma finalidade específicas, portanto não podem ser utilizados para nomear variáveis, classes, métodos ou atributos.

##### **Controle de pacotes**

import: importa pacotes ou classes para dentro do código.

package: especifica a que pacote todas as classes de um arquivo pertencem

#### Modificadores de acesso

public: acesso de qualquer classe

private: acesso apenas dentro da classe

protected: acesso por classes no mesmo pacote e subclasses

#### Primitivos 

boolean: um valor indicando verdadeiro ou falso

byte: um inteiro de 8 bits (signed)

char: um character unicode (16-bit unsigned)

double: um número de ponto flutuante de 64 bits (signed)

float: um número de ponto flutuante de 32 bits (signed)

int: um inteiro de 32 bits (signed)

long: um inteiro de 64 bits (signed)

short: um inteiro de 32 bits (signed)

void: indica que o método não tem retorno de valor

#### Modificadores de classes, variáveis ou métodos

**abstract**: classe que não pode ser instanciada ou método que precisa ser implementado por uma subclasse não abstrata.

**class**: especifica uma classe

**extends**: indica a superclasse que a subclasse está estendendo

**final**: impossibilita que uma classe seja estendida, que um método seja sobrescrito ou que uma variável seja reinicializada.

**implements**: indica as interfaces que uma classe irá implementar

**native**: indica que um método está escrito em uma linguagem dependente da plataforma, como o C

**new**: instancia um novo objeto, chamando seu construtor

**static**: faz um método ou variável pertencer à classe ao invés de às instâncias

strictfp: estranho, ovo ignorar :)

**synchonized**: indica que um método só pode ser acessado por uma thread de cada vez

**transient**: impede a serialização de campos

#### Controle de fluxo dentro de um bloco de código

break: sai do bloco de código em que ele está

case: executa um bloco de código dependendo do teste do switch

continue: pula a execução do código que viria após essa linha e vai para próxima passagem do loop.


### Terminal e Argumentos (Entradas e Saída de dados)





### Documentação Java

[Link da documentação oficial do Java SE 21](https://docs.oracle.com/en/java/javase/21/docs/api/index.html)


