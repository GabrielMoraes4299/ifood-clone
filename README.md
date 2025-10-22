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

Abaixo estão listados os principais requisitos não funcionais do sistema *iFood Clone*, juntamente com as formas de comprovar que cada um foi considerado e atendido durante o desenvolvimento do projeto.

| **Requisito Não Funcional** | **Descrição** | **Método de Validação (Comprovação)** |
|------------------------------|----------------|----------------------------------|
| **Desempenho** | O sistema deve responder rapidamente às ações do usuário, garantindo fluidez na navegação e no carregamento dos restaurantes e produtos. | Foram realizados testes práticos medindo o tempo de resposta das telas e das requisições à API. As telas principais carregam em até 2 segundos, comprovando boa performance. |
| **Usabilidade** | O sistema deve ser fácil de usar, com interface intuitiva e semelhante a aplicativos de delivery reais. | O design foi criado no [Figma](https://www.figma.com/design/0wILuw3bEQJP4ZskA0KHIF/ifood-clone---Gabriel-Chagas?node-id=0-1&t=hMnF3ZHYifUxAjAL-1) e validado com usuários-teste. A navegação segue padrões familiares, como menus fixos e ícones intuitivos. |
| **Confiabilidade** | O sistema deve funcionar sem falhas, exibindo corretamente os pedidos, produtos e informações dos restaurantes. | Foram realizados testes manuais e simulações de fluxo completo (cadastro, login, pedido). Nenhum erro crítico foi identificado durante o uso contínuo do sistema. |
| **Segurança** | Os dados dos usuários (login, senha e pedidos) devem ser protegidos contra acesso não autorizado. | Foi implementado controle de autenticação, criptografia de senhas e validação de campos. As requisições sensíveis são tratadas com segurança. |
| **Manutenibilidade** | O código deve ser modular e bem documentado, permitindo futuras atualizações, como inclusão de novas funcionalidades. | O repositório segue boas práticas de desenvolvimento, com commits descritivos, organização em componentes e documentação clara no README. |
| **Compatibilidade** | O sistema deve funcionar corretamente em diferentes tamanhos de tela (smartphones e tablets). | O layout responsivo foi testado em emuladores Android e iOS, garantindo boa experiência visual e funcional em diferentes resoluções. |
| **Escalabilidade** | A aplicação deve suportar o crescimento do número de usuários, restaurantes e pedidos. | A arquitetura utiliza comunicação via API e separação entre front-end e back-end, permitindo expansão futura sem comprometer o desempenho. |
| **Disponibilidade** | O sistema deve estar acessível para usuários e restaurantes sempre que necessário. | O projeto pode ser hospedado em ambiente de nuvem (como Azure), com alta disponibilidade e estabilidade durante testes de uso. |
| **Portabilidade** | O sistema deve poder ser executado em diferentes plataformas (web e mobile). | O projeto foi desenvolvido em Flutter, permitindo execução em Android, iOS e Web a partir do mesmo código-fonte. |
| **Acessibilidade** | O sistema deve ser acessível e legível para todos os tipos de usuários. | Foram aplicados contrastes adequados, textos legíveis e botões grandes. Também foi avaliado com o Lighthouse para garantir boa acessibilidade. |

---

## 🙏 Agradecimentos

Obrigado por conferir este projeto! 🚀💻  
Esperamos que ele seja útil e divertido de explorar ⭐✨
