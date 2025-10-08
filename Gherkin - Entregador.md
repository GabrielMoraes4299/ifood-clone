# Gherkin Entregador  

## Visualizar pedidos

**Scenario**: Entregador acessa a tela de "Pedidos" com pedidos disponíveis
**Given** que o entregador está logado no aplicativo  
**When** ele abrir a tela de "Pedidos"  
**And** houver pedidos  
**Then** o sistema deve exibir os pedidos

**Scenario**: Entregador acessa a tela de "Pedidos" sem pedidos
**Given** que o entregador está logado no aplicativo  
**When** ele abrir a tela de "Pedidos disponíveis"  
**And** não houver pedidos  
**Then** o sistema deve exibir uma mensagem inform**and**o que não há pedidos

---

## Visualizar detalhes do pedido
**Scenario**: Entregador acessa detalhes de um pedido disponível
**Given** que o entregador está logado no aplicativo  
**When** ele abrir a tela de "Pedidos disponíveis"  
**And** clicar em um pedido  
**Then** o sistema deve exibir os pedidos pendentes com itens, endereço e forma de pagamento

---

## Acessar histórico de entregas e ganhos
  **Scenario**: Entregador acessa histórico  
    **Given** que o entregador está logado no aplicativo  
    **When** ele acessar a tela de "Histórico"  
    **Then** o sistema deve mostrar a lista de entregas concluídas com valores pagos  

  **Scenario**: Entregador acessa histórico  
    **Given** que o entregador está logado no aplicativo  
    **When** ele acessar a tela de "Histórico" mas não tem entregas concluídas  
    **Then** o sistema deve mostrar uma mensagem de que não há entregas concluídas 

  **Scenario**: Entregador filtra histórico por período  
    **Given** que o entregador está na tela de "Histórico"  
    **When** ele selecionar um intervalo de datas  
    **Then** o sistema deve exibir apenas as entregas realizadas nesse período

  **Scenario**: Entregador filtra histórico por período  
  **Given** que o entregador está na tela de "Histórico"  
  **When** ele selecionar um intervalo de datas inválidas  
  **Then** o sistema deve exibir uma mensagem pedindo datas válidas

---