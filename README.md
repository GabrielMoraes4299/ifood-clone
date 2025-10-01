# ifood-clone
# Histórias de Usuário

  ## Usuário
- Eu como **usuário** quero buscar restaurantes e produtos pelo aplicativo para escolher o que vou pedir.  
- Eu como **usuário** quero adicionar e remover itens do meu carrinho para controlar o que vou comprar.  
- Eu como **usuário** quero finalizar o pedido e pagar pelo aplicativo para recebê-lo no conforto da minha casa.

## Entregador
- Eu como **entregador** quero visualizar os pedidos para saber quantos pedidos tenho para entregar
- Eu como **entregador** quero visualizar os detalhes do pedido (itens, endereço de entrega, forma de pagamento) para realizar a entrega corretamente.  
- Eu como **entregador** quero acessar meu histórico de entregas e ganhos para acompanhar meu faturamento.  

---

# Gherkin Usuário  

## Buscar restaurantes e produtos
  Scenario: Usuário pesquisa por um restaurante existente  
    Given que o usuário está na tela inicial do aplicativo  
    When ele digitar o nome de um restaurante na busca  
    Then o sistema deve exibir a lista de restaurantes correspondentes  

  Scenario: Usuário pesquisa por um produto existente  
    Given que o usuário está na tela inicial do aplicativo  
    When ele digitar o nome de um produto na busca  
    Then o sistema deve exibir restaurantes que oferecem esse produto  

  Scenario: Usuário pesquisa por um produto ou restaurante existente  
    Given que o usuário está na tela inicial do aplicativo  
    When ele digitar o nome de um produto ou restaurante na busca  
    Then o sistema deve exibir uma mensagem de produtos ou restaurantes não encontrados  

---

## Adicionar e remover itens do carrinho
  Scenario: Usuário adiciona um item ao carrinho  
    Given que o usuário visualiza um cardápio de restaurante  
    When ele selecionar um produto e clicar em "Adicionar ao carrinho"  
    Then o produto deve ser incluído no carrinho  

  Scenario: Usuário remove um item do carrinho  
    Given que o usuário possui itens no carrinho  
    When ele clicar em "Remover" em um produto do carrinho  
    Then o produto deve ser retirado do carrinho  

---

## Finalizar pedido e pagar
  Scenario: Usuário finaliza pedido com sucesso  
    Given que o usuário tem itens no carrinho  
    And escolheu a forma de pagamento  
    When ele clicar em "Finalizar pedido"  
    Then o sistema deve registrar o pedido  
    And o pagamento deve ser processado  
    And o usuário deve ver a confirmação com o tempo estimado de entrega  

  Scenario: Pagamento não autorizado  
    Given que o usuário tem itens no carrinho  
    And escolheu a forma de pagamento  
    When o pagamento for recusado pelo sistema de pagamento  
    Then o sistema deve informar que o pagamento não foi autorizado  
    And permitir que o usuário tente novamente ou escolha outra forma de pagamento  

---

# Gherkin Entregador  

## Visualizar pedidos

Scenario: Entregador acessa detalhes de um pedido disponível
Given que o entregador está logado no aplicativo  
When ele abrir a tela de "Pedidos disponíveis"  
And não houver nenhum pedido  
Then o sistema deve exibir os pedidos pendentes com itens, endereço e forma de pagamento

---

## Visualizar detalhes do pedido
  Scenario: Entregador acessa detalhes de um pedido disponível  
    Given que o entregador está logado no aplicativo  
    When ele abrir a tela de "Pedidos disponíveis"
    And clicar em um pedido
    Then o sistema deve exibir os itens, endereço e forma de pagamento  

---

