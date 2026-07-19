# Claude Workspace

Antes de qualquer atividade, leia [.claude/ENGINEERING.md](.claude/ENGINEERING.md). Ele contém os padrões de engenharia obrigatórios deste projeto e tem prioridade sobre preferências do agente.

## Governança do projeto

- **Diretrizes de engenharia**: [.claude/ENGINEERING.md](.claude/ENGINEERING.md)
- **Memória técnica do projeto**: [PROJECT_CONTEXT.md](PROJECT_CONTEXT.md) — atualize sempre que uma decisão técnica relevante for tomada.
- **Agentes disponíveis** (invocáveis via ferramenta Agent):
  - `architect` ([.claude/agents/architect.md](.claude/agents/architect.md)) — consulte antes de decisões arquiteturais.
  - `reviewer` ([.claude/agents/reviewer.md](.claude/agents/reviewer.md)) — consulte antes de concluir qualquer tarefa.
- **Skills disponíveis** (invocáveis via ferramenta Skill): planning, implementation, debugging, documentation, git, release. Listadas em [.claude/skills/](.claude/skills/).

## Regras de operação

- Utilize as skills sempre que forem aplicáveis. Quando uma tarefa envolver múltiplas áreas, combine as skills necessárias.
- Quando existir dúvida arquitetural, consulte o agente `architect`.
- Antes de concluir qualquer tarefa, consulte o agente `reviewer`.
- Nunca ignore as diretrizes do [ENGINEERING.md](.claude/ENGINEERING.md).
- Sempre que forem adicionados ou alterados arquivos de governança (ENGINEERING.md, PROJECT_CONTEXT.md, skills ou agents), realize uma revisão de conformidade antes de continuar o desenvolvimento.
