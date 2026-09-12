---
tipo: referencia
status: ativo
tags: [comandos, segundo-cerebro, agente]
---

# Comandos do Segundo Cérebro

## Conhecimento

- `/capturar [texto]` — cria uma nota atômica, classifica e sugere conexões.
- `/processar` — transforma itens da Inbox em notas permanentes.
- `/consultar [pergunta]` — responde citando notas internas.
- `/conectar [nota]` — sugere relações entre notas.
- `/revisar` — lista perguntas, riscos, decisões e bloqueios abertos.
- `/status` — apresenta o estado textual do projeto.
- `/mapa` — mostra áreas e conexões.
- `/exportar` — produz Markdown ou JSON estruturado.

## Governança

- `/decidir` — registra uma decisão.
- `/risco` — registra um risco.
- `/pergunta` — registra uma pergunta aberta.
- `/handoff` — resume estado, evidências, riscos e próximos passos.

## Segurança

- `/politica [id ou tema]` — consulta ou propõe nova versão de uma política.
- `/pratica [tema]` — registra ou consulta uma prática.
- `/validar-acao [contexto]` — avalia uma ação pelo Policy Engine.
- `/checklist [fase]` — seleciona o checklist aplicável.
- `/incidente [descrição]` — abre registro de incidente.
- `/auditoria [período]` — reúne eventos e exceções.
- `/excecao [política]` — solicita exceção temporária e aprovada.

## Formato de resposta

Toda resposta operacional deve separar, quando aplicável:

- **FATO** — sustentado por fonte.
- **INFERÊNCIA** — interpretação com confiança explícita.
- **RECOMENDAÇÃO** — ação proposta, ainda não decidida.
- **DECISÃO** — escolha autorizada e registrada.
- **RISCO** — evento incerto com impacto potencial.
- **PERGUNTA** — lacuna que exige resposta.

