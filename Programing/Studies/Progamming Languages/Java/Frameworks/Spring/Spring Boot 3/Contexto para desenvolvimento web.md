
## Objetivo  Geral

Para o desenvolvimento de uma aplicação web,  é importante utilizar ferramentas modernas e confiáveis para garantir a qualidade, desempenho e segurança de um software.

![[Pasted image 20240222204242.png]]
## Pré-requisitos

- IDE para desenvolvimento Kotlin (IntelliJ Community)
- JDK 17+
- Kotlin 1.7.22
- Sintaxe básica Kotlin
- Conhecimento acerca de POO

## Entendendo a Arquitetura Rest

###  O que é API?

- API significa **Aplication Programming Interface**
- No contexto de APIs,a palavra **Aplicação** refere-se a qualquuuer software com uma função distinta.
- A **Interface** pode ser pensada como um contrato de serviço entre duas aplicações.
- Esse contrato define como as duas se comunicam usando solicitações e respostas.
- A documentação de suas respectivas APIs contém informações sobre como os desenvolvedores devem estruturar essas solicitações e respostas.

### Como as APIs funcionam?

- A arquitetura da API geralmente é explicada em termos de cliente e servidor.
- A aplicação que envia a solicitação é chamada de cliente e a aplicação que envia a resposta é chamada servidor.

![[Pasted image 20240222210320.png]]

### Tipos de APIs

- **APIs  SOAP:** Cliente e servidor trocam mensagens usando XML. Esta é uma API menos flexível que era mais popular.
- **APIs RPC:** O cliente conclui uma função (ou um procedimento) no servidor e o servidor envia a saída de volta ao cliente.
- **APIs WebSocket:** O servidor pode enviar mensagens de retorno  de chamada a clientes conectados, tornando-o mais eficiente que a **API REST**.
- **APIs REST:** O cliente envia solicitação ao servidor como dados. O servidor usa essa entrada do cliente para iniciar funções internas e retorna os dados de saída ao cliente.


### O que são APIs REST?

- **REST** significa Transferência Representacional de Estado.
- Clientes e servidores trocam dados usando **HTTP**.
- O **HTTP** permite criar, atualizar, pesquisar, executar e remover operações, atuando sobe determinados recursos.
- A principal característica da **API REST** é a ausência de estados.

![[Pasted image 20240222214126.png]]


![[Pasted image 20240222214513.png]]

![[Pasted image 20240222214544.png]]

### JSON

- O JSON é um formato de troca de dados entre sistemas independente de linguagem de programação derivado do JavaScript.
- É frequentemente utilizado em aplicações Ajax, configurações, banco de dados e serviços web **RESTful**.

![[Pasted image 20240222215845.png]]

### Referências

[Link do material de estudo](https://academiapme-my.sharepoint.com/:p:/g/personal/renato_dio_me/ERVAxF7Z_uBIoMMef0ns7EUB-pRDR2J0pSJ4PS29L27_2w?rtime=5jiITRk03Eg)