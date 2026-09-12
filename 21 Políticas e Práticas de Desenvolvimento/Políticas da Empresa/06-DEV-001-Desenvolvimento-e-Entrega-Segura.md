---
policy_id: DEV-001
titulo: Desenvolvimento, Revisão e Entrega Segura
versao: 0.1.0
status: rascunho
obrigatoriedade: mandatory
enforcement: block
data_criacao: 2026-09-12
data_revisao: PENDENTE_DEFINICAO
responsavel: PENDENTE_DEFINICAO
tags: [politica, pratica, checklist, supply-chain, desenvolvimento]
---

# DEV-001 — Desenvolvimento, revisão e entrega segura

## Objetivo

Garantir que mudanças produzidas por humanos ou agentes sejam compreensíveis, revisáveis, testadas e acompanhadas de evidências.

## Escopo

Aplica-se a código, configuração, infraestrutura, dependências, pull requests, pipelines e releases.

## Regras

1. Toda mudança deve estar vinculada a uma tarefa, objetivo e critério de aceite.
2. Alterações de agentes devem ser atribuídas ao agente e ao responsável humano.
3. O diff deve ser revisável e limitado ao escopo solicitado.
4. Testes relevantes, análise estática, secret scanning e análise de dependências devem ocorrer antes do merge.
5. Dependências novas exigem justificativa, origem confiável, licença compatível e avaliação de risco.
6. Falha em teste obrigatório, verificação de segurança ou produção de evidência bloqueia a entrega.
7. Mudanças críticas exigem revisão humana independente.

## Definition of Done mínima

- critérios de aceite satisfeitos;
- revisão concluída;
- testes e verificações aprovados;
- documentação pertinente atualizada;
- evidências anexadas;
- riscos residuais registrados;
- plano de rollback definido quando necessário.

## Controles determinísticos

- proteção de branch;
- revisão obrigatória;
- gates no CI;
- SAST e secret scanner;
- análise de dependências e lockfile;
- verificação de testes e artefatos.

## Evidências exigidas

- referência da tarefa;
- pull request e revisão;
- relatórios de testes e segurança;
- inventário de dependências alteradas;
- risco residual e rollback.

## Relações

[[01-SEC-001-Gestao-de-Segredos]] · [[04-AGT-001-Acoes-e-Aprovacoes-de-Agentes]] · [[07-AUD-001-Auditoria-e-Evidencias]]

