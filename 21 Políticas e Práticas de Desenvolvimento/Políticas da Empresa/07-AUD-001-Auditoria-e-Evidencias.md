---
policy_id: AUD-001
titulo: Rastreabilidade, Auditoria e Evidências
versao: 0.1.0
status: rascunho
obrigatoriedade: mandatory
enforcement: block
data_criacao: 2026-09-12
data_revisao: PENDENTE_DEFINICAO
responsavel: PENDENTE_DEFINICAO
tags: [politica, auditoria, evidencia, compliance]
---

# AUD-001 — Rastreabilidade, auditoria e evidências

## Objetivo

Permitir reconstruir o que aconteceu, por que aconteceu, quem autorizou e quais evidências sustentaram cada decisão relevante.

## Escopo

Aplica-se a ações humanas, ações de agentes, decisões, ferramentas, aprovações, exceções, políticas, incidentes e mudanças no projeto.

## Regras

1. Eventos relevantes devem registrar identidade, timestamp, origem, intenção, ação, resultado e decisão de autorização.
2. Fatos, inferências, recomendações, decisões e riscos devem ser diferenciados.
3. Logs não podem conter segredos ou dados pessoais desnecessários.
4. Políticas e exceções devem ser versionadas com autor, justificativa e validade.
5. Evidências devem estar vinculadas à tarefa e protegidas contra alteração não autorizada.
6. Ações críticas sem capacidade de auditoria devem ser bloqueadas.
7. O acesso às evidências deve respeitar a necessidade de conhecimento.

## Controles determinísticos

- event log append-only;
- schema de eventos;
- IDs de correlação;
- verificação de integridade;
- redação de dados sensíveis;
- controle de acesso e retenção.

## Evidências exigidas

- evento original e origem;
- versão da política aplicada;
- decisão do Policy Engine;
- registro de aprovação ou exceção;
- resultado da ação e verificações;
- relatório de integridade.

## Exceções

Uma exceção pode reduzir a coleta ao mínimo necessário, mas não pode eliminar a atribuição ou a autorização de ações críticas.

## Relações

[[02-SEC-002-Privacidade-e-Retencao]] · [[04-AGT-001-Acoes-e-Aprovacoes-de-Agentes]] · [[08-INC-001-Resposta-a-Incidentes]]

