---
policy_id: AGT-001
titulo: Ações, Autonomia e Aprovações de Agentes
versao: 0.1.0
status: rascunho
obrigatoriedade: mandatory
enforcement: block
data_criacao: 2026-09-12
data_revisao: PENDENTE_DEFINICAO
responsavel: PENDENTE_DEFINICAO
tags: [politica, agente, guardrail, aprovacao, gate]
---

# AGT-001 — Ações, autonomia e aprovações de agentes

## Objetivo

Definir limites claros para agentes de IA e garantir supervisão humana proporcional ao impacto de cada ação.

## Escopo

Aplica-se ao agente Maestro, agentes executores, ferramentas delegadas e automações associadas.

## Ações permitidas inicialmente

- ler e analisar recursos expressamente colocados no escopo;
- propor planos, mudanças, testes e correções;
- criar alterações reversíveis no workspace quando solicitadas;
- executar verificações locais autorizadas;
- produzir relatórios com fatos, inferências, riscos e recomendações separados.

## Ações que exigem aprovação humana

- merge ou deploy;
- acesso ou alteração em produção;
- exclusão ou alteração destrutiva;
- modificação de permissões;
- acesso, revogação ou rotação de segredos;
- comunicação externa em nome da empresa;
- aquisição, contratação ou ação com impacto financeiro;
- exceção a qualquer política obrigatória.

## Regras

1. O Maestro pode observar eventos autorizados, recomendar, alertar e solicitar aprovação; não pode vigiar pessoas ou agir silenciosamente em seu nome.
2. Toda ferramenta deve possuir escopo, timeout, limite de tentativas e comportamento de falha.
3. Loops e concorrência ilimitados são proibidos.
4. Mudanças devem gerar diff e evidência de verificação.
5. Falha de autorização, contexto ou rastreabilidade resulta em bloqueio e escalonamento.

## Controles determinísticos

- allowlist de ferramentas;
- Policy Engine externo ao modelo;
- gates de aprovação;
- sandbox;
- timeout, retries limitados e idempotência;
- limites de concorrência e custo.

## Evidências exigidas

- escopo da tarefa;
- identidade do agente e responsável humano;
- chamadas de ferramentas;
- aprovação quando aplicável;
- diff, testes e resultado final.

## Relações

[[03-SEC-003-Identidade-e-Acesso]] · [[05-AGT-002-Prompt-Injection]] · [[07-AUD-001-Auditoria-e-Evidencias]]

