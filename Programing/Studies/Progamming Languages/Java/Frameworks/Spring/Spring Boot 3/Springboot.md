
### Conceito

Enquanto que o Spring Framework é baseado no padrão de injeção de dependências, o Springboot foca na configuração automática.

### Antes  do Springboot

Desafios com a configuração do projeto.
- Dependência individual.
- Verbosidade.
- Incompatibilidade de versões.
- Complexidade de gestão.
- Configurações complexas e repetitivas.

### Starters

Descritores de dependências

![[Pasted image 20240223033551.png]]


### Alguns Starters

Listagem de alguns starters mais utilizados

Spring-boot-starter-*
- data-jpa: Integração ao banco de dados via JPA - Hibernate.
- data-mongodb: Interação com banco de dados MongoDB.
- web: Inclusão do container  Tomcat para aplicações REST.
- web-services: Webservices baseados na arquitetura SOAP.
- batch: Implementação de JOBs de processos.
- test: Disponibilização de recursos para testes unitários como JUnit.
- openfeign: Client HTTP baseado em interfaces.
- actuator: Gerenciamento de monitoramento da aplicação.


### Beans vs Components

### Scopes - Singleton e Prototype

### Properties Value

### Configuration Properties

### ORM (Object-Relational Mapping)

Object-Relational Mapping, Em português, mapeamento objeto-relacional, é um recurso para aproximar o paradigma da orientação a objetos ao contexto de banco de dados relacional.

O uso de ORM é realizado através do mapeamento de objeto para uma tabela por uma biblioteca ou Framework.

![[Pasted image 20240223234311.png]]

### JPA (Java Persistence Aplication)

JPA é uma especificação baseado em interfaces, que através de um framework realiza operações de persistência de objetos em Java.


![[Pasted image 20240223234806.png]]


### Mapeamento do JPA

Vamos conhecer os aspectos das anotações de mapeamento do JPA:

- Identificação
- Definição
- Relacionamento
- Herança
- Persistência


```Java
import javax.persistence.Column;
import javax.persistence.Entity;
import javax.persistence.GeneratedValue;
import javax.persistence.GenerationType;
import javax.persistence.Id;
import javax.persistence.Table;

@Entity
@Table(name="user_tb")
public class Usuario{

	@Id
	@GeneratedValue(strategy=GenerationType.AUTO)
	@Column(name="user_id")
	private Long id;

	private String name;

	@Column(name="user_login")
	private String login;

	@Column(name="user_password")
	private String password;
}
```

![[Pasted image 20240224000000.png]]
