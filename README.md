# Portfólio — Felipe Haiashida

Site de portfólio estático, sem build, pronto para hospedar no GitHub Pages.

---

## 📁 Estrutura

```
seu-repositorio/
├── index.html       ← arquivo único do site
├── videos/          ← seus MP4s vão aqui
│   ├── projeto1.mp4
│   ├── projeto2.mp4
│   └── ...
└── README.md
```

---

## 🚀 Deploy no GitHub Pages (passo a passo)

### 1. Criar o repositório

1. Vá em [github.com/new](https://github.com/new) e crie um repositório **público**.
2. Pode usar qualquer nome — por exemplo `portfolio` ou `felipe-haiashida.github.io`.
   - Se usar o nome `seu-usuario.github.io`, o site fica em `https://seu-usuario.github.io/`.
   - Se usar outro nome, o site fica em `https://seu-usuario.github.io/nome-do-repo/`.

### 2. Subir os arquivos

**Opção A — pela interface web (mais fácil):**

1. Na página do repositório, clique em **Add file → Upload files**.
2. Arraste o `index.html` e a pasta `videos/` (com seus MP4s dentro).
3. Clique em **Commit changes**.

**Opção B — pelo terminal:**

```bash
git clone https://github.com/seu-usuario/seu-repo.git
cd seu-repo
# copie o index.html e a pasta videos/ para cá
git add .
git commit -m "primeira versão do portfólio"
git push
```

### 3. Ativar o GitHub Pages

1. No repositório, vá em **Settings → Pages**.
2. Em **Source**, escolha **Deploy from a branch**.
3. Em **Branch**, selecione **main** (ou `master`) e a pasta **/ (root)**.
4. Clique em **Save**.
5. Aguarde 1–2 minutos. O link do site aparecerá na mesma página.

✅ Pronto. Seu portfólio está no ar.

---

## ✏️ Como editar o conteúdo

O site tem um **modo de edição embutido** que funciona direto no navegador.

### Fluxo de edição

1. Abra o site (no GitHub Pages ou abrindo o `index.html` localmente).
2. Clique no botão **`✎ editar`** no canto superior direito.
3. Edite qualquer texto clicando nele e digitando por cima.
4. Adicione/remova projetos, experiências, habilidades.
5. Suas edições ficam salvas **no seu navegador** (localStorage) — você pode fechar e voltar depois.
6. Quando estiver satisfeito, clique em **`↓ baixar html`** — um novo `index.html` é baixado com tudo dentro.
7. Substitua o `index.html` no seu repositório do GitHub e dê commit. O site público é atualizado.

### Adicionar vídeos

Cada projeto suporta:

- **MP4 local** (recomendado): clique no botão **`↑ mp4`** no card do projeto, escolha o arquivo. Aparece um aviso laranja com o nome do arquivo — você precisa salvar esse MP4 na pasta `videos/` do repositório com **exatamente o mesmo nome**.
- **Caminho relativo manual**: digite no campo `link →` algo como `videos/meu-video.mp4`. Coloque o arquivo na pasta `videos/`.
- **YouTube**: cole a URL completa (`https://youtube.com/watch?v=...`).
- **Vimeo**: cole a URL (`https://vimeo.com/123456789`).
- **URL direto de MP4**: qualquer link `.mp4` público funciona.

⚠ **Importante**: o modo edição mostra prévias de MP4 locais usando o arquivo do seu computador, mas isso é **só para visualizar**. Para o vídeo aparecer no site público, você precisa **enviar o MP4 para a pasta `videos/` do repositório**.

### Workflow recomendado para adicionar um vídeo novo

1. Abra o site, ative o modo edição.
2. No projeto desejado, clique em `↑ mp4` e selecione o arquivo.
3. O sistema vai usar o nome `videos/seu-video.mp4` automaticamente.
4. Clique em **`↓ baixar html`** — vai aparecer um aviso com o nome do arquivo a salvar.
5. Faça o upload no GitHub:
   - Substitua o `index.html` no repositório.
   - Adicione o MP4 dentro da pasta `videos/`.
6. Commit. Aguarde ~1 minuto. Site atualizado.

---

## 🎨 Editar diretamente o código

Se preferir, você também pode editar o conteúdo abrindo `index.html` num editor de texto. Procure pelo bloco:

```js
// === DEFAULT_DATA_START ===
const DEFAULT_DATA = { ... };
// === DEFAULT_DATA_END ===
```

Tudo que está nesse objeto pode ser editado livremente — nome, descrição dos projetos, links, habilidades, etc. Não mexa nos comentários `DEFAULT_DATA_START` e `DEFAULT_DATA_END` — eles são usados pelo modo edição.

---

## 💡 Dicas

- **Tamanho dos vídeos**: o GitHub aceita arquivos de até 100 MB cada. Para vídeos maiores, comprima com [HandBrake](https://handbrake.fr/) ou hospede em outro lugar (Vimeo, YouTube unlisted, etc.) e cole o link.
- **Loading rápido**: vídeos MP4 devem ter resolução 720p ou 1080p, codec H.264. Use `ffmpeg` para otimizar:
  ```bash
  ffmpeg -i original.mp4 -vcodec h264 -acodec aac -crf 23 videos/projeto.mp4
  ```
- **Domínio próprio**: dá pra apontar um domínio como `felipehaiashida.com` para o GitHub Pages. Em **Settings → Pages → Custom domain**.

---

## 🛠 Troubleshooting

**Editei o site mas as mudanças sumiram quando troquei de navegador.**
Normal — o modo edição salva no localStorage do seu navegador. Para tornar permanente e visível para todo mundo, você precisa baixar o HTML e dar commit no repositório.

**O vídeo aparece quando estou editando, mas não aparece no site público.**
Provavelmente o MP4 ainda não foi enviado para a pasta `videos/` do repositório. Confira se o arquivo tem o mesmo nome que o campo `link →` do projeto.

**Quero começar do zero.**
Clique no botão **`↺ reset`** no modo edição. Confirma e tudo volta ao estado original.
