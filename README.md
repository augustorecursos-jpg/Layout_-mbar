# Layout Âmbar · Mapa de Assentos

Mapa interativo de assentos do **Bloco 6** e da **Matriz (Holding)**, com o visual da Trilha de Desenvolvimento.

- **Quem abre o link** (gestores, equipe) vê o mapa em **modo leitura**: busca por nome, destaque por área, detalhes de cada lugar, exportação para Excel e impressão.
- **Quem edita** (o responsável pelo layout) aloca pessoas, inclui e exclui mesas e, ao final, clica em **Publicar**. A nova versão vai para este repositório e o Render atualiza o site em 1 ou 2 minutos.

## Arquivos

| Arquivo | O que é |
|---|---|
| `index.html` | O sistema inteiro (página única, sem instalação). |
| `dados/mapa.json` | A versão publicada do mapa: pessoas, lugares, áreas e plantas. Atualizado pelo botão **Publicar**. |
| `render.yaml` | Configuração do site estático no Render. |

## Colocar no ar no Render (uma vez)

1. Entre em [render.com](https://render.com) com a conta do GitHub.
2. **New → Static Site** e escolha o repositório `Layout_-mbar`.
3. Preencha:
   - **Branch:** `main`
   - **Build Command:** deixe em branco (ou `echo ok`)
   - **Publish Directory:** `.`
4. Clique em **Create Static Site**. O endereço fica parecido com `https://layout-ambar.onrender.com`.

> Alternativa: **New → Blueprint** e selecione o repositório; o Render lê o `render.yaml` sozinho.

## Entrar como editor (uma vez em cada computador)

1. Crie um token em **GitHub → Settings → Developer settings → Fine-grained tokens → Generate new token**:
   - **Repository access:** *Only select repositories* → `Layout_-mbar`
   - **Permissions → Contents:** *Read and write*
2. Abra o site com `#editor` no final do endereço (ex.: `https://layout-ambar.onrender.com/#editor`), ou clique em **Entrar como editor** no rodapé da lateral.
3. Cole o token. A partir daí, esse navegador mostra os botões de edição e o **Publicar**.

O token fica guardado só no seu navegador. Para sair, use **⋯ → Configurar publicação → Sair do modo editor**.

## Dia a dia

1. Faça as alterações (alocar, mover, editar planta…). Elas são salvas no seu navegador automaticamente.
2. Quando estiver pronto, clique em **Publicar** (o botão fica laranja quando há alterações não publicadas).
3. Em 1–2 minutos, todos que abrirem o link verão a nova versão.

## Privacidade

O mapa contém nomes de colaboradores. Recomenda-se deixar este repositório **privado** (Settings → General → Danger Zone → Change visibility); o Render continua publicando normalmente. Lembre que o endereço do site no Render pode ser aberto por qualquer pessoa que tenha o link.
