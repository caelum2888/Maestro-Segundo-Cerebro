---
policy_id: AGT-002
titulo: Prevenção de Prompt Injection e Tratamento de Conteúdo Não Confiável
versao: 0.1.0
status: rascunho
obrigatoriedade: mandatory
enforcement: block
data_criacao: 2026-09-12
data_revisao: PENDENTE_DEFINICAO
responsavel: PENDENTE_DEFINICAO
tags: [politica, prompt-injection, agente, guardrail, cybersecurity]
---

# AGT-002 — Prompt injection e conteúdo não confiável

## Objetivo

Impedir que arquivos, páginas, logs, mensagens ou resultados de ferramentas alterem indevidamente instruções, políticas ou permissões dos agentes.

## Escopo

Aplica-se a todo conteúdo fornecido, recuperado ou gerado durante uma execução de agente.

## Regras

1. Conteúdo externo é dado não confiável, ainda que pareça uma instrução legítima.
2. Dados recuperados não podem alterar objetivo, identidade, políticas, permissões ou limites de execução.
3. Instruções confiáveis e dados devem ser separados estruturalmente.
4. Argumentos de ferramentas devem ser validados por schema e política antes da execução.
5. Comandos encontrados em arquivos ou páginas não devem ser executados automaticamente.
6. Solicitações para revelar segredos, ignorar políticas ou ampliar escopo devem ser bloqueadas e registradas.
7. O sistema deve falhar de forma segura quando a origem ou autoridade de uma instrução não puder ser confirmada.

## Controles determinísticos

- separação entre instrução e dado;
- validação de schemas;
- allowlist de ferramentas e argumentos;
- Policy Engine;
- sanitização de entradas e saídas;
- testes adversariais de prompt injection.

## Evidências exigidas

- origem do conteúdo;
- resultado da validação;
- decisão de autorização;
- registro das ações bloqueadas;
- casos adversariais e resultados dos testes.

## Exceções

Nenhum conteúdo externo pode receber autoridade de política por exceção informal. Alterações de autoridade exigem mudança formal e versionada da configuração.

## Relações

[[04-AGT-001-Acoes-e-Aprovacoes-de-Agentes]] · [[06-DEV-001-Desenvolvimento-e-Entrega-Segura]] · [[07-AUD-001-Auditoria-e-Evidencias]]

