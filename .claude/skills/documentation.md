---
name: documentation
description: Use para avaliar se uma alteração exige atualização de documentação. Foca em README, CHANGELOG, INSTALL, DEVELOPMENT, DEPLOYMENT, ARCHITECTURE, API, ROADMAP e principalmente PROJECT_CONTEXT.md, que é a memória técnica do projeto.
---

Toda alteração deve avaliar necessidade de atualizar documentação.

Quando necessário atualizar:

- `README.md`
- `CHANGELOG.md`
- `INSTALL.md`
- `DEVELOPMENT.md`
- `DEPLOYMENT.md`
- `ARCHITECTURE.md`
- `API.md`
- `ROADMAP.md`

Se algum documento estiver ausente, sugerir sua criação.

Sempre garantir que um novo desenvolvedor consiga instalar e executar o projeto apenas utilizando a documentação.

## PROJECT_CONTEXT.md

Sempre avaliar se a alteração realizada exige atualização do `PROJECT_CONTEXT.md`.

O `PROJECT_CONTEXT.md` deve conter apenas informações específicas do projeto.

Atualizar sempre que houver:

- decisões arquiteturais importantes;
- mudança de tecnologias;
- criação de módulos relevantes;
- mudança na estrutura do projeto;
- novas convenções;
- limitações conhecidas;
- dívidas técnicas relevantes;
- integrações externas;
- decisões cujo motivo seja importante preservar.

Evitar registrar informações temporárias.

Evitar duplicar conteúdo existente no README.

O objetivo do `PROJECT_CONTEXT.md` é servir como memória técnica do projeto.

Sempre que uma decisão técnica importante for tomada, registrar não apenas a decisão, mas também o motivo pelo qual ela foi escolhida e, quando relevante, as alternativas consideradas.
