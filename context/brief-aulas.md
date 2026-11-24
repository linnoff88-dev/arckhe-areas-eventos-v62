# Brief comum â€” aulas 2 a 9 do "Ãreas do ARCKHÉ Eventos v6.2"

Curso: `~/projetos/areas-eventos-v62` (formato-curso-v6, **perfil tÃ©cnico**, 9 aulas, 1 aula = 1 Ã¡rea do eventos.ARCKHÉ.pro).
Leia antes: `context/curriculo.md` (promessa, prÃ¡tica e gancho de cada aula; personagens; cenas), `curso.json` (termos),
a skill `~/.claude/skills/formato-curso-v6/` (SKILL.md + references/CONTEUDO-INICIANTE.md, V6-DESIGN.md, CHECKLIST-V6.md)
e o **molde aprovado 10/10**: `aulas/aula-1.html` (GestÃ£o de IA). Siga a mesma estrutura e densidade.

## Fonte dos fatos (Ãºnica)
`~/projetos/areas-eventos/conteudo/trilha{1,2,3}.py` â€” `MODULES[i]` da trilha (Ã­ndice local 0..2). Campos: title, goal, steps (lab),
check/answer (bom para o teste-se), snippet (prompt pronto â€” base da prÃ¡tica), sources (links), topics (6 tÃ³picos: what/why/keys/example/action).
Pode conferir na pÃ¡gina original `~/projetos/ARCKHÉeventos/<slug>/index.html`. **Nada fora disso**: sem data ou preÃ§o que a pÃ¡gina nÃ£o tenha;
Claude â†’ Codex sem data de evento; IA Cultivada sem vÃ­deo; nenhum vÃ­deo do Explicavideos. ConteÃºdo de terceiros citado na pÃ¡gina: sÃ³ referÃªncia.

## Regras desta ediÃ§Ã£o
- Personagens fixos do curso: **SÃ´nia**, gerente de loja (49, loja de calÃ§ados de bairro com site e WhatsApp) â†’ `data-ex="gerente de loja"`;
  **Diego**, analista de RH (35, empresa de 120 pessoas) â†’ `data-ex="analista de RH"`. Alterne os dois; situaÃ§Ãµes novas em cada aula
  (nÃ£o repita as da aula 1: lista de assistentes do RH, ficha da vendedora de WhatsApp, fÃ©rias, pedidos copiados para planilha).
- Kicker: `Aula N de 9 Â· <Ãrea>`. Cena: `assets/img/aula-N.webp` (jÃ¡ gerada; alt descrevendo a cena do curriculo.md, >20 caracteres).
- 3â€“4 steps, cada um com visual real (`.tela`, `.lado`, `.janela`, `.terminal`, `.diag` sÃ³ se nÃ£o houver tela). â‰¥1 `.calma`. 1 `.quiz` (use check/answer do v2 quando couber).
- PrÃ¡tica = a do currÃ­culo, baseada no `snippet` do v2, **simplificada** para â‰¤12 min e para chat de IA comum (copiar e colar). Ãrea com
  comando (Codex + Claude): o caminho principal Ã© no chat; o comando pode ir num `details.mais` com `.terminal`, com `.gterm` nos termos.
- Termos de `curso.json` (agente, Codex, Claude Code, WebMCP, Skill, LOOP-R, token, runtime, lock-in, Computer Use, evals, handoff, SEO)
  e toda palavra da lista-sentinela (terminal, API, script, servidor, instalar, login, workflowâ€¦) **sÃ³ com `.gterm` na 1Âª vez nesta aula**,
  com a MESMA definiÃ§Ã£o (`data-def`) em todas as aulas. DefiniÃ§Ãµes jÃ¡ usadas: veja `aulas/aula-1.html` (agente, LOOP-R, token) e as das
  outras aulas prontas em `aulas/`. Evite o termo quando uma palavra comum resolver.
- `details.complementar` depois da `.fecho`: os 6 tÃ³picos do v2 da Ã¡rea, **enxugados** em frases curtas (â‰¤22 palavras), um `comp-sec` por tÃ³pico,
  e `p.comp-fontes` com os `sources`. Mesmo cuidado de jargÃ£o.
- Tela "boa" simulada nunca inventa nÃºmero, data ou nome que nÃ£o esteja no pedido mostrado.
- CartÃµes `cards-N`: 3 ou 4, frente termina em "?", formas decisÃ£o/diagnÃ³stico/aplicaÃ§Ã£o, sem repetir a `.cola`.
- `nav.lnav`: `#aula-(N-1)`/trilha e `#aula-(N+1)`; na aula 9 o prÃ³ximo Ã© `#trilha` ("voltar Ã  trilha â†’"). RodapÃ© `Aula N Â· Ãreas ARCKHÉ v6.2 Â· ARCKHÉ AI PRO`.
- `data-tempo` = palavras/200 + minutos da prÃ¡tica + 1 (arredonde para cima), alvo 12â€“15.

## Como validar (numa cÃ³pia isolada, nunca montando no projeto)
```bash
S=$(mktemp -d)/c; cp -r ~/projetos/areas-eventos-v62 $S
python3 -c "import json;p='$S/curso.json';c=json.load(open(p));c['modulos']=[{'titulo':'M','aulas':[N]}];json.dump(c,open(p,'w'),ensure_ascii=False)"
# a montagem aceita sÃ³ as aulas listadas; renomeie/ajuste se precisar (aula N sozinha)
python3 ~/.claude/skills/formato-curso-v6/scripts/montar-curso.py $S
node ~/.claude/skills/formato-curso-v6/scripts/auditar-curso.cjs $S/curso.html
```
Meta: **â‰¥9/10 e sem falha em 7, 8 e 10** (mire 10/10). Grave sÃ³ o arquivo final em `~/projetos/areas-eventos-v62/aulas/aula-N.html`.
NÃ£o gere imagens, nÃ£o faÃ§a git, nÃ£o chame API externa. Ao terminar, feche qualquer Chromium que tenha aberto.
Responda: nota do auditor, nÂº de palavras, e qualquer fato de que ficou em dÃºvida.
