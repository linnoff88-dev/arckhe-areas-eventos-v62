# CurrÃ­culo â€” Ãreas do ARCKHÉ Eventos v6.2

EdiÃ§Ã£o v6.2 (formato-curso-v6, perfil tÃ©cnico) do curso v2 `linnoff88-dev/areas-eventos` (id 307 no portal).
Fonte Ãºnica de fatos: `~/projetos/areas-eventos/conteudo/trilha{1,2,3}.py`, que por sua vez sÃ³ usa as pÃ¡ginas
`~/projetos/ARCKHÉeventos/<Ã¡rea>/index.html` + `shared/acesso.json` (lidas em 28/09/2026). Mapa: `~/projetos/wifi/PLANO-VIDEOS-EXPLICAVIDEOS-EVENTOS.md`.

## Descoberta (Passo 0) â€” definida pelo agente em 29/09/2026 a partir do plano e do v2; o usuÃ¡rio pode trocar

1. **Aluno:** profissional ou gestor de 30+ que jÃ¡ usa IA no trabalho (chat), ouviu falar das Ã¡reas do eventos.ARCKHÉ.pro
   e nÃ£o sabe o que cada uma Ã© nem por onde comeÃ§ar.
2. **ProfissÃµes-alvo:** **gerente de loja** (SÃ´nia, 49, loja de calÃ§ados de bairro com site e WhatsApp) e **analista de RH**
   (Diego, 35, empresa de 120 pessoas). Anti-clone: nÃ£o usadas nos Ãºltimos v6 (contadora/fisioterapeuta, dona de clÃ­nica/contador,
   desenvolvedor/analista, coordenadora/professora, professor/gestora). `data-ex="gerente de loja"` e `data-ex="analista de RH"`.
3. **JÃ¡ usa:** celular, WhatsApp, e-mail, planilha, um chat de IA. NÃ£o programa. NÃ£o usa terminal.
4. **Sai fazendo:** explica cada Ã¡rea em uma frase, sabe para quem ela Ã© e sai com um primeiro passo feito na Ã¡rea escolhida.
5. **SessÃ£o:** 15 minutos, muitas vezes no celular.

## Regras de conteÃºdo

- SÃ³ fatos, nÃºmeros e nomes das pÃ¡ginas das Ã¡reas / acesso.json (via trilhaN.py). Sem data ou preÃ§o que a pÃ¡gina nÃ£o tenha.
- Claude â†’ Codex: nada de data de evento. IA Cultivada: nada de vÃ­deo. Nenhum vÃ­deo do Explicavideos.
- Tela "boa" simulada nunca inventa nÃºmero, data ou nome que nÃ£o esteja no pedido.
- Termos tÃ©cnicos (agente, Codex, Claude Code, WebMCPâ€¦) sempre com `.gterm` na primeira vez em CADA aula.
- `details.complementar` = os 6 tÃ³picos do v2 daquela Ã¡rea (o que Ã© / por que / conceitos / na prÃ¡tica), texto do v2 enxugado.

## MÃ³dulos e aulas (1 aula = 1 Ã¡rea)

| Aula | Ãrea | MÃ³dulo | Promessa ("VocÃª consegueâ€¦") | PrÃ¡tica | Gancho para a prÃ³xima |
|---|---|---|---|---|---|
| 1 | GestÃ£o de IA | 1 Â· Gerenciar e comandar agentes | dizer o que a Ã¡rea resolve e escolher um processo seu que um agente poderia assumir sob gestÃ£o | prompt | gerenciar exige saber delegar: aula 2 |
| 2 | AGI-ready | 1 | reescrever um pedido seu como delegaÃ§Ã£o (objetivo, contexto, limites, como saber que estÃ¡ bom) | prompt | delegar uma vez Ã© fÃ¡cil; melhorar sempre Ã© cultivar: aula 3 |
| 3 | IA Cultivada | 1 | montar a ficha de um agente seu com os oito elementos do cultivo | prompt | a ficha Ã© sua ou do fornecedor? aula 4 |
| 4 | Claude â†’ Codex | 2 Â· Ferramentas e ambiente | encontrar onde o seu jeito de trabalhar com IA estÃ¡ preso e juntar num documento que qualquer modelo lÃª | tarefa | com dois modelos Ã  mÃ£o, use os dois: aula 5 |
| 5 | Codex + Claude | 2 | pedir que uma IA revise o que outra fez, com achados e correÃ§Ã£o mÃ­nima | prompt | onde guardar tudo isso: aula 6 |
| 6 | OSWork | 2 | escolher a ediÃ§Ã£o do OSWork certa para o seu momento | analise | o sistema funciona; agora, fazÃª-lo melhorar: aula 7 |
| 7 | RSI | 3 Â· Melhorar, decidir e abrir | rodar um ciclo curto de melhoria com teste antes e depois | prompt | melhorar exige decidir entre versÃµes: aula 8 |
| 8 | JEV | 3 | montar uma decisÃ£o com alternativas e critÃ©rio e conferir a escolha | prompt | e quando quem decide Ã© o agente do cliente, no seu site? aula 9 |
| 9 | WebMCP | 3 | fazer o diagnÃ³stico gratuito do seu site e escolher a primeira correÃ§Ã£o | tarefa | fim: voltar ao mapa e escolher a Ã¡rea |

## Cenas (sem texto na imagem, adultos brasileiros 30â€“60, sem robÃ´)

- trilha: gerente de loja (mulher, 49) e analista de RH (homem, 35) numa mesa de cafÃ© de trabalho olhando juntos um mapa de papel com nove caminhos coloridos.
- aula-1: Diego, analista de RH, numa sala de reuniÃ£o, cola notas adesivas num quadro separando tarefas de pessoas e tarefas que poderiam ir para um assistente.
- aula-2: SÃ´nia, gerente de loja, no balcÃ£o da loja de calÃ§ados, escreve num caderno uma lista de responsabilidades para delegar, celular ao lado.
- aula-3: Diego revisa numa mesa uma ficha impressa com anotaÃ§Ãµes Ã  mÃ£o, como quem ajusta uma receita, xÃ­cara de cafÃ© ao lado.
- aula-4: SÃ´nia, no escritÃ³rio dos fundos da loja, junta anotaÃ§Ãµes espalhadas (post-its, caderno, celular) numa Ãºnica pasta de papel.
- aula-5: Diego no notebook com duas janelas lado a lado, comparando dois rascunhos, marcando um papel com caneta.
- aula-6: SÃ´nia em casa Ã  noite, escolhendo entre cinco pastas coloridas sobre a mesa, notebook aberto.
- aula-7: Diego compara duas versÃµes impressas de um documento, marcando com âœ“ e âœ— Ã  caneta, numa mesa organizada.
- aula-8: SÃ´nia no estoque da loja, tablet na mÃ£o, pesando duas opÃ§Ãµes de pedido de reposiÃ§Ã£o diante das prateleiras de caixas.
- aula-9: SÃ´nia no balcÃ£o olhando o site da loja no notebook enquanto uma cliente mostra algo no celular.
