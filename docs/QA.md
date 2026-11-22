# Checklist de QA

| # | Critério | Status |
|---|---|---|
| 1 | Build | Não há build: site estático puro |
| 2 | Publicável no GitHub Pages | Workflow `pages.yml`, caminhos relativos |
| 3 | Assets com base path de repositório | Todos os caminhos relativos (`css/`, `vendor/`, `assets/`) |
| 4 | Funciona offline | Nenhuma requisição externa. Os links de referência só abrem se clicados |
| 5 | Sem cortes em 1920×1080 e 1366×768 | Verificado por screenshot (Chromium headless) |
| 6 | Teclado e fullscreen | Padrão do Reveal (`→`, `←`, `F`, `S`, `Esc`) |
| 7 | Omarchy só revelado no slide 12 | Slide 2 só mostra "MacBook Air 2013 · Omarchy Linux". A revelação no 12 é falada (notas); as fotos do meetup não são usadas |
| 8 | Texto em pt-BR, sem placeholders | OK |
| 9 | Fontes e afirmações sensíveis | Ver abaixo |
| 10 | README com dev, deploy e palco | `README.md` |

## Afirmações e fontes

- **Satya Nadella:** paráfrase, sem aspas. [The Pragmatic Engineer, 16/11/2026](https://newsletter.pragmaticengineer.com/p/software-engineering-after-code-becomes), trechos de verificação (~12:32) e software factories (~15:39).
- **Tobi Lütke:** paráfrase. O termo *slop grenades* vem do The Knowledge Project (Shane Parrish), set/2026, e saiu em várias matérias. Sobre o River: artigo [Learning on the Shop floor](https://x.com/tobi/status/2053121182044451016) (X, mai/2026). Os números do River (1.870 PRs/semana, ~1 em 8 PRs) **não aparecem na tela**, porque só foram vistos por fontes secundárias.
- **DHH, keynote:** paráfrase ("se declarou aposentado da programação profissional; código à mão virou exceção na 37signals"). [Keynote Rails World 2026](https://www.youtube.com/watch?v=vDjW_dRyKXY), 23/09/2026. Conferir a fala exata no vídeo se for citar literalmente.
- **"Very soon":** relato do palestrante sobre conversa presencial (pergunta de Obie Fernandez). Wording confirmado pelo palestrante. Identificado na tela como relato.
- **60+ PRs / 2 dias / ≈30 por dia:** experimento próprio. A ressalva "não benchmark; volume não comprova qualidade" fica nas notas do palestrante.
- **Gráfico do slide 7:** ilustrativo, sem dados (indicado nas notas).
- **Omarchy, slide 12:** os números vêm do repositório oficial [omacom/omarchy](https://github.com/omacom/omarchy) em 22/11/2026. O repositório antigo `basecamp/omarchy` redireciona para ele.
  - **Commits:** `git rev-list --count HEAD` na branch `quattro` deu 8.179.
  - **Primeiro commit:** 01/06/2025, de DHH ("Initial basics").
  - **PRs:** 2.404 mergeados de 10.448 abertos, pela busca `is:pr is:merged` da API do GitHub. Commits enviados direto na branch, sem PR, não entram nessa conta.
  - **Ritmo recente:** 769 PRs mergeados entre 22/10 e 21/11/2026, cerca de 26 por dia.
  - **Autores:** 671 e-mails distintos, o que é uma aproximação do número de pessoas.
  - **Versões:** datas das tags v1.1.0 (04/07/2025), v2.0.0 (25/08/2025), v3.0.0 (17/09/2025), v4.0.0 (14/08/2026) e v4.5.0 (04/11/2026).
- **DHH sobre o Omarchy:** paráfrase. No Lex Fridman Podcast #501 (26/08/2026) ele disse que agentes escreveram praticamente todo o código do Omarchy Quattro: "in the last two months it has been 100%". Fonte secundária: Startup Fortune. No post da DigitalOcean (set/2026) ele fala em "agent runners for PR reviews" no pipeline do Omarchy.
