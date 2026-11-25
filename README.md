# êÂreas do ARCKHê Eventos v6.2 ê¢â¬â O que êÂ© cada êÂ¡rea

<div align="center">
  <img src="capa/logo.svg" alt="Arckhé AI" height="48" />
  <p><strong>Arckhé AI</strong></p>
</div>


Curso rêÂ¡pido no formato ARCKHê v6.2 (iniciante 30+, aulas de ~15 minutos): as nove êÂ¡reas de assunto do
[eventos.ARCKHê.pro](https://eventos.ARCKHê.pro/), uma por aula, em trêÂªs mêÂ³dulos. PortuguêÂªs, inglêÂªs e espanhol.

- Curso: https://linnoff88-dev.github.io/ êÂ· English: https://linnoff88-dev.github.io/ êÂ· EspaêÂ±ol: https://linnoff88-dev.github.io/
- EdiêÂ§êÂ£o v2 do mesmo curso: https://linnoff88-dev.github.io/

| MêÂ³dulo | Aulas |
|---|---|
| 1 êÂ· Gerenciar e comandar agentes | 1 GestêÂ£o de IA êÂ· 2 AGI-ready êÂ· 3 IA Cultivada |
| 2 êÂ· Ferramentas e ambiente | 4 Claude ê¢â â Codex êÂ· 5 Codex + Claude êÂ· 6 OSWork |
| 3 êÂ· Melhorar, decidir e abrir | 7 RSI êÂ· 8 JEV êÂ· 9 WebMCP |

## Fontes

Fatos sêÂ³ das pêÂ¡ginas das êÂ¡reas (`~/projetos/ARCKHêeventos/<êÂ¡rea>/`) e de `shared/acesso.json`, via o conteêÂºdo do v2
(`~/projetos/areas-eventos/conteudo/`). CurrêÂ­culo, personagens e cenas: `context/curriculo.md`. Leitor simulado: `context/leitor-simulado.md`.

## Editar

Aulas em `aulas/aula-N.html` (formato-curso-v6). Depois de editar:

```bash
python3 ~/.claude/skills/formato-curso-v6/scripts/montar-curso.py .
python3 ~/.claude/skills/formato-curso-v6/scripts/traduzir-curso.py . en es   # Codex pela assinatura; cache em i18n/
node ~/.claude/skills/formato-curso-v6/scripts/auditar-curso.cjs curso.html     # e en/curso.html, es/curso.html
node ~/.claude/skills/formato-curso-v6/scripts/testar-motor.cjs curso.html
```

Cenas: `context/gera-cenas.sh` (Codex image_gen pela assinatura; fallback flux2-klein local).

## Mais no ARCKHê AI

- Ficha do curso: https://www.ARCKHê AI/cursos/309-areas-do-ARCKHê-eventos-v6-2-o-que-e-cada-area/
- Guia: https://www.ARCKHê AI/aprender-inteligencia-artificial/
- Todos os cursos: https://www.ARCKHê AI/cursos/

---

<div align="center">
  <img src="capa/logo.svg" alt="Arckhé AI" height="32" />
  <p><strong>Arckhé AI</strong></p>
</div>