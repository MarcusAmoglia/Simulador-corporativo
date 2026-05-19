#  Simulador Corporativo Web (Engenharia de Software, PO & QA)
> **Nota de Confidencialidade:** Este software possui propriedade intelectual protegida e código-fonte fechado. Este repositório serve como portfólio técnico para demonstrar minha atuação em Engenharia de Software (Arquitetura e Motores de Cálculo), Desenvolvimento Full Stack, Product Ownership e Engenharia de Qualidade (QA).

---

## 🚀 Links do Projeto
* **Demonstração em Vídeo (Explicação do Software):** [Assistir no YouTube](https://www.youtube.com/watch?v=w793MSipWZM)
* **Ambiente de Homologação (Deploy):** [Acessar App na Vercel](https://projeto-vercel-stem-cs.vercel.app/)

---

## 💻 Arquitetura e Stack Técnica
O sistema é uma plataforma robusta de simulação de tomada de decisões corporativas, onde o maior desafio técnico foi a modelagem e o processamento de dados financeiros e administrativos em tempo real.

* **Backend:** Java (Spring Boot) / Node.js (Desenvolvimento do motor de regras, microsserviços e persistência).
* **Frontend:** React.js + Vite & Tailwind CSS (Consumo das APIs e renderização dos painéis dinâmicos de forma responsiva).
* **Processo & Gestão:** Scrum/Kanban com foco em Engenharia de Requisitos orientada a código.

---

## 🎯 Minhas Contribuições Técnicas e Práticas

### 1. Engenharia de Software & Motores de Cálculo (Cérebro do Backend)
Minha principal contribuição no projeto foi a **concepção, modelagem e codificação de toda a lógica matemática e de engenharia de software** que roda por trás do simulador no backend (Java/Spring Boot e Node.js).
* **Desenvolvimento dos Algoritmos de Simulação:** Projetei e implementei os cálculos matemáticos complexos que processam os dados inseridos pelos usuários e geram os resultados analíticos da simulação (projeções financeiras, balanços, taxas de depreciação e matrizes de decisão corporativa).
* **Arquitetura de Dados:** Garanti que esses cálculos fossem performáticos, evitando gargalos de processamento no servidor e assegurando a consistência dos estados da aplicação a cada nova rodada/turno simulado.
* **Validação Severa no Core:** Implementei camadas de validação no backend para impedir que inputs corrompidos ou inconsistentes chegassem ao motor de cálculo, blindando o sistema contra falhas de lógica.

### 2. Engenharia de Requisitos & Gestão de Produto (Product Owner)
Por ter desenhado a engenharia dos cálculos, consegui atuar como um PO extremamente técnico, eliminando o "telefone sem fio" entre o negócio e o código:
* **Mapeamento de Épicos e Histórias:** Traduzi as necessidades dos stakeholders diretamente em arquitetura de software e User Stories refinadas.
* **Critérios de Aceite Automatizáveis:** Estruturei regras de negócio complexas no padrão BDD (Gherkin), servindo como documentação viva tanto para os desenvolvedores quanto para a estratégia de qualidade.

### 3. Engenharia de Qualidade (QA & Estratégia de Testes)
Como fui o autor dos cálculos do backend, desenhei a matriz de testes focada em estressar os limites dos algoritmos que eu mesmo criei:
* **Testes de Integração e Regressão de APIs:** Validação exaustiva de payloads, códigos de status HTTP e precisão matemática das respostas JSON vindas do backend.
* **Fidelidade de UI (Frontend):** Testes na interface React com Tailwind para garantir que o consumo dessas rotas pesadas mantivesse uma excelente experiência de usuário e responsividade impecável no mobile.

---

## 📋 Demonstração da Engenharia de Processo (Exemplo Prático)

### A. Fluxo de Validação do Motor de Cálculo (BDD)
Para mapear o comportamento do motor de cálculo Java/Node que desenvolvi, utilizei a seguinte estrutura de cenários:

```gherkin
Funcionalidade: Processamento do Motor de Projeção Financeira

  Cenário: Processamento com sucesso de rodada complexa
    Dado que o motor de cálculo baseado em Java/Spring Boot recebeu a carga de dados da rodada
    Quando o endpoint de encerramento de turno for acionado pelo frontend React
    Então o backend deve executar as fórmulas matemáticas de projeção corporativa
    E persistir o novo estado consistente no banco de dados
    E retornar o payload JSON processado com HTTP Status 200 (OK) em tempo recorde.
