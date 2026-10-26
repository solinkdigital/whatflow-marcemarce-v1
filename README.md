# What'flow v1 — MarceMarce Interiores

Protótipo estático mobile-first, sem backend, preparado para execução via VS Code Live Server e publicação no GitHub Pages.

## Incluído nesta versão de trabalho
- Identidade visual MarceMarce: logótipo e duas fotografias de cozinhas.
- Texto inicial actualizado: “Damos forma ao seu projecto” / “O que vamos produzir?”.
- Selector de idioma para Português (predefinido), Inglês, Francês, Chinês simplificado, Russo e Espanhol. A tradução desta versão cobre elementos principais da interface; ainda não é uma tradução integral de todos os campos, validações e da mensagem WhatsApp.
- Selecção de município dependente da província e limpeza do município quando a província muda.
- Preparação de mensagem para WhatsApp; o cliente deve enviar manualmente.
- What'flow Stories não incluído, conforme decisão de manter a versão sem backend.

## Importante sobre os municípios
O ficheiro `js/app.js` contém uma lista inicial de municípios por província para demonstrar a dependência dinâmica. A lista ainda precisa de validação e complementação contra a divisão administrativa oficial actual de Angola antes de ser considerada completa ou usada como fonte oficial.

## Executar localmente
1. Descompacte o ZIP.
2. Abra a pasta no VS Code.
3. Inicie `index.html` com a extensão Live Server.
4. Teste as etapas, selecção de idioma, província/município e abertura do WhatsApp.

Não abra `index.html` directamente via `file://`, pois o carregamento da configuração JSON usa `fetch`.

## Publicar no GitHub Pages
Envie o conteúdo da pasta para a raiz do repositório. Em Settings → Pages, escolha Deploy from a branch, `main` e `/(root)`.

## Limitações
- Sem backend, não existe armazenamento central de pedidos, login de comerciantes ou publicação real de Stories.
- O selector multilingue ainda não traduz todos os textos da aplicação. A tradução integral do formulário e da mensagem WhatsApp deve ser concluída numa iteração seguinte.
- Não colocar segredos ou credenciais no repositório público.
