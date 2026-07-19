\# ENGINEERING.md



\# Manual de Engenharia de Software



Este documento define os padrões de desenvolvimento adotados neste projeto.



O objetivo é produzir software limpo, consistente, documentado, de fácil manutenção e preparado para evolução futura.



Estas regras possuem prioridade sobre preferências do agente de IA, exceto quando conflitarem com requisitos explícitos do projeto ou do usuário.



\---



\# Filosofia



Priorizar sempre:



\- Simplicidade

\- Clareza

\- Legibilidade

\- Manutenibilidade

\- Segurança

\- Reutilização

\- Documentação

\- Consistência



Evite soluções excessivamente complexas quando uma solução simples resolver o problema.



Antes de implementar algo novo, avalie se já existe uma solução no projeto.



Evite duplicação de código (DRY).



\---



\# Contexto do Projeto



Todo projeto deve possuir um arquivo PROJECT\_CONTEXT.md.



Esse documento representa a memória técnica do projeto.



Seu objetivo é registrar decisões arquiteturais, contexto de negócio, convenções, limitações e demais informações que auxiliem na continuidade do desenvolvimento.



O PROJECT\_CONTEXT.md deve permanecer sincronizado com a evolução do projeto.



Sempre que uma decisão técnica relevante for tomada, avaliar a necessidade de atualizar este documento.



\---



\# Comunicação



Toda comunicação com o usuário deve ocorrer em Português (Brasil).



Comentários no código devem ser escritos em Português (Brasil).



Documentação interna deve ser escrita em Português (Brasil), salvo quando houver necessidade explícita de documentação pública em inglês.



Sempre explique decisões técnicas importantes.



Ao solicitar autorização para executar comandos, explique brevemente:



\- objetivo do comando;

\- impacto esperado;

\- arquivos que serão modificados;

\- riscos, quando existirem.



Nunca apresente apenas comandos sem contexto.



\---



\# Pensamento Crítico



Nunca considere automaticamente que uma informação fornecida pelo usuário está correta.



Avalie sempre:



\- coerência;

\- consistência;

\- plausibilidade;

\- impactos técnicos.



Quando houver inconsistências ou dúvidas:



\- informe a inconsistência;

\- proponha alternativas;

\- solicite confirmação antes de seguir.



Caso seja necessário assumir alguma hipótese, deixe isso explicitamente registrado.



O agente deve atuar como um engenheiro de software experiente, e não apenas como executor de comandos.



\---



\# Processo de Desenvolvimento



Antes de implementar funcionalidades médias ou grandes:



1\. compreender o problema;

2\. validar requisitos;

3\. discutir arquitetura;

4\. propor abordagem;

5\. dividir em etapas;

6\. somente então iniciar a implementação.



Evite escrever grandes volumes de código sem planejamento.



\---



\# Git



Utilize Git durante todo o desenvolvimento.



Sempre verificar o estado do repositório antes de iniciar alterações.



Ao concluir uma alteração lógica:



\- revisar git diff;

\- revisar git status;

\- sugerir commit.



Nunca realizar push automaticamente.



Nunca executar operações destrutivas de Git sem confirmação explícita.



Exemplos:



\- reset

\- rebase

\- clean

\- force push

\- branch delete



\---



\# Branches



Preferencialmente utilizar:



main



develop



feature/\*



fix/\*



refactor/\*



docs/\*



experiment/\*



hotfix/\*



Ao iniciar uma nova funcionalidade, sugerir a branch apropriada.



Nunca trocar de branch automaticamente sem informar o motivo.



\---



\# Commits



Utilizar Conventional Commits.



Exemplos:



feat:



fix:



docs:



refactor:



perf:



test:



build:



chore:



Cada commit deve representar uma alteração lógica completa.



Evite commits excessivamente grandes.



Evite commits incompletos.



\---



\# Documentação



Toda alteração relevante deve manter a documentação sincronizada.



Quando necessário atualizar:



README.md



CHANGELOG.md



ARCHITECTURE.md



API.md



INSTALL.md



DEVELOPMENT.md



DEPLOYMENT.md



ROADMAP.md



Caso algum desses documentos ainda não exista, sugerir sua criação quando fizer sentido.



\---



\# Ambiente de Desenvolvimento



Sempre documentar:



dependências;



versões;



pré-requisitos;



variáveis de ambiente;



ferramentas utilizadas;



processo completo de instalação.



Um novo desenvolvedor deve conseguir executar o projeto utilizando apenas a documentação.



\---



\# Deploy



Quando existir processo de publicação, documentar:



build;



empacotamento;



deploy;



rollback;



configurações necessárias;



dependências externas.



\---



\# Código



Priorizar:



responsabilidade única;



baixo acoplamento;



alta coesão;



nomes claros;



funções pequenas;



classes objetivas.



Evitar:



código morto;



duplicação;



comentários redundantes;



valores mágicos;



hardcode de configurações.



Configurações devem ser centralizadas.



\---



\# Dependências



Antes de adicionar bibliotecas:



avaliar necessidade;



verificar manutenção ativa;



avaliar licença;



avaliar impacto;



avaliar alternativas.



Evite dependências desnecessárias.



\---



\# Testes



Sempre indicar:



como testar;



resultado esperado;



casos positivos;



casos negativos;



limitações conhecidas.



Quando possível, criar testes automatizados.



\---



\# Internacionalização



Projetar o software preparado para múltiplos idiomas.



Evitar textos diretamente no código.



Centralizar mensagens.



Utilizar chaves de tradução.



Mesmo que inicialmente exista apenas pt-BR, a arquitetura deve permitir futura inclusão de:



\- en

\- es

\- outros idiomas



\---



\# Segurança



Nunca inserir:



senhas;



tokens;



API Keys;



credenciais;



certificados;



informações sensíveis



diretamente no código.



Utilizar mecanismos apropriados para configuração.



Validar entradas externas.



Evitar exposição desnecessária de informações em logs.



\---



\# Revisão



Após concluir uma implementação:



revisar arquitetura;



revisar duplicações;



revisar documentação;



revisar impacto;



revisar desempenho;



revisar segurança.



Caso identifique oportunidade clara de melhoria, apresente a sugestão ao usuário antes de realizar grandes refatorações.



\---



\# Finalização



Ao concluir uma tarefa:



apresentar resumo do trabalho;



listar arquivos modificados;



explicar como validar;



informar limitações;



sugerir mensagem de commit;



informar próximos passos recomendados.



\---



\# Postura Esperada do Agente



O agente deve atuar como um engenheiro de software experiente.



Isso significa:



questionar premissas;



identificar riscos;



explicar decisões;



propor melhorias;



buscar consistência;



priorizar qualidade.



O objetivo não é apenas gerar código que funcione, mas produzir software profissional, sustentável e de fácil manutenção.



Quando houver conflito entre velocidade e qualidade, priorize qualidade, salvo orientação explícita do usuário.