## Acessar histórico de entregas e ganhos
  Scenario: Entregador acessa histórico  
    Given que o entregador está logado no aplicativo  
    When ele acessar a tela de "Histórico"  
    Then o sistema deve mostrar a lista de entregas concluídas com valores pagos  

  Scenario: Entregador acessa histórico  
    Given que o entregador está logado no aplicativo  
    When ele acessar a tela de "Histórico" mas não tem entregas concluídas  
    Then o sistema deve mostrar uma mensagem de que não há entregas concluídas 

  Scenario: Entregador filtra histórico por período  
    Given que o entregador está na tela de "Histórico"  
    When ele selecionar um intervalo de datas  
    Then o sistema deve exibir apenas as entregas realizadas nesse período

  Scenario: Entregador filtra histórico por período  
  Given que o entregador está na tela de "Histórico"  
  When ele selecionar um intervalo de datas inválidas  
  Then o sistema deve exibir uma mensagem pedindo datas válidas

---

# Documentação do Projeto

## Diagramas de Sequência
- [Realizar Pagamento](./Diagrama%20de%20Sequência%20-%20Realizar%20Pagamento.png)
- [Visualizar Detalhes do Pedido](./Diagrama%20de%20Sequência%20-%20Visualizar%20Detalhes%20do%20Pedido.png)
- [Visualizar Histórico de Entregas](./Diagrama%20de%20Sequência%20-%20Visualizar%20Histórico%20de%20Entregas.png)
- [Buscar Produtos](./Diagrama%20de%20Sequência%20-%20Buscar%20Produtos.png)
- [Gerenciar Carrinho](./Diagrama%20de%20Sequência%20-%20Gerenciar%20Carrinho.png)

## Diagramas de Caso de Uso
- [Usuário](./Diagrama%20de%20Casos%20de%20Uso%20-%20Usuário.png)
- [Entregador](./Diagrama%20de%20Casos%20de%20Uso%20-%20Entregador.png)

## Telas
- [Esboço de Tela - Usuário](./Esboço%20de%20Tela%20-%20Usuário.png)  
- [Esboço de Tela - Entregador](./Esboço%20de%20Tela%20-%20Entregador.png)  

---

# Requisitos Não-Funcionais

## Usabilidade
- A interface deve ser intuitiva e responsiva, permitindo que usuários e entregadores utilizem o app sem necessidade de treinamento.
- O fluxo de pedido (buscar → adicionar ao carrinho → pagar) deve ser concluído em poucos cliques.
- Deve oferecer acessibilidade, com suporte a leitores de tela e contraste adequado.

## Desempenho
- O sistema deve suportar milhares de usuários simultâneos sem degradação significativa de desempenho.
- O tempo de resposta das requisições (ex.: buscar restaurantes, atualizar carrinho) deve ser inferior a 2 segundos em condições normais de rede.
- O carregamento das telas deve ser otimizado para dispositivos móveis de média performance.

## Manutenibilidade
- O código deve seguir boas práticas de desenvolvimento (ex.: padrões de projeto, separação em camadas).
- O sistema deve possuir testes automatizados que facilitem futuras atualizações sem comprometer funcionalidades existentes.
- A arquitetura deve ser modular, permitindo substituição ou atualização de componentes sem afetar o todo.

## Portabilidade
- O aplicativo deve estar disponível para Android e iOS.
- A aplicação web (se houver) deve ser compatível com os principais navegadores (Chrome, Edge, Safari, Firefox).
- O sistema deve ser adaptável a diferentes resoluções de tela (celulares, tablets).

## Segurança
- Os dados dos usuários e entregadores devem ser criptografados em trânsito (HTTPS/TLS).
- As informações sensíveis (como senhas e dados de pagamento) devem ser armazenadas de forma segura (hash/salt, PCI DSS).
- O sistema deve implementar autenticação segura (ex.: OAuth2, JWT).
- Deve haver proteção contra ataques comuns (SQL Injection, XSS, CSRF).

## Confiabilidade
- O sistema deve ter disponibilidade mínima de 99,5% (SLA mensal).
- Deve existir um plano de recuperação em caso de falhas (backup automático e redundância de servidores).
- Em caso de falha de um serviço (ex.: pagamento), o sistema deve informar claramente o usuário e permitir nova tentativa.
