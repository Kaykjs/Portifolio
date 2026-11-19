# Portifolio

Portfólio pessoal de Kayk Junior, feito com HTML, CSS e JavaScript.

## Painel ADM de projetos

Os projetos do site ficam no arquivo `projetos.json` e podem ser gerenciados pelo painel em **`/admin`** (ex.: `https://SEU-SITE/admin/`), sem mexer no código.

No painel dá para:

- adicionar, editar e excluir projetos;
- mudar a ordem (os 3 primeiros aparecem logo de cara no site);
- enviar o print do projeto (a imagem é reduzida automaticamente para não pesar).

Ao clicar em **Publicar no site**, o painel salva as mudanças direto neste repositório no GitHub, e a hospedagem (Vercel/GitHub Pages) atualiza o site sozinha em cerca de 1 minuto.

### Criar o token de acesso (só uma vez)

1. Acesse https://github.com/settings/personal-access-tokens/new
2. Dê um nome (ex.: `painel-portfolio`) e escolha a validade.
3. Em **Repository access**, escolha **Only select repositories** → `Portifolio`.
4. Em **Permissions → Repository permissions → Contents**, escolha **Read and write**.
5. Clique em **Generate token**, copie e cole no painel.

O token fica salvo só no seu navegador. Nunca coloque o token no código nem compartilhe.

### Importante

Como o painel salva direto no GitHub, antes de editar o projeto no seu computador faça **Fetch/Pull** (no GitHub Desktop: *Fetch origin* → *Pull origin*) para baixar as mudanças feitas pelo painel.

### Testar localmente

O site lê o `projetos.json` com `fetch`, então abra com o **Live Server** do VS Code (abrir o `index.html` com dois cliques não carrega os projetos).
