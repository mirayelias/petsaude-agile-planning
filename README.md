# PetSaúde - Gestão e Agendamento Veterinário

## Visão Geral do Projeto
O **PetSaúde** é uma plataforma voltada para tutores de animais de estimação realizarem agendamentos de consultas veterinárias, banho e tosa, além de acompanhar o histórico de vacinas e prontuário digital do pet.

---

## Governança da Squad e Papéis (Scrum & Agile)

- **Elias dos Santos:** Product Owner (PO) & Product Manager (PM)
  - Responsável pela visão do produto, escrita do Backlog, priorização de negócios e validação dos Critérios de Aceitação.
- **Squad de Desenvolvimento:**
  - **Kauazinho (Tech Lead / Backend):** Arquitetura de banco de dados e APIs RESTful.
  - **Joãozinho (Frontend / UI/UX):** Desenvolvimento das interfaces web/mobile e experiência do usuário.
  - **Lorenzinho (QA & DevOps):** Garantia de qualidade, testes automatizados e integração contínua.

---

## Definição de Prontidão e Conclusão

- **DoR (Definition of Ready):** História escrita no padrão INVEST, com critérios de aceitação claros, priorizada pelo PO e estimativa de Story Points atribuída pela squad.
- **DoD (Definition of Done):** Código integrado à branch principal via Pull Request, revisado por 1 peer, com testes unitários passando e documentado no Swagger.

- #  Declaração de Alinhamento Estratégico da Reta Final (PO)

## 1. Fluxo Nuclear Demonstrável (Happy Path)
O caminho principal ponta a ponta que a squad garantirá em perfeito funcionamento perante a banca avaliadora será:
- **Passo a passo:** O cliente acessa o catálogo de produtos orgânicos, utiliza a busca dinâmica, adiciona itens desejados ao carrinho de compras, aplica o cálculo de frete por CEP e finaliza o pedido com sucesso, gerando o registro correspondente no banco de dados e exibindo a notificação de confirmação.

## 2. Justificativa dos Cortes de Escopo (Won't Have)
Após a análise de priorização e restrição de cronograma para a reta final:
- **Funcionalidades postergadas:** O módulo de gamificação/ranking de voluntários e o painel avançado de relatórios gerenciais para administradores foram movidos para o escopo *Won't Have* (backlog futuro).
- **Fundamentação:** A decisão baseou-se na mitigação de riscos técnicos, focando 100% dos esforços de desenvolvimento na estabilização do fluxo central de vendas (catálogo, carrinho e checkout).

## 3. Blindagem e Contingência Operacional
Para neutralizar riscos de infraestrutura no dia da apresentação à banca, adotamos as seguintes salvaguardas:
- **Ambiente local de contingência:** Toda a aplicação (frontend, backend e banco de dados) estará containerizada via Docker, permitindo a execução offline completa caso ocorram falhas de conexão com a internet ou instabilidade no deploy em nuvem.
- **Massa de dados pré-populada:** Scripts de inicialização com produtos, categorias e utilizadores de teste configurados para demonstração imediata.
