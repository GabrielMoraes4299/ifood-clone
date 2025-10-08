# Gherkin Cliente  

## Buscar restaurantes e produtos
  **Scenario**: Cliente pesquisa por um restaurante existente  
    **Given** que o cliente está na tela inicial do aplicativo  
    **When** ele digitar o nome de um restaurante na busca  
    **Then** o sistema deve exibir a lista de restaurantes correspondentes  

  **Scenario**: Cliente pesquisa por um produto existente  
    **Given** que o cliente está na tela inicial do aplicativo  
    **When** ele digitar o nome de um produto na busca  
    **Then** o sistema deve exibir restaurantes que oferecem esse produto  

  **Scenario**: Cliente pesquisa por um produto ou restaurante existente  
    **Given** que o cliente está na tela inicial do aplicativo  
    **When** ele digitar o nome de um produto ou restaurante na busca  
    **Then** o sistema deve exibir uma mensagem de produtos ou restaurantes não encontrados  

---

## Adicionar e remover itens do carrinho
  **Scenario**: Cliente adiciona um item ao carrinho  
    **Given** que o cliente visualiza um cardápio de restaurante  
    **When** ele selecionar um produto e clicar em "Adicionar ao carrinho"  
    **Then** o produto deve ser incluído no carrinho  

  **Scenario**: Cliente remove um item do carrinho  
    **Given** que o cliente possui itens no carrinho  
    **When** ele clicar em "Remover" em um produto do carrinho  
    **Then** o produto deve ser retirado do carrinho  

---

## Finalizar pedido e pagar
  **Scenario**: Cliente finaliza pedido com sucesso  
    **Given** que o cliente tem itens no carrinho  
    **And** escolheu a forma de pagamento  
    **When** ele clicar em "Finalizar pedido"  
    **Then** o sistema deve registrar o pedido  
    **And** o pagamento deve ser processado  
    **And** o cliente deve ver a confirmação com o tempo estimado de entrega  

  **Scenario**: Pagamento não autorizado  
    **Given** que o cliente tem itens no carrinho  
    **And** escolheu a forma de pagamento  
    **When** o pagamento for recusado pelo sistema de pagamento  
    **Then** o sistema deve informar que o pagamento não foi autorizado  
    **And** permitir que o cliente tente novamente ou escolha outra forma de pagamento  

---