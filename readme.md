# API, REST, RESTFUL e Microserviços

## API

Imagine uma situação em um restaurante:

- **Cliente**: Você, sentado na mesa, pedindo seu prato.
- **Garçom**: O intermediário que anota seu pedido e o leva até a cozinha.
- **Cozinha**: O local onde seu pedido é preparado.

Na analogia, o garçom representa a **API**.

### O que é uma API?

Uma API (Interface de Programação de Aplicações) é um conjunto de rotinas e padrões estabelecidos por uma aplicação para que outras aplicações possam utilizar suas funcionalidades. Em outras palavras, uma API permite a comunicação entre diferentes serviços.

- **Responsável por estabelecer comunicação entre diferentes serviços**.
- **Meio de Campo entre as tecnologias**.

## REST

REST (Representational State Transfer) são boas práticas utilizadas na transferência de dados em APIs. Geralmente, a transferência é feita utilizando o protocolo HTTP. Na analogia do restaurante, o protocolo HTTP seria equivalente ao bloco de notas do garçom, onde ele anota seus pedidos e leva até a cozinha.

### O que é REST?

REST define obrigações para essas transferências de dados, baseadas em recursos (entidades, objetos, dados).

### 5 necessidades (constraints) para cumprir e se tornar RESTFUL:

1. **Client-server**: O cliente e o servidor precisam estar separados. A separação permite a portabilidade do sistema, usando diferentes tecnologias para a web e dispositivos móveis, como React para web e React Native para smartphones.

2. **Stateless**: Cada requisição do cliente ao servidor deve conter todas as informações necessárias para que o servidor entenda e responda à requisição. O servidor não deve "lembrar" que o cliente foi autenticado na requisição anterior. Por exemplo, a sessão do usuário deve ser enviada em todas as requisições para confirmar que o usuário está autenticado.

3. **Cacheable**: As respostas para uma requisição devem ser explícitas ao informar se aquela requisição pode ou não ser cacheada pelo cliente.

4. **Layered System**: O cliente acessa um endpoint sem precisar conhecer a complexidade e os passos necessários para o servidor responder à requisição.

5. **Code on demand (optional)**: Dá à aplicação a possibilidade de pegar códigos (como JavaScript) e executá-los no cliente.

## RESTFUL

Ser RESTful significa aplicar todos os padrões REST mencionados acima.

## APIs REST

APIs RESTful são interfaces que seguem os princípios REST, permitindo a comunicação entre diferentes softwares ou serviços. 

Geralmente, os dados são transferidos em formatos como JSON.

### Ferramentas para APIs REST

- **POSTMAN**: Utilizado para fazer testes de API, facilitando o envio de requisições e a visualização de respostas.

## Microserviços

### O que são Microserviços?

Microserviços são uma abordagem arquitetônica para o desenvolvimento de software, onde uma aplicação é estruturada como um conjunto de serviços pequenos e independentes, que comunicam entre si por meio de APIs.

### Características dos Microserviços:

1. **Modularidade**: Cada microserviço é uma unidade funcional independente, responsável por uma única funcionalidade da aplicação.
2. **Independência de Desenvolvimento**: Equipes podem trabalhar em diferentes microserviços de forma independente, usando diferentes tecnologias e linguagens de programação.
3. **Escalabilidade**: Cada microserviço pode ser escalado de forma independente, conforme a demanda de sua funcionalidade específica.
4. **Facilidade de Manutenção**: Modificações, atualizações e correções podem ser feitas em um microserviço específico sem afetar os demais.
5. **Resiliência**: Falhas em um microserviço não comprometem a aplicação inteira, aumentando a robustez do sistema.

### Benefícios dos Microserviços:

- **Melhoria na Organização de Equipes**: Equipes menores e especializadas podem ser atribuídas a diferentes microserviços.
- **Atualizações e Deploys Mais Ágeis**: Mudanças podem ser implementadas e lançadas mais rapidamente.
- **Adoção de Tecnologias Diversas**: Possibilidade de usar a tecnologia mais adequada para cada microserviço.

### Desafios dos Microserviços:

- **Complexidade de Gestão**: Requer um sistema de orquestração e monitoramento eficiente.
- **Comunicação entre Serviços**: Necessidade de gerenciar chamadas de API, autenticação e segurança entre microserviços.
- **Manutenção de Consistência**: Garantir que os dados e estados entre diferentes microserviços estejam sempre consistentes.

### Ferramentas e Tecnologias para Microserviços:

- **Docker**: Para criar, implantar e executar aplicações em containers.
- **Kubernetes**: Para orquestração de containers, gerenciando automaticamente a implantação, dimensionamento e operações de aplicativos em containers.
- **Istio**: Para gerenciar a comunicação segura entre microserviços, fornecendo monitoramento, segurança e roteamento de tráfego.

### Resumo

- **API**: Interface para comunicação entre diferentes softwares.
- **REST**: Conjunto de boas práticas para transferências de dados em APIs.
- **RESTFUL**: Aplicação completa dos padrões REST.
- **Microserviços**: Abordagem arquitetônica onde uma aplicação é composta por serviços pequenos e independentes, facilitando a escalabilidade e manutenção.

