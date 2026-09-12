---
policy_id: SEC-001
titulo: Gestão de Segredos
versao: 0.1.0
status: rascunho
obrigatoriedade: mandatory
enforcement: block
data_criacao: 2026-09-12
data_revisao: PENDENTE_DEFINICAO
responsavel: PENDENTE_DEFINICAO
tags: [politica, segredo, cybersecurity, menor-privilegio]
---

# SEC-001 — Gestão de Segredos

## Objetivo

Impedir que credenciais, tokens, chaves, certificados ou informações equivalentes sejam expostos, copiados ou utilizados fora do propósito autorizado.

## Escopo

Aplica-se a colaboradores, agentes de IA, serviços, repositórios, prompts, logs, notas, relatórios, pipelines e ambientes do projeto Maestro.

## Regras

1. Segredos nunca devem ser incluídos em prompts, código, commits, issues, logs, relatórios ou notas.
2. Segredos devem ser armazenados somente em cofre autorizado pela empresa.
3. Código e configuração devem referenciar identificadores ou variáveis, nunca valores secretos.
4. Eventos e saídas devem ser redigidos antes da persistência.
5. Agentes não podem listar, copiar ou transmitir segredos sem autorização específica e necessidade comprovada.
6. Exposição confirmada exige interrupção da ação, preservação de evidência, revogação e substituição do segredo.

## Controles determinísticos

- scanner de segredos em pre-commit e CI;
- mecanismo de redação de logs e eventos;
- controle de acesso ao cofre;
- bloqueio de commits com segredo detectado;
- registro de acessos ao cofre.

## Evidências exigidas

- relatório do scanner;
- registro de redação;
- log de acesso ao cofre;
- registro de revogação quando houver exposição.

## Exceções

Exigem justificativa, duração limitada e aprovação de `PENDENTE_DEFINICAO`. Não é permitido abrir exceção para armazenar segredo em texto simples.

## Relações

[[03-SEC-003-Identidade-e-Acesso]] · [[07-AUD-001-Auditoria-e-Evidencias]] · [[08-INC-001-Resposta-a-Incidentes]]

