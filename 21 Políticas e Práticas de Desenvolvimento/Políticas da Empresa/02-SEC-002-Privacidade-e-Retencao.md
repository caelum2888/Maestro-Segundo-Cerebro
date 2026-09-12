---
policy_id: SEC-002
titulo: Privacidade, Minimização e Retenção de Dados
versao: 0.1.0
status: rascunho
obrigatoriedade: mandatory
enforcement: block
data_criacao: 2026-09-12
data_revisao: PENDENTE_DEFINICAO
responsavel: PENDENTE_DEFINICAO
tags: [politica, privacidade, compliance, auditoria]
---

# SEC-002 — Privacidade, minimização e retenção

## Objetivo

Garantir que o Maestro colete apenas dados necessários, autorizados e transparentes, preservando a privacidade dos participantes.

## Escopo

Aplica-se a prompts, eventos, telemetria, arquivos, diffs, relatórios, históricos, evidências e dados armazenados no Segundo Cérebro.

## Regras

1. Toda categoria de dado deve ter finalidade, base de autorização, responsável e retenção definidos antes da coleta real.
2. O sistema deve observar atividades de trabalho, não pessoas.
3. É proibida a captura oculta de digitação, comunicação pessoal, credenciais ou conteúdo fora do projeto.
4. Participantes devem saber quais dados são coletados, por quê, onde ficam e quem pode acessá-los.
5. Dados pessoais e conteúdo sensível devem ser minimizados ou redigidos.
6. Deve existir processo para consulta, correção, exportação e exclusão quando aplicável.
7. Retenção indefinida é proibida. Os prazos ainda precisam de decisão formal.

## Controles determinísticos

- allowlist de campos coletáveis;
- redação automática;
- controle de acesso por papel;
- expiração e exclusão programadas;
- inventário de dados e trilha de consentimento.

## Evidências exigidas

- inventário de dados;
- registro de consentimento ou autorização;
- logs de retenção e exclusão;
- histórico de acesso a dados protegidos.

## Exceções

Exigem justificativa, finalidade, prazo e aprovação de `PENDENTE_DEFINICAO`. A exceção não pode autorizar vigilância oculta.

## Relações

[[00-RESUMO-GERAL]] · [[07-AUD-001-Auditoria-e-Evidencias]] · [[08-INC-001-Resposta-a-Incidentes]]

