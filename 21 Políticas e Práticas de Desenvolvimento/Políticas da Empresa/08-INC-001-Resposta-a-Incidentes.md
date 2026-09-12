---
policy_id: INC-001
titulo: Resposta a Incidentes de Segurança e Agentes
versao: 0.1.0
status: rascunho
obrigatoriedade: mandatory
enforcement: block
data_criacao: 2026-09-12
data_revisao: PENDENTE_DEFINICAO
responsavel: PENDENTE_DEFINICAO
tags: [politica, incidente, cybersecurity, auditoria]
---

# INC-001 — Resposta a incidentes

## Objetivo

Conter incidentes, proteger pessoas e ativos, preservar evidências e restabelecer operações de forma autorizada e verificável.

## Escopo

Aplica-se a incidentes de segurança, privacidade, acesso indevido, exposição de segredos, comportamento inesperado de agentes e falhas de guardrails.

## Fluxo obrigatório

1. **Detectar:** registrar o sinal e sua origem.
2. **Conter:** interromper ações relacionadas e reduzir exposição.
3. **Preservar:** proteger logs, diffs, decisões e outras evidências.
4. **Classificar:** avaliar impacto e severidade com base em fatos disponíveis.
5. **Notificar:** acionar o responsável humano ainda a ser definido.
6. **Erradicar:** remover acesso, segredo, configuração ou causa confirmada.
7. **Recuperar:** restaurar de forma controlada e verificar o resultado.
8. **Aprender:** registrar causa, decisões, melhorias e risco residual.

## Regras

1. Não declarar comprometimento sem evidência suficiente.
2. Não apagar ou modificar evidências relevantes.
3. Credenciais confirmadas como expostas devem ser revogadas e substituídas.
4. Agentes relacionados ao incidente devem perder temporariamente a capacidade de ações críticas.
5. A retomada exige aprovação humana e evidência de contenção.

## Controles determinísticos

- botão ou mecanismo de parada de emergência;
- revogação de credenciais;
- preservação de evidências;
- workflow de incidentes;
- gate de recuperação;
- monitoramento após retomada.

## Evidências exigidas

- registro e linha do tempo do incidente;
- ações de contenção;
- identidades e aprovações;
- evidência de recuperação;
- revisão pós-incidente.

## Relações

[[01-SEC-001-Gestao-de-Segredos]] · [[02-SEC-002-Privacidade-e-Retencao]] · [[07-AUD-001-Auditoria-e-Evidencias]]
