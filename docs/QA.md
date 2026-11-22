# Checklist de QA

| # | Critério | Status |
|---|---|---|
| 1 | Build | Não há build: site estático puro |
| 2 | Publicável no GitHub Pages | Workflow `pages.yml`, caminhos relativos |
| 3 | Assets com base path de repositório | Todos os caminhos relativos (`css/`, `vendor/`, `assets/`) |
| 4 | Funciona offline | Nenhuma requisição externa. Os links de referência só abrem se clicados |
| 5 | Sem cortes em 1920×1080 e 1366×768 | Verificado por screenshot (Chromium headless) |
| 6 | Teclado e fullscreen | Padrão do Reveal (`→`, `←`, `F`, `S`, `Esc`) |
| 7 | Omarchy só revelado no slide 13 | Slide 2 só mostra "MacBook Air 2013 · Omarchy Linux". Fotos do meetup só no 13 |
| 8 | Texto em pt-BR, sem placeholders | OK |
| 9 | Fontes e afirmações sensíveis | Ver abaixo |
| 10 | README com dev, deploy e palco | `README.md` |

## Afirmações e fontes

- **Satya Nadella:** paráfrase, sem aspas. [The Pragmatic Engineer, 16/11/2026](https://newsletter.pragmaticengineer.com/p/software-engineering-after-code-becomes), trechos de verificação (~12:32) e software factories (~15:39).
- **Tobi Lütke:** paráfrase. O termo *slop grenades* vem do The Knowledge Project (Shane Parrish), set/2026, e saiu em várias matérias. Sobre o River: artigo [Learning on the Shop floor](https://x.com/tobi/status/2053121182044451016) (X, mai/2026). Os números do River (1.870 PRs/semana, ~1 em 8 PRs) **não aparecem na tela**, porque só foram vistos por fontes secundárias.
- **DHH, keynote:** paráfrase ("se declarou aposentado da programação profissional; código à mão virou exceção na 37signals"). [Keynote Rails World 2026](https://www.youtube.com/watch?v=vDjW_dRyKXY), 23/09/2026. Conferir a fala exata no vídeo se for citar literalmente.
- **"Very soon":** relato do palestrante sobre conversa presencial (pergunta de Obie Fernandez). Wording confirmado pelo palestrante. Identificado na tela como relato.
- **60+ PRs / 2 dias / ≈30 por dia:** experimento próprio. Identificado como "não benchmark; volume não comprova qualidade".
- **Gráfico do slide 7 e barras do slide 10:** ilustrativos, sem dados. Isso está escrito na tela.
- **Card de PR do slide 6:** exemplo fictício e ilustrativo.
