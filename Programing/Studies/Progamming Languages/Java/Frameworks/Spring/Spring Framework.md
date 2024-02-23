
### Fundamentos

- O que é Spring Framework
- Spring Versus Java EE
- Conceito de Inversão de Controle
- Injeção de Dependências
- Beans \\ Autowired \\ Scopes


### Conceito

Framework open source desenvolvido para a plataforma Java baseado nos padrões de projetos inversão de controle e injeção de dependência.

Sua estrutura é composta por módulos afins de reduzir a complexidade no desenvolvimento de aplicações simples ou corporativas.

![[Pasted image 20240223030250.png]]

### Spring versus Java EE

![[Pasted image 20240223030514.png]]


### Inversão de Controle

Inversion of Control ou IoC, trata-se do redirecionamento do fluxo de execução de um código retirando parcialmente o controle sobre ele e delegando-o para  um container.
O principal propósito é minimizar o acoplamento do código.


![[Pasted image 20240223030942.png]]


![[Pasted image 20240223031112.png]]

### Injeção de Dependências

Injeção de dependência é um padrão de desenvolvimento com a finalidade de manter o baixo o nível de acoplamento entre módulos de um sistema.

![[Pasted image 20240223031300.png]]

### Beans

Objeto que é instanciado (criado), montado e gerenciado por um contêiner através do princípio da inversão de controle.

![[Pasted image 20240223031518.png]]

### Singleton

O contêiner do Spring IoC define apenas uma instância do objeto.


### Prototype

Será criado um novo objeto a cada solicitação ao contêiner.


### HTTP-Request

Um bean será criado para cada requisição HTTP. Os objetos existirão enquanto a requisição estiver em execução.

### HTTP-Session

Um bean será criado para a sessão de usuário. Precisamos acessar a mesma solicitação duas vezes para testar os escopos específicos da web.

### HTTP-Global

Ou Aplication Scope cria um bean para o ciclo de vida do contexto da aplicação. Objetos compartilhados por toda a aplicação.


### Autowired

Uma anotação (indicação) onde deverá ocorrer uma injeção automática  de dependências.

- byName: É buscado um método set que corresponde ao nome do Bean.
- byType: É considerado o tipo da classe para inclusão do Bean.
- byConstrutor: Usamos o construtor para incluir a dependência.