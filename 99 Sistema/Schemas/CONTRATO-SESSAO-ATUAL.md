# Contrato — `sessao-atual.md`

O monitor usa o arquivo `sessao-atual.md`, localizado na raiz do vault configurado em `VAULT_PATH`.

## Estrutura obrigatória

O arquivo deve conter exatamente estes cinco títulos de segundo nível, preservando grafia e acentos:

1. `## Objetivo`
2. `## Ações`
3. `## Riscos`
4. `## Bloqueios`
5. `## Status`

O conteúdo de cada seção aceita texto livre, listas e múltiplas linhas. Frontmatter YAML é opcional. Não renomeie os títulos, pois `ler_estado()` depende deles para separar os campos.

O monitor verifica alterações periodicamente e pode emitir notificações no Telegram. Não inclua segredos, credenciais ou dados pessoais desnecessários nessa nota.

## Fluxo de atualização

1. Atualize o objetivo corrente.
2. Registre apenas ações já realizadas.
3. Registre riscos e bloqueios ou use `Nenhum`.
4. Atualize o status.
5. Salve o arquivo e aguarde o ciclo do monitor.

Para evitar conflitos, mantenha apenas um responsável por editar `sessao-atual.md` em cada sessão operacional.

