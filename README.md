# Pedras do Brasil — Landing

Landing page estática (HTML/CSS/JS puro, sem build) para a **Pedras do Brasil**, revestimentos e pisos em pedra natural brasileira.

Estilo fino e minimalista (mesmo DNA do Fino Acabamento), fiel à marca: verde `#3E564C`/`#507F69`, serifa da marca (Minion) traduzida em **Cormorant Garamond**, e uma sans geométrica light (**Jost**) para navegação e rótulos. Hero com slideshow de fundo e título que troca a cada slide.

## Rodar local

```bash
python3 -m http.server 8790
# abre http://localhost:8790
```

Ou só abrir o `index.html` no navegador.

## Estrutura

- `index.html` — página inteira (CSS e JS embutidos, para carregar rápido)
- `assets/img/` — fotos (hero, linhas, aplicações) e logos, em WebP/PNG
- `assets/textures/` — swatches de material (amostras)
- `assets/fonts/` — Cormorant Garamond + Jost, self-hosted (woff2)
- `favicon.ico` / `favicon-256.png`

Fotos e logos extraídos dos catálogos e do manual de marca oficiais da Pedras do Brasil.

## Performance

Lighthouse mobile (throttle real, devtools): **Performance 98 · Acessibilidade 100 · Best Practices 100 · SEO 100**. FCP/LCP 1,0s, CLS 0.

## ⚠️ Preencher antes de publicar

Os contatos estão com placeholder. Trocar em `index.html`:

| Onde | Placeholder atual | Trocar por |
|---|---|---|
| WhatsApp (JS, `var TEL`) | `5528999999999` | número real (formato `55` + DDD + número) |
| Telefone exibido | `(28) 99999-9999` | número real |
| E-mail | `contato@pedrasdobrasil.com.br` | e-mail real |
| Instagram | `@pedrasdobrasil` | handle real |
| Cidade | `Cachoeiro de Itapemirim · Espírito Santo` | confirmar cidade/UF |

O `TEL` no JS controla todos os links de WhatsApp e o envio do formulário (abre o WhatsApp com a mensagem pronta). É só trocar em um lugar.
