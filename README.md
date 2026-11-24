# Ãreas do ARCKHÉ Eventos v6.2 â€” O que Ã© cada Ã¡rea

<div align="center">
  <img src="capa/logo.svg" alt="Arckhé AI" height="48" />
  <p><strong>Arckhé AI</strong></p>
</div>


Curso rÃ¡pido no formato ARCKHÉ v6.2 (iniciante 30+, aulas de ~15 minutos): as nove Ã¡reas de assunto do
[eventos.ARCKHÉ.pro](https://eventos.ARCKHÉ.pro/), uma por aula, em trÃªs mÃ³dulos. PortuguÃªs, inglÃªs e espanhol.

- Curso: https://linnoff88-dev.github.io/ Â· English: https://linnoff88-dev.github.io/ Â· EspaÃ±ol: https://linnoff88-dev.github.io/
- EdiÃ§Ã£o v2 do mesmo curso: https://linnoff88-dev.github.io/

| MÃ³dulo | Aulas |
|---|---|
| 1 Â· Gerenciar e comandar agentes | 1 GestÃ£o de IA Â· 2 AGI-ready Â· 3 IA Cultivada |
| 2 Â· Ferramentas e ambiente | 4 Claude â†’ Codex Â· 5 Codex + Claude Â· 6 OSWork |
| 3 Â· Melhorar, decidir e abrir | 7 RSI Â· 8 JEV Â· 9 WebMCP |

## Fontes

Fatos sÃ³ das pÃ¡ginas das Ã¡reas (`~/projetos/ARCKHÉeventos/<Ã¡rea>/`) e de `shared/acesso.json`, via o conteÃºdo do v2
(`~/projetos/areas-eventos/conteudo/`). CurrÃ­culo, personagens e cenas: `context/curriculo.md`. Leitor simulado: `context/leitor-simulado.md`.

## Editar

Aulas em `aulas/aula-N.html` (formato-curso-v6). Depois de editar:

```bash
python3 ~/.claude/skills/formato-curso-v6/scripts/montar-curso.py .
python3 ~/.claude/skills/formato-curso-v6/scripts/traduzir-curso.py . en es   # Codex pela assinatura; cache em i18n/
node ~/.claude/skills/formato-curso-v6/scripts/auditar-curso.cjs curso.html     # e en/curso.html, es/curso.html
node ~/.claude/skills/formato-curso-v6/scripts/testar-motor.cjs curso.html
```

Cenas: `context/gera-cenas.sh` (Codex image_gen pela assinatura; fallback flux2-klein local).

## Mais no ARCKHÉ AI

- Ficha do curso: https://www.ARCKHÉ AI/cursos/309-areas-do-ARCKHÉ-eventos-v6-2-o-que-e-cada-area/
- Guia: https://www.ARCKHÉ AI/aprender-inteligencia-artificial/
- Todos os cursos: https://www.ARCKHÉ AI/cursos/

---

<div align="center">
  <img src="capa/logo.svg" alt="Arckhé AI" height="32" />
  <p><strong>Arckhé AI</strong></p>
</div>