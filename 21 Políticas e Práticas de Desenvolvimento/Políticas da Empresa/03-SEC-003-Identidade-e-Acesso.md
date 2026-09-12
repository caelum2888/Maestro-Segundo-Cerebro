---
policy_id: SEC-003
titulo: Identidade, Controle de Acesso e Menor Privilégio
versao: 0.1.0
status: rascunho
obrigatoriedade: mandatory
enforcement: block
data_criacao: 2026-09-12
data_revisao: PENDENTE_DEFINICAO
responsavel: PENDENTE_DEFINICAO
tags: [politica, menor-privilegio, zero-trust, aprovacao]
---

# SEC-003 — Identidade, acesso e menor privilégio

## Objetivo

Garantir que cada pessoa, agente ou serviço tenha somente o acesso necessário para a tarefa, pelo menor tempo possível.

## Escopo

Aplica-se a desenvolvedores, líderes técnicos, administradores, agentes, serviços, repositórios, ferramentas e ambientes.

## Regras

1. Toda ação relevante deve estar associada a identidade verificável.
2. Permissões devem ser limitadas por tarefa, recurso, ambiente e duração.
3. Ausência de autorização explícita resulta em negação.
4. Agentes não podem elevar seus próprios privilégios ou editar regras de autorização.
5. Contas compartilhadas são proibidas para ações críticas.
6. Privilégios devem ser revistos quando a função, a tarefa ou o vínculo terminar.
7. Acesso administrativo exige autenticação reforçada e evidência auditável.

## Controles determinísticos

- provedor de identidade;
- RBAC ou ABAC;
- tokens com escopo e duração limitados;
- negação por padrão;
- revisão periódica de permissões;
- autenticação multifator para acessos críticos.

## Evidências exigidas

- identidade da parte executora;
- decisão de autorização;
- registro de acesso;
- histórico de concessão e revogação;
- resultado da revisão de permissões.

## Exceções

Exigem aprovação de `PENDENTE_DEFINICAO`, prazo de validade e remoção automática ao término.

## Relações

[[01-SEC-001-Gestao-de-Segredos]] · [[04-AGT-001-Acoes-e-Aprovacoes-de-Agentes]] · [[07-AUD-001-Auditoria-e-Evidencias]]

