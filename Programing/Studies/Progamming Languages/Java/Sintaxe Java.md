
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

### Organizando arquivos

