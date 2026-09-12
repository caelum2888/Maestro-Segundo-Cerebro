---
tipo: schema
versao: 0.1.0
status: rascunho
tags: [schema, evento, agente]
---

# Schema mínimo de evento operacional

```json
{
  "event_id": "",
  "timestamp": "",
  "actor": {
    "type": "human | agent | service",
    "id": ""
  },
  "task_id": "",
  "event_type": "intent | plan | tool_call | change | test | decision | risk | handoff",
  "source": "",
  "scope": [],
  "summary": "",
  "evidence_refs": [],
  "authorization": {
    "decision": "allow | deny | require_approval",
    "policy_ids": [],
    "approval_id": null
  },
  "sensitivity": "public | internal | confidential | restricted"
}
```

Campos e enumerações devem ser validados fora do modelo antes da persistência.

