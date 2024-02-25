
O Spring Data JPA adiciona uma camada sobre o JPA.  Isso significa que ele usa todos os recursos definidos pela especificação JPA, especialmente os mapeamentos de entidade e os recursos de persistência baseado em interfaces e anotações. Por isso, o Spring Data JPA adiciona seus próprios recursos, como uma implementação sem código do padrão de repositório e a criação de consultas de banco de dados a partir de nomes de métodos.

![[Pasted image 20240224000852.png]]

A partir de agora nossa interação com o banco de dados será através de herança de interfaces e declaração de métodos com anotações.

**Interfaces:**
- CrudRepository
- JPARepository
- PagingAndSortingRepository

**Anotações:**
- @Query
- @Param

