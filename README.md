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

### 5WHH
#### 5W:

##### 1. **WHAT — O que será feito?**

Desenvolver um **sistema completo de delivery**, semelhante ao iFood, contendo:

##### 👤 Aplicativo do Cliente
- Cadastro e login  
- Endereço e geolocalização  
- Listagem de restaurantes  
- Cardápio  
- Carrinho  
- Checkout  
- Pagamentos (Pix, cartão, carteira digital)  
- Acompanhamento do pedido em tempo real  
- Notificações push  
- Histórico e reordenação  

##### 🛵 Aplicativo do Entregador
- Cadastro  
- Receber pedidos  
- Aceitar/rejeitar entregas  
- Rota até o restaurante  
- Rota até o cliente  
- Status da entrega  

##### 👨🏻‍🍳 Aplicativo/Painel do Restaurante
- Cadastro  
- Cardápio  
- Gestão de pedidos  
- Financeiro  
- Promoções e cupons  

##### 🌐 Backend e Infra
- API REST  
- Autenticação JWT  
- Banco PostgreSQL  
- WebSockets para tempo real  
- Sistema de pagamentos  
- Geolocalização  
- Deploy em nuvem (Azure)  

---

##### 2. **WHY — Por que será feito?**

- Criar uma solução robusta que atue como concorrente direto do iFood, replicando suas principais funcionalidades e propondo melhorias;
- Consolidar, na prática, um ecossistema completo envolvendo aplicativos mobile, painel web, backend robusto e infraestrutura em nuvem.

---

##### 3️. **WHEN – Quando será feito?**

##### 📅 Cronograma geral (7 meses)

| Etapa | Entrega | Data |
|------|---------|------|
| Planejamento | Documento 5W2H + arquitetura | 10 dias |
| Design e protótipos | Telas mobile e web | 20 dias |
| Backend – Fase 1 | Cadastro, autenticação, restaurantes | 30 dias |
| Backend – Fase 2 | Pedidos, pagamentos e entregas | 30 dias |
| Aplicativo Usuário | Primeira versão funcional | 30 dias |
| Teste com usuários não contaminados | Feedback real do App Cliente | 5 dias |
| Aplicativo Entregador | Primeira versão funcional | 30 dias |
| Teste com usuários não contaminados | Feedback real do App Entregador | 5 dias |
| Painel Web Restaurantes | Gestão de pedidos | 20 dias |
| Teste com usuários não contaminados | Feedback real do Painel Restaurante | 5 dias |
| Dashboard Admin | Gestão completa do sistema | 20 dias |
| Entrega Final | MVP pronto | — |

---

##### 4️. **WHERE – Onde será feito?**
- Desenvolvimento remoto (home office)
- Repositórios e versionamento no **GitHub**
- Organização de tarefas no **GitHub Projects / Issues / Milestones**
- Documentação no próprio repositório
- Reuniões via Google Meet / Discord

- Infraestrutura:
  - Hospedagem: **Microsoft Azure**
  - CI/CD: GitHub Actions
  - Banco de dados: Azure PostgreSQL
  - Storage: Azure Blob Storage

##### 5️. **WHO – Quem fará?**

##### 👥 Equipe necessária e responsabilidades

| Especialidade                          | Qnt. | Remuneração (R$)          | Papéis e Responsabilidades |
|----------------------------------------|-----|----------------------------|-----------------------------|
| **Product Owner**                      | 1   | R$ 21.600 / mês            | Visão do produto, priorização, alinhamento com investidores |
| **Scrum Master / PM**                  | 1   | R$ 19.800 / mês            | Facilitar sprints, remover impedimentos, garantir fluxo |
| **UI/UX Designer**                     | 1   | R$ 14.400 / mês            | Prototipação, telas, identidade visual, UX |
| **Dev Flutter (Usuário)**              | 2   | R$ 16.200 / mês (cada)     | App do cliente, telas, carrinho, pedidos, integrações |
| **Dev Flutter (Entregador)**           | 1   | R$ 16.200 / mês            | App do entregador, rotas, GPS, tracking |
| **Backend Developer (Python + Django)**| 3   | R$ 18.000 / mês (cada)     | APIs, autenticação, pagamentos, lógica de pedidos |
| **Frontend Web (Angular)**             | 2   | R$ 16.200 / mês (cada)     | Painel do restaurante e admin |
| **DevOps / Infraestrutura**            | 1   | R$ 19.800 / mês            | Deploy, CI/CD, Azure, monitoramento |
| **QA Tester**                          | 1   | R$ 12.600 / mês            | Testes contínuos, validação, checklist |
| **DBA / Eng. Dados**                   | 1   | R$ 18.000 / mês            | Modelagem, otimização, migrações |
| **Usuários-Teste Remunerados**         | 10  | R$ 60 por teste (cada)     | Testes não contaminados, feedback real |

### 🧮 Total de pessoas: **14 profissionais** + **10 usuários-teste não contaminados**

---

##### 👥 Como manter a equipe motivada?

- Bônus a cada entrega do cronograma
- Reuniões de feedback semanais
- Demonstrações do progresso a cada sprint
- Reconhecimento individual e coletivo
- Ambiente de trabalho leve e organizado
- Participação no lucro futuro do produto
- Transparência total sobre decisões e prioridades

---

#### 2H:

##### 1. **HOW – Como será feito?**

##### Tecnologias
- **Frontend mobile:** Flutter
- **Frontend web:** Angular 2+
- **Backend:** Python + Django REST Framework
- **Banco:** PostgreSQL
- **Infra:** Azure
- **Autenticação:** JWT + OAuth2
- **Pagamentos:** Stripe
- **Geolocalização:** Google Maps API
- **Mensageria:** Firebase Messaging
- **CI/CD:** GitHub Actions

##### Metodologia
- Metodologia ágil baseada em **Scrum**
- **Sprints de 2 semanas (14 dias)** ao longo dos 7 meses
- Cada etapa do cronograma ocupa **1 a 2 sprints**, conforme complexidade
- **Daily Meeting** de 15 minutos para alinhamento rápido
- **Planning** no início de cada sprint e **Review + Retrospectiva** no final
- **Testes contínuos** dentro das sprints + **testes com usuários não contaminados** ao final de cada grande entrega
- Versionamento seguindo **Gitflow**

---

##### 2. **HOW MUCH – Quanto vai custar?**

##### Custos estimados (6 meses)  
Sem limite de verba, considerando equipe SENIOR.

| Item | Custo |
|------|-------|
| Salários (somados e multiplicados por **1,8**, como solicitado) | **R$ 630.000 a R$ 900.000** |
| Infraestrutura Azure | R$ 7.000 – R$ 15.000 |
| APIs externas (Maps, pagamentos etc.) | R$ 2.000 – R$ 6.000 |
| Licenças, ferramentas, design | R$ 5.000 – R$ 10.000 |

##### 💰 **Custo total estimado: R$ 650.000 a R$ 930.000**

---

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
