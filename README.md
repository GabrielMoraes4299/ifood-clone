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
- 🎨[Protótipo no Figma](https://www.figma.com/design/0wILuw3bEQJP4ZskA0KHIF/ifood-clone---Gabriel-Chagas?node-id=0-1&t=hMnF3ZHYifUxAjAL-1)

---

## ✅ Requisitos Não Funcionais

Abaixo estão listados os principais requisitos não funcionais do sistema, juntamente com as formas de comprovar que cada um foi considerado e atendido durante o desenvolvimento do projeto.

| **Requisito Não Funcional** | **Descrição** | **Método de Validação (Comprovação)** |
|------------------------------|----------------|----------------------------------|
| **Desempenho** | O sistema deve responder em até 2 segundos após uma ação do usuário. | Foi realizado um teste prático medindo o tempo de resposta das telas e requisições. O tempo médio ficou abaixo de 2 segundos, comprovando boa performance. |
| **Usabilidade** | O sistema deve ser fácil de usar, com interface intuitiva e clara. | O design foi criado no [Figma](https://www.figma.com/design/0wILuw3bEQJP4ZskA0KHIF/ifood-clone---Gabriel-Chagas?node-id=0-1&t=hMnF3ZHYifUxAjAL-1) e validado com usuários-teste. A navegação é simples e direta. |
| **Confiabilidade** | O sistema deve funcionar sem travamentos ou erros inesperados. | Foram realizados testes manuais e automatizados. Nenhum erro crítico foi encontrado durante a demonstração contínua do sistema. |
| **Segurança** | Os dados sensíveis devem ser protegidos e acessíveis apenas a usuários autorizados. | Implementado controle de autenticação e verificação de login. As senhas são tratadas de forma segura e as rotas protegidas. |
| **Manutenibilidade** | O código deve ser organizado e bem documentado, facilitando futuras alterações. | O repositório segue boas práticas, com README, commits descritivos e comentários no código. A estrutura de pastas está clara e modular. |
| **Compatibilidade** | O sistema deve funcionar corretamente em diferentes dispositivos e navegadores. | O design responsivo foi testado em versões desktop e mobile, garantindo compatibilidade com Chrome, Edge e Firefox. |
| **Escalabilidade** | A aplicação deve suportar o aumento de usuários sem perda de desempenho. | A arquitetura foi pensada com separação de camadas e consumo de API, facilitando o aumento de carga futura. |
| **Disponibilidade** | O sistema deve estar disponível para acesso a qualquer momento. | O projeto está hospedado em ambiente online confiável, garantindo acesso contínuo ao cliente e usuários. |
| **Portabilidade** | O sistema deve poder ser executado em diferentes ambientes. | O projeto pode ser rodado localmente ou hospedado em cloud, com suporte a múltiplos sistemas operacionais. |
| **Acessibilidade** | A interface deve ser legível e navegável por todos os tipos de usuários. | Foram aplicados contrastes adequados, textos legíveis e suporte à navegação por teclado. Avaliado com ferramenta Lighthouse. |

---
