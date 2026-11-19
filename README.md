# Ãreas do INEMA Eventos v6.2 â€” O que Ã© cada Ã¡rea

<div align="center">
  <img src="capa/logo.svg" alt="Arckhé AI" height="48" />
  <p><strong>Arckhé AI</strong></p>
</div>


Curso rÃ¡pido no formato INEMA v6.2 (iniciante 30+, aulas de ~15 minutos): as nove Ã¡reas de assunto do
[eventos.inema.pro](https://eventos.inema.pro/), uma por aula, em trÃªs mÃ³dulos. PortuguÃªs, inglÃªs e espanhol.

- Curso: https://inematds.github.io/areas-eventos-v62/ Â· English: https://inematds.github.io/areas-eventos-v62/en/ Â· EspaÃ±ol: https://inematds.github.io/areas-eventos-v62/es/
- EdiÃ§Ã£o v2 do mesmo curso: https://inematds.github.io/areas-eventos/

| MÃ³dulo | Aulas |
|---|---|
| 1 Â· Gerenciar e comandar agentes | 1 GestÃ£o de IA Â· 2 AGI-ready Â· 3 IA Cultivada |
| 2 Â· Ferramentas e ambiente | 4 Claude â†’ Codex Â· 5 Codex + Claude Â· 6 OSWork |
| 3 Â· Melhorar, decidir e abrir | 7 RSI Â· 8 JEV Â· 9 WebMCP |

## Fontes

Fatos sÃ³ das pÃ¡ginas das Ã¡reas (`~/projetos/inemaeventos/<Ã¡rea>/`) e de `shared/acesso.json`, via o conteÃºdo do v2
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

## Mais no INEMA.CLUB

- Ficha do curso: https://www.inema.club/cursos/309-areas-do-inema-eventos-v6-2-o-que-e-cada-area/
- Guia: https://www.inema.club/aprender-inteligencia-artificial/
- Todos os cursos: https://www.inema.club/cursos/

---

<div align="center">
  <img src="capa/logo.svg" alt="Arckhé AI" height="32" />
  <p><strong>Arckhé AI</strong></p>
</div>