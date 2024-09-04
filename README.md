# Serviço de microserviço

### Irei utiliar conceitos básicos de micro-serviços.

#### Cenário de estudo.

O que espero desse sistema? 

Tenha dois microserviços de negocio: Um de cliente e um pedido, onde eles tem recursos compartilhados como o pedido precisa de um cliente
para ser valido e os dois tem um recurso em comum compartilhado que seria o endereço.

Tenha um microserviço para redicionamento de rota (PROXY), que será o API Gateway.

Tenha um microserviço de autenticação com o keycloack que vai controlar todos os acessos e permissões no sistema.

Cada microserviço deve ter um banco de dados próprio, por exemplo o de cliente e pedido deve ter o seu proprio banco de dados.
Enquanto o keycloack também tem seu banco de dados próprio o único que não vai ter banco de dados é o MS-GATEWAY.

Tenha um frontend em react que consiga controlar os acessos pelo keycloack com os conceitos basicos de criação de cliente e pedido.
