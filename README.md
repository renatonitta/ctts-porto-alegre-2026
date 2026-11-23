# Agentes de IA no processo de desenvolvimento de software
### A qualidade e a velocidade

Apresentação de Renato Nitta (@renatonitta) no CTTS Porto Alegre 2026. São 12 slides, cerca de 20 minutos.

Site estático com [Reveal.js 5.1.0](https://revealjs.com) incluído no repositório (`vendor/`). Não tem build, Node, nem dependência de rede: fontes, scripts e fotos são todos locais.

## Estrutura

```
index.html              slides + notas do palestrante (<aside class="notes">)
css/style.css           visual (tema escuro, 1920×1080)
vendor/reveal/          Reveal.js 5.1.0 + plugin de notas (MIT)
vendor/fonts/           Source Sans Pro (OFL)
assets/photos/*.webp    fotos otimizadas usadas nos slides
assets/photos/original/ fotos originais, sem alteração
.github/workflows/      deploy automático no GitHub Pages
docs/QA.md              checklist de aceite e fontes
```

## Rodar localmente

```sh
python3 -m http.server 8000
# abrir http://localhost:8000
```

Abrir `index.html` direto pelo navegador também funciona. Só a janela de notas do palestrante precisa de um servidor local.

## Deploy

Cada push na `main` publica o site pelo workflow `.github/workflows/pages.yml`.
Configuração (uma vez só): **Settings → Pages → Source: GitHub Actions**.
URL: https://renatonitta.github.io/ctts-porto-alegre-2026/

## No palco

| Tecla | Ação |
|---|---|
| `→` / `Espaço` | próximo (inclui revelações) |
| `←` | anterior |
| `F` | tela cheia |
| `S` | notas do palestrante + cronômetro (janela separada) |
| `Esc` / `O` | visão geral dos slides |
| `B` / `.` | tela preta (pausa) |
| `L` | alterna tema escuro / claro |

- Abrir a apresentação pelo servidor local (`python3 -m http.server`) no MacBook. Depois do primeiro carregamento ela funciona sem internet.
- Apertar `S` antes de começar e arrastar a janela de notas para a tela do notebook.
- Os slides 6 e 7 têm revelações em etapas. Cada `→` mostra a próxima.
- O slide 12 traz as **Referências** e os contatos. Dá para deixá-lo na tela durante as perguntas.
- **Tema claro:** aperte `L` para alternar entre escuro e claro, caso o projetor não fique bom. A escolha fica salva no navegador. Também dá para abrir direto no claro com `?theme=light` na URL.
