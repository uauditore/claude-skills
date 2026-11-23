# Skills para Claude Code

32 skills prontas para usar no [Claude Code](https://claude.com/claude-code). Uma skill é uma pasta com um `SKILL.md` que ensina o Claude a fazer um tipo de tarefa de um jeito específico. O Claude carrega a skill sozinho quando o pedido combina com a descrição dela, ou você chama na mão com `/nome-da-skill`.

## Como instalar

1. Clone o repositório ou baixe o zip (botão **Code → Download ZIP**).
2. Copie as pastas que quiser para `~/.claude/skills/` (no Windows, `C:\Users\<voce>\.claude\skills\`).
3. Reinicie o Claude Code.

Cada pasta tem o arquivo `LICENSE` do autor original e um `ORIGEM.md` ou `INSTALL-NOTE.md` dizendo de onde veio.

---

## Design de interface

| Skill | O que faz |
|---|---|
| **frontend-design** | Dá direção estética a uma interface nova ou redesenhada: tipografia, composição e escolhas que não parecem template genérico. |
| **impeccable** | Kit completo de design de produto: criar, criticar, auditar, polir, simplificar e endurecer telas (web e mobile). Cobre hierarquia, layout, cor, tipografia, microcopy, responsivo e casos de borda. Também documenta design systems (DESIGN.md, tokens). |
| **prototype** | Gera várias versões bem diferentes de um mesmo componente e mostra com um seletor visual, para você trocar entre elas ao vivo e escolher a melhor. Só roda quando chamada. |
| **break-ui** | Tenta quebrar uma tela com dados de pior caso (nomes enormes, e-mails sem quebra, campos vazios, números extremos, emoji, texto não latino) e lista tudo que quebrou, com a correção. |
| **web-interface-guidelines** | Revisa código de UI contra as Web Interface Guidelines da Vercel: foco, formulários, animação, tipografia, imagens, performance, navegação, toque, modo escuro e i18n. |
| **accessibility** | Auditoria e correção de acessibilidade seguindo a WCAG 2.2: leitor de tela, navegação por teclado, contraste, semântica e ARIA. |

## Animação e motion

| Skill | O que faz |
|---|---|
| **animate** | Constrói uma animação do zero na ordem certa de decisões: se deve animar, com que propósito, qual ferramenta, quais propriedades, curva, duração, interrupção e saída. Escreve o código. |
| **find-animation-opportunities** | Procura no código ou na tela lugares que deveriam animar e não animam, e descarta o que não deveria. Só sugere, com valores exatos. |
| **improve-animations** | Audita todo o motion de um projeto e entrega uma lista priorizada, com planos de implementação que outro agente consegue executar. Não altera o código. |
| **review-animations** | Revisão exigente de código de animação, baseada na filosofia de design engineering do Emil Kowalski. Aprova pouco e aponta muito. |

## Processo de desenvolvimento (Superpowers)

Estas 15 vêm do plugin **Superpowers** e funcionam melhor juntas. Se quiser o conjunto completo, com o hook que as ativa no começo de cada sessão, instale o plugin pelo marketplace oficial: `/plugin install superpowers@claude-plugins-official`.

| Skill | O que faz |
|---|---|
| **using-superpowers** | Ponto de entrada: ensina o Claude a procurar e usar as skills antes de responder qualquer coisa. |
| **brainstorming** | Antes de criar qualquer coisa, conduz uma conversa para entender o objetivo, explorar alternativas e fechar um desenho antes de começar. |
| **writing-plans** | Transforma uma especificação em um plano de implementação passo a passo, antes de tocar no código. |
| **executing-plans** | Executa um plano de implementação na própria sessão, tarefa por tarefa, com pontos de verificação. |
| **subagent-driven-development** | Executa um plano despachando um subagente por tarefa independente, com revisão entre elas. |
| **dispatching-parallel-agents** | Quando há duas ou mais tarefas independentes, divide entre agentes que trabalham em paralelo. |
| **test-driven-development** | Obriga o ciclo TDD: escrever o teste que falha, depois o código mínimo, depois refatorar. |
| **systematic-debugging** | Método para investigar bugs e testes quebrados: reproduzir, isolar e achar a causa raiz antes de propor correção. |
| **verification-before-completion** | Antes de dizer que algo está pronto ou corrigido, exige rodar os comandos de verificação e mostrar a evidência. |
| **requesting-code-review** | Prepara e pede revisão de código ao terminar uma tarefa ou antes de fazer merge. |
| **receiving-code-review** | Como receber feedback de revisão: verificar tecnicamente cada ponto antes de aceitar ou rebater, sem concordar no automático. |
| **using-git-worktrees** | Cria um espaço de trabalho isolado (git worktree) antes de começar uma feature ou executar um plano. |
| **finishing-a-development-branch** | Quando a implementação está pronta e os testes passam, ajuda a decidir como integrar: merge, PR ou limpeza. |
| **writing-skills** | Como criar, editar e testar skills novas para que funcionem de verdade. |
| **diagnosing-superpowers** | Quando uma sessão com Superpowers deu errado (repetição, plano ignorado, custo alto), investiga o porquê e monta um relatório. |

## Obsidian

| Skill | O que faz |
|---|---|
| **obsidian-markdown** | Escreve Markdown no padrão do Obsidian: wikilinks, embeds, callouts, propriedades e tags. |
| **obsidian-bases** | Cria e edita Obsidian Bases (`.base`): visões de tabela e cartões, filtros, fórmulas e resumos. |
| **json-canvas** | Cria e edita arquivos JSON Canvas (`.canvas`): mapas mentais, fluxogramas, nós, grupos e conexões. |
| **obsidian-cli** | Usa o Obsidian CLI para ler, criar, buscar e organizar notas de um cofre, e para desenvolver plugins e temas. |
| **defuddle** | Extrai o conteúdo limpo de uma página web em Markdown, sem menus e anúncios, para economizar tokens. Precisa do CLI `defuddle`. |

## Outras

| Skill | O que faz |
|---|---|
| **skill-creator** | Cria skills do zero, melhora skills existentes e mede o desempenho delas com testes e benchmarks. |
| **graphify** | Transforma código, documentos, artigos ou imagens num grafo de conhecimento persistente, com consultas de caminho, comunidades e nós centrais. Precisa de Python; na primeira vez a skill instala o pacote `graphifyy` via `uv`. |

---

## Créditos e licenças

- Emil Kowalski ([emilkowalski/skill](https://github.com/emilkowalski/skill)), MIT: animate, break-ui, find-animation-opportunities, improve-animations, prototype, review-animations.
- Addy Osmani ([addyosmani/web-quality-skills](https://github.com/addyosmani/web-quality-skills)), MIT: accessibility.
- Jesse Vincent ([obra/superpowers](https://github.com/obra/superpowers)), MIT: as 15 skills do Superpowers.
- Steph Ango ([kepano/obsidian-skills](https://github.com/kepano/obsidian-skills)), MIT: as 5 skills do Obsidian.
- Anthropic, Apache 2.0: frontend-design e skill-creator.
- impeccable e web-interface-guidelines: licença incluída em cada pasta.
- graphify: projeto público graphify (pacote `graphifyy`).
