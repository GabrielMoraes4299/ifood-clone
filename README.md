# ifood-clone
Este projeto é um clone conceitual do
iFood, desenvolvido como parte da
disciplina de Engenharia de Software. O
objetivo é aplicar os conceitos de
levantamento de requisitos, modelagem e
prototipação de sistemas.

---

# Autor
- Gabriel Chagas Fernandes de Moraes – Análise e Desenvolvimento de Sistemas

---

# Levantamento de Requisitos

### Histórias de Usuário
- 👤[Cliente](./História%20de%20Usuário%20-%20Cliente.md)
- 🛵[Entregador](./História%20de%20Usuário%20-%20Entregador.md)

---

### Gherkin
- 🙋[Cliente](./Gherkin%20-%20Cliente.md)
- 📦[Entregador](./Gherkin%20-%20Entregador.md)
---

# Documentação do Projeto

### Diagramas de Sequência
- 💵[Realizar Pagamento](./Diagrama%20de%20Sequência%20-%20Realizar%20Pagamento.png)
- 🍔[Visualizar Detalhes do Pedido](./Diagrama%20de%20Sequência%20-%20Visualizar%20Detalhes%20do%20Pedido.png)
- 📜[Visualizar Histórico de Entregas](./Diagrama%20de%20Sequência%20-%20Visualizar%20Histórico%20de%20Entregas.png)
- 🔍[Buscar Produtos](./Diagrama%20de%20Sequência%20-%20Buscar%20Produtos.png)
- 🛒[Gerenciar Carrinho](./Diagrama%20de%20Sequência%20-%20Gerenciar%20Carrinho.png)

### Diagramas de Caso de Uso
- 🍴[Cliente](./Diagrama%20de%20Casos%20de%20Uso%20-%20Cliente.png)
- 🛵[Entregador](./Diagrama%20de%20Casos%20de%20Uso%20-%20Entregador.png)

### Wireframes
- 🍽️[Esboço de Tela - Cliente](./Esboço%20de%20Tela%20-%20Cliente.png)  
- 🛵[Esboço de Tela - Entregador](./Esboço%20de%20Tela%20-%20Entregador.png)  

---

### Interfaces
- 🍽️[Interface - Cliente](./Interface%20-%20Cliente.png)  
- 🛵[Interface - Entregador](./Interface%20-%20Entregador.png)  

---

# Requisitos Não-Funcionais

### Usabilidade
- A interface deve ser intuitiva e responsiva, permitindo que usuários e entregadores utilizem o app sem necessidade de treinamento.
- O fluxo de pedido (buscar → adicionar ao carrinho → pagar) deve ser concluído em poucos cliques.
- Deve oferecer acessibilidade, com suporte a leitores de tela e contraste adequado.

### Desempenho
- O sistema deve suportar milhares de usuários simultâneos sem degradação significativa de desempenho.
- O tempo de resposta das requisições (ex.: buscar restaurantes, atualizar carrinho) deve ser inferior a 2 segundos em condições normais de rede.
- O carregamento das telas deve ser otimizado para dispositivos móveis de média performance.

### Manutenibilidade
- O código deve seguir boas práticas de desenvolvimento (ex.: padrões de projeto, separação em camadas).
- O sistema deve possuir testes automatizados que facilitem futuras atualizações sem comprometer funcionalidades existentes.
- A arquitetura deve ser modular, permitindo substituição ou atualização de componentes sem afetar o todo.

### Portabilidade
- O aplicativo deve estar disponível para Android e iOS.
- A aplicação web (se houver) deve ser compatível com os principais navegadores (Chrome, Edge, Safari, Firefox).
- O sistema deve ser adaptável a diferentes resoluções de tela (celulares, tablets).

### Segurança
- Os dados dos usuários e entregadores devem ser criptografados em trânsito (HTTPS/TLS).
- As informações sensíveis (como senhas e dados de pagamento) devem ser armazenadas de forma segura (hash/salt, PCI DSS).
- O sistema deve implementar autenticação segura (ex.: OAuth2, JWT).
- Deve haver proteção contra ataques comuns (SQL Injection, XSS, CSRF).

### Confiabilidade
- O sistema deve ter disponibilidade mínima de 99,5% (SLA mensal).
- Deve existir um plano de recuperação em caso de falhas (backup automático e redundância de servidores).
- Em caso de falha de um serviço (ex.: pagamento), o sistema deve informar claramente ao usuário e permitir nova tentativa.
