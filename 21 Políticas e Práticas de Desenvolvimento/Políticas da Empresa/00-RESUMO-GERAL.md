---
documento: resumo-de-politicas
projeto: Maestro — Plataforma de Orquestração Humano–IA
versao: 0.1.0
status: rascunho
data_criacao: 2026-09-12
responsavel: PENDENTE_DEFINICAO
tags: [politica, cybersecurity, compliance, agentes, empresa]
---

# Resumo geral das políticas da empresa

## Finalidade

Este conjunto estabelece as regras mínimas para pessoas, agentes de IA, serviços e ferramentas que trabalham no projeto **Maestro — Plataforma de Orquestração Humano–IA**. Seu objetivo é permitir colaboração produtiva com supervisão humana, segurança por padrão, privacidade, rastreabilidade e capacidade de recuperação.

Estas políticas estão em **rascunho**. Tornam-se normativas após definição dos responsáveis, aprovação formal e implementação dos controles indicados.

## Princípios obrigatórios

1. Evidência antes de conclusão.
2. Menor privilégio e acesso limitado à tarefa.
3. Negação por padrão quando não houver autorização.
4. Controles críticos aplicados fora do modelo de linguagem.
5. Conteúdo externo tratado como dado não confiável.
6. Coleta mínima, transparente e consentida.
7. Supervisão do trabalho, nunca vigilância de pessoas.
8. Ações relevantes vinculadas a identidade e evidência.
9. Ações críticas exigem aprovação humana.
10. Falhas de autorização, contexto ou auditoria resultam em bloqueio seguro.

## Catálogo

| ID | Política | Objetivo | Enforcement |
| --- | --- | --- | --- |
| [SEC-001](01-SEC-001-Gestao-de-Segredos.md) | Gestão de segredos | Impedir exposição e uso indevido de credenciais | Bloquear |
| [SEC-002](02-SEC-002-Privacidade-e-Retencao.md) | Privacidade e retenção | Limitar coleta, uso e permanência dos dados | Bloquear |
| [SEC-003](03-SEC-003-Identidade-e-Acesso.md) | Identidade e acesso | Aplicar menor privilégio e negação por padrão | Bloquear |
| [AGT-001](04-AGT-001-Acoes-e-Aprovacoes-de-Agentes.md) | Ações de agentes | Delimitar autonomia e aprovações | Bloquear |
| [AGT-002](05-AGT-002-Prompt-Injection.md) | Prompt injection | Separar instruções confiáveis de dados externos | Bloquear |
| [DEV-001](06-DEV-001-Desenvolvimento-e-Entrega-Segura.md) | Entrega segura | Exigir revisão, testes e evidências | Bloquear |
| [AUD-001](07-AUD-001-Auditoria-e-Evidencias.md) | Auditoria | Manter decisões e ações rastreáveis | Bloquear |
| [INC-001](08-INC-001-Resposta-a-Incidentes.md) | Incidentes | Conter, investigar e recuperar com segurança | Bloquear |

## Matriz resumida de ações

| Ação | Regra inicial |
| --- | --- |
| Leitura de arquivos do projeto | Permitida dentro do escopo autorizado |
| Análise e recomendação | Permitida, com origem e confiança registradas |
| Alteração reversível no workspace | Permitida quando explicitamente solicitada e verificável por diff |
| Commit ou abertura de PR | Exige atribuição, testes e política do repositório |
| Merge, deploy ou acesso à produção | Exige aprovação humana explícita |
| Exclusão, mudança de permissões ou rotação de segredo | Exige aprovação humana explícita |
| Comunicação externa em nome da empresa | Exige aprovação humana explícita |
| Ação sem identidade, escopo ou trilha de auditoria | Bloqueada |

## Decisões necessárias antes da vigência

- Nomear o responsável pelas políticas.
- Nomear o aprovador de exceções e ações críticas.
- Definir dados permitidos e proibidos.
- Definir retenção por categoria de dado.
- Confirmar normas aplicáveis, incluindo LGPD quando pertinente.
- Escolher cofre de segredos e ferramentas de SAST, DAST e análise de dependências.
- Definir autonomia dos agentes em desenvolvimento, homologação e produção.
- Definir canal e responsável por incidentes.

Até essas decisões serem registradas, ações críticas permanecem **bloqueadas por padrão**.
