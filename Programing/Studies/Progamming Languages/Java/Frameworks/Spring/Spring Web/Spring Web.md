
### Rest Controller

Um **Rest controller** em Spring nada mais é que uma classe contendo anotações específicas para a disponibilização de recursos HTTPs baseados em nossos serviços e regras de negócio.

Anotações e configurações mais comuns:

- **@RestController:** Responsável por designar o bean de component que suporta requisições HTTP com base na arquitetura REST.
- **@RequestMapping("prefix"):** Determina qual a URI comum para todos os recursos disponibilizados pelo **Controller**.
- **@GetMapping:** Determina que o método aceitará requisições **HTTP** do tipo **GET**.
- **@PostMapping**: Determina que o  método aceitará requisições **HTTP** do tipo **POST**.
- **@PutMapping:** Determina que o método aceitará requisições **HTTP** do tipo **PUT**.
- **@DeleteMapping:** Determina que o método aceitará requisições **HTTP** do tipo **DELETE**.
- **@RequestBody:** Converte um JSON para o tipo do objeto esperado como parâmetro no método.
- **@PathVariable:** Consegue determinar que parte da URI será composta por parâmetros recebidos nas requisições.