---
tipo: mapa-de-conteudo
status: ativo
tags: [agente, guardrail, aprovacao]
---

# Guardrails para agentes

## Regra central

Agentes podem analisar e executar apenas ações autorizadas, limitadas e verificáveis. O modelo recomenda; controles determinísticos autorizam ou bloqueiam.

## Classes de ação

| Classe | Exemplos | Tratamento |
| --- | --- | --- |
| G0 — Leitura | Ler arquivos autorizados, consultar estado | Permitir e registrar |
| G1 — Reversível | Editar workspace, executar testes | Permitir com escopo, diff e limite |
| G2 — Consequencial | Commit, PR, comunicação interna | Política específica e evidência |
| G3 — Crítica | Merge, deploy, produção, exclusão, segredo | Aprovação humana obrigatória |
| GX — Proibida | Vigilância oculta, exfiltração, autoelevação | Bloquear e alertar |

## Condições mínimas antes de uma ferramenta

- identidade conhecida;
- objetivo e escopo definidos;
- ferramenta permitida;
- argumentos validados;
- recursos e ambiente autorizados;
- impacto classificado;
- aprovação presente quando exigida;
- capacidade de registrar resultado.

## Políticas relacionadas

- [[../21 Políticas e Práticas de Desenvolvimento/Políticas da Empresa/04-AGT-001-Acoes-e-Aprovacoes-de-Agentes|AGT-001]]
- [[../21 Políticas e Práticas de Desenvolvimento/Políticas da Empresa/05-AGT-002-Prompt-Injection|AGT-002]]
- [[../21 Políticas e Práticas de Desenvolvimento/Políticas da Empresa/03-SEC-003-Identidade-e-Acesso|SEC-003]]

