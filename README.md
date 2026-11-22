# Skills para Claude Code

Como instalar: copie cada pasta para `~/.claude/skills/` (no Windows, `C:\Users\<voce>\.claude\skills\`).
Reinicie o Claude Code. Elas aparecem sozinhas e podem ser chamadas com `/nome-da-skill`.

| Skill | Para que serve |
|---|---|
| accessibility | Auditoria e correções de acessibilidade (WCAG 2.2) |
| animate | Constrói uma animação do zero, decidindo propósito, curva, duração e saída |
| break-ui | Estressa uma tela com dados de pior caso e lista o que quebrou |
| find-animation-opportunities | Aponta onde a interface deveria animar (só sugere) |
| improve-animations | Auditoria de motion do projeto com plano priorizado |
| review-animations | Revisão crítica de código de animação |
| prototype | Gera várias versões de um componente de UI com seletor visual |
| impeccable | Design, crítica, polimento e auditoria de interfaces |
| web-interface-guidelines | Revisão de UI contra as Web Interface Guidelines da Vercel |
| graphify | Transforma código/documentos em grafo de conhecimento consultável (precisa de Python; a skill instala o pacote `graphifyy` via uv na primeira vez) |

Cada pasta mantém a licença do autor original (MIT ou Apache 2.0). O graphify é do projeto público graphify (pacote `graphifyy`).
