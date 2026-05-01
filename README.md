# 📌 Projeto
 
## 📝 Sobre o Projeto

A **Central de Ocorrência Integrada (COI)** é um sistema web full-stack desenvolvido especificamente para modernizar as operações táticas e administrativas da Defesa Civil. 

* **Funcionalidade:** O sistema atua como o centro de comando digital da corporação. Ele centraliza a recepção de chamados dos munícipes, permite o despacho georreferenciado de viaturas no mapa e possibilita o acompanhamento em tempo real das equipes de campo. Através da plataforma, agentes e atendentes podem registrar dados, anexar evidências fotográficas in loco e gerar uma linha do tempo completa e auditável de cada atendimento.
* **Finalidade:** O grande objetivo do sistema é substituir métodos de registro manuais, físicos e descentralizados (como pranchetas, rádios analógicos e planilhas isoladas) por uma fonte única de verdade. A COI foi projetada para reduzir drasticamente o tempo de resposta a emergências, garantir a integridade dos dados durante situações de crise e otimizar o direcionamento de recursos públicos onde eles são mais necessários.

---

## 👥 Equipe

- **Artur Assis Guerra** — Full Stack Developer  
- **Eduardo Christianini Fonseca Junior** — Full Stack Developer  
- **Vanderson Guimarães da Silva** — Full Stack Developer  
- **Ícaro Lopes dos Santos Santana** — Full Stack Developer  

---

## 🚀 Tecnologias Utilizadas

### Frontend
- React
- Vite

### Backend
- Node.js
- TypeScript

### Banco de Dados
- PostgreSQL

---

## 📖 Objetivo

O objetivo deste projeto é desenvolver uma aplicação web completa, integrando frontend e backend, com foco em boas práticas de desenvolvimento, organização de código e escalabilidade.

---
## 🧑‍💻 Atores e Autenticação
O sistema conta com um módulo de Autenticação e Controle de Acesso (Login), garantindo que cada usuário acesse apenas as ferramentas do seu cargo.

* **Atendente (Base):** Autentica-se no painel da central. Realiza o primeiro contato, cadastra os dados do cidadão, categoriza o evento, define a localização no mapa e despacha a viatura.
* **Agente de Defesa Civil (Campo):** Autentica-se na interface de campo. Recebe o chamado, roteiriza o atendimento, enriquece a ocorrência com dados in loco (upload de fotos) e encerra o chamado.

## ⚙️ Funcionalidades Principais

* **Autenticação Segura:** Sistema de login individual para Atendentes e Agentes, com proteção de rotas e rastreabilidade de ações.
* **Cadastro de Munícipes:** Registro de dados do cidadão solicitante (nome, telefone, endereço, histórico de chamados).
* **Integração com Mapa (Geolocalização):** Visualização do local exato da ocorrência através de mapas interativos e visualização da distribuição de viaturas na cidade.
* **Gestão de Ocorrências e Acompanhamento:** Abertura, delegação de viaturas, encerramento de chamados e uma timeline cronológica do que acontece na ocorrência.
* **Enriquecimento Multimídia:** Upload e armazenamento de fotografias atreladas aos chamados para laudos técnicos visuais.
* **Gestão de Recursos:** Administração de Viaturas, Funcionários e Tipos de Ocorrência com integridade referencial nativa no banco de dados.
* **Dashboard Operacional:** Visualização clara do fluxo de trabalho para identificar rapidamente ocorrências pendentes e equipes em operação.

## 🔒 Requisitos Não Funcionais & Segurança
* **Responsividade (Mobile-First):** Interface do Agente otimizada para uso em smartphones no campo, enquanto o painel do Atendente é focado em navegação desktop.
* **Segurança e LGPD:** Criptografia de senhas (Bcrypt) e proteção de rotas (JWT), garantindo a privacidade dos dados pessoais dos munícipes cadastrados.
* **Resiliência a Falhas (Offline-First para Agentes):** Capacidade de salvar laudos e fotos localmente no dispositivo do agente caso haja queda de internet em áreas de desastre, sincronizando automaticamente com o PostgreSQL quando a conexão for reestabelecida.

## 📱 Notificações e Mensageria
* **Alertas de Status:** Atualizações no painel para que os Atendentes saibam instantaneamente quando um Agente chega ao local ou finaliza uma ocorrência.

## 🛠️ Ferramentas de Engenharia & Gestão
* **Metodologia Ágil:** Gestão de tarefas, Sprints e Backlog conduzidas através de metodologias ágeis (Scrum/Kanban).
* **Prototipagem (UI/UX):** Telas e fluxos de navegação desenhados no Figma antes do desenvolvimento.
