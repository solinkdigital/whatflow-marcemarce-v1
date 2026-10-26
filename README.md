# What'flow v1 — MarceMarce Interiores

Protótipo estático mobile-first, sem backend, preparado para VS Code Live Server e GitHub Pages.

## Estrutura obrigatória

Ao publicar, todos estes elementos devem ficar na raiz do repositório (não coloque a pasta inteira dentro de outra pasta):

- `index.html`
- `styles.css`
- `js/app.js`
- `config/companies/marcemarce.json`
- `assets/companies/marcemarce/logo.jpg`
- `assets/companies/marcemarce/cozinha-1.jpg`
- `assets/companies/marcemarce/cozinha-2.jpg`

## Publicar/corrigir no GitHub Pages

1. Descompacte este ZIP no computador.
2. Abra a pasta descompactada. Deve ver `index.html` e `styles.css` directamente, e também as pastas `js`, `config` e `assets`.
3. No repositório `solinkdigital/whatflow-marcemarce-v1`, escolha **Add file → Upload files**.
4. Envie os ficheiros e pastas do conteúdo descompactado, mantendo a estrutura acima. Não envie apenas `index.html`, `styles.css` e `README.md`.
5. Confirme o commit na branch `main`.
6. Em **Settings → Pages**, confirme `Deploy from a branch`, branch `main`, pasta `/(root)`.
7. Aguarde a publicação e actualize o site com `Ctrl + F5`.

Os nomes e as maiúsculas/minúsculas dos ficheiros têm de coincidir exactamente com os caminhos usados no código. O GitHub Pages diferencia maiúsculas e minúsculas.

## Executar localmente

Abra a pasta no VS Code e inicie `index.html` com a extensão Live Server. Não abra directamente via `file://`, porque a configuração da empresa é carregada por `fetch`.

## Funcionalidades e limites

- Identidade visual MarceMarce: logótipo e duas fotografias de cozinhas.
- Texto inicial: “Damos forma ao seu projecto” / “O que vamos produzir?”.
- Selector: português, inglês, francês, chinês simplificado, russo e espanhol.
- Selecção de município dependente da província; a lista de municípios é inicial e precisa de validação contra a divisão administrativa oficial actual de Angola.
- Prepara uma mensagem para WhatsApp; o cliente envia manualmente.
- What'flow Stories não incluído. Sem backend, não há armazenamento central de pedidos nem área de comerciante.
- **Nota de idioma:** nesta versão, a tradução não cobre integralmente todos os campos, validações, revisão final e mensagem WhatsApp. A tradução completa requer uma actualização adicional do JavaScript.

Não coloque segredos ou credenciais no repositório público.
