# Brief comum ê¢â¬â aulas 2 a 9 do "êÂreas do ARCKHê Eventos v6.2"

Curso: `~/projetos/areas-eventos-v62` (formato-curso-v6, **perfil têÂ©cnico**, 9 aulas, 1 aula = 1 êÂ¡rea do eventos.ARCKHê.pro).
Leia antes: `context/curriculo.md` (promessa, prêÂ¡tica e gancho de cada aula; personagens; cenas), `curso.json` (termos),
a skill `~/.claude/skills/formato-curso-v6/` (SKILL.md + references/CONTEUDO-INICIANTE.md, V6-DESIGN.md, CHECKLIST-V6.md)
e o **molde aprovado 10/10**: `aulas/aula-1.html` (GestêÂ£o de IA). Siga a mesma estrutura e densidade.

## Fonte dos fatos (êÂºnica)
`~/projetos/areas-eventos/conteudo/trilha{1,2,3}.py` ê¢â¬â `MODULES[i]` da trilha (êÂ­ndice local 0..2). Campos: title, goal, steps (lab),
check/answer (bom para o teste-se), snippet (prompt pronto ê¢â¬â base da prêÂ¡tica), sources (links), topics (6 têÂ³picos: what/why/keys/example/action).
Pode conferir na pêÂ¡gina original `~/projetos/ARCKHêeventos/<slug>/index.html`. **Nada fora disso**: sem data ou preêÂ§o que a pêÂ¡gina nêÂ£o tenha;
Claude ê¢â â Codex sem data de evento; IA Cultivada sem vêÂ­deo; nenhum vêÂ­deo do Explicavideos. ConteêÂºdo de terceiros citado na pêÂ¡gina: sêÂ³ referêÂªncia.

## Regras desta ediêÂ§êÂ£o
- Personagens fixos do curso: **SêÂ´nia**, gerente de loja (49, loja de calêÂ§ados de bairro com site e WhatsApp) ê¢â â `data-ex="gerente de loja"`;
  **Diego**, analista de RH (35, empresa de 120 pessoas) ê¢â â `data-ex="analista de RH"`. Alterne os dois; situaêÂ§êÂµes novas em cada aula
  (nêÂ£o repita as da aula 1: lista de assistentes do RH, ficha da vendedora de WhatsApp, fêÂ©rias, pedidos copiados para planilha).
- Kicker: `Aula N de 9 êÂ· <êÂrea>`. Cena: `assets/img/aula-N.webp` (jêÂ¡ gerada; alt descrevendo a cena do curriculo.md, >20 caracteres).
- 3ê¢â¬â4 steps, cada um com visual real (`.tela`, `.lado`, `.janela`, `.terminal`, `.diag` sêÂ³ se nêÂ£o houver tela). ê¢â°Â¥1 `.calma`. 1 `.quiz` (use check/answer do v2 quando couber).
- PrêÂ¡tica = a do currêÂ­culo, baseada no `snippet` do v2, **simplificada** para ê¢â°Â¤12 min e para chat de IA comum (copiar e colar). êÂrea com
  comando (Codex + Claude): o caminho principal êÂ© no chat; o comando pode ir num `details.mais` com `.terminal`, com `.gterm` nos termos.
- Termos de `curso.json` (agente, Codex, Claude Code, WebMCP, Skill, LOOP-R, token, runtime, lock-in, Computer Use, evals, handoff, SEO)
  e toda palavra da lista-sentinela (terminal, API, script, servidor, instalar, login, workflowê¢â¬Â¦) **sêÂ³ com `.gterm` na 1êÂª vez nesta aula**,
  com a MESMA definiêÂ§êÂ£o (`data-def`) em todas as aulas. DefiniêÂ§êÂµes jêÂ¡ usadas: veja `aulas/aula-1.html` (agente, LOOP-R, token) e as das
  outras aulas prontas em `aulas/`. Evite o termo quando uma palavra comum resolver.
- `details.complementar` depois da `.fecho`: os 6 têÂ³picos do v2 da êÂ¡rea, **enxugados** em frases curtas (ê¢â°Â¤22 palavras), um `comp-sec` por têÂ³pico,
  e `p.comp-fontes` com os `sources`. Mesmo cuidado de jargêÂ£o.
- Tela "boa" simulada nunca inventa nêÂºmero, data ou nome que nêÂ£o esteja no pedido mostrado.
- CartêÂµes `cards-N`: 3 ou 4, frente termina em "?", formas decisêÂ£o/diagnêÂ³stico/aplicaêÂ§êÂ£o, sem repetir a `.cola`.
- `nav.lnav`: `#aula-(N-1)`/trilha e `#aula-(N+1)`; na aula 9 o prêÂ³ximo êÂ© `#trilha` ("voltar êÂ  trilha ê¢â â"). RodapêÂ© `Aula N êÂ· êÂreas ARCKHê v6.2 êÂ· ARCKHê AI PRO`.
- `data-tempo` = palavras/200 + minutos da prêÂ¡tica + 1 (arredonde para cima), alvo 12ê¢â¬â15.

## Como validar (numa cêÂ³pia isolada, nunca montando no projeto)
```bash
S=$(mktemp -d)/c; cp -r ~/projetos/areas-eventos-v62 $S
python3 -c "import json;p='$S/curso.json';c=json.load(open(p));c['modulos']=[{'titulo':'M','aulas':[N]}];json.dump(c,open(p,'w'),ensure_ascii=False)"
# a montagem aceita sêÂ³ as aulas listadas; renomeie/ajuste se precisar (aula N sozinha)
python3 ~/.claude/skills/formato-curso-v6/scripts/montar-curso.py $S
node ~/.claude/skills/formato-curso-v6/scripts/auditar-curso.cjs $S/curso.html
```
Meta: **ê¢â°Â¥9/10 e sem falha em 7, 8 e 10** (mire 10/10). Grave sêÂ³ o arquivo final em `~/projetos/areas-eventos-v62/aulas/aula-N.html`.
NêÂ£o gere imagens, nêÂ£o faêÂ§a git, nêÂ£o chame API externa. Ao terminar, feche qualquer Chromium que tenha aberto.
Responda: nota do auditor, nêÂº de palavras, e qualquer fato de que ficou em dêÂºvida.
