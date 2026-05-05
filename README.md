# Felipe Haiashida — Portfólio

Portfólio pessoal de **Felipe Haiashida Carvalho**, desenvolvedor de aplicações imersivas em Realidade Virtual (VR) e Realidade Aumentada (AR), graduando em Ciência da Computação pelo IFCE.

O site reúne os principais projetos educacionais imersivos desenvolvidos com Unity, Meta SDK e XR Interaction Toolkit, além de experiência profissional, formação acadêmica e stack técnica.

🌐 **Acesse:** _publique no GitHub Pages e adicione o link aqui_

---

## 👤 Sobre

Desenvolvedor focado em **soluções educacionais interativas**, com aplicações testadas em escolas públicas e eventos acadêmicos, promovendo a democratização do acesso a tecnologias imersivas. Atua em liderança técnica, mentoria em Web 3.0, prototipagem rápida, design de interfaces para VR e otimização de desempenho para dispositivos standalone.

- 📍 Fortaleza — CE, Brasil
- ✉ felipehaiashida@gmail.com
- ☎ +55 (85) 99439-4479
- 🔗 [GitHub](https://github.com/felipehaiashida) · [LinkedIn](https://www.linkedin.com/in/felipe-haiashida-carvalho-0b7b9919a/)

---

## 🧪 Projetos em destaque

### 1. Rede de Experimentos Remotos para a Educação do Brasil — 2025
Plataforma educacional em VR para experimentos científicos interativos. Inclui simulação realista de pêndulo físico com modelagem matemática aplicada. Arquitetura modular pensada para escalar a outras disciplinas, com foco em escolas com acesso limitado a laboratórios físicos.

> Stack: Unity · XR Interaction Toolkit · C#

### 2. Laboratório Virtual de História — 2025
Museu virtual interativo para o ensino fundamental, com ambientes imersivos inspirados no Egito Antigo e na Roma Antiga. Interações baseadas em manipulação de objetos e exploração espacial, aplicando princípios de gamificação e aprendizagem experiencial.

> Stack: Unity · VR · Meta SDK · Gamificação

### 3. Aplicações VR/AR — Huawei ICT Academy — 2024 / Atual
Desenvolvimento de aplicações VR e AR em Unity com foco em usabilidade, performance e interatividade. Interfaces imersivas com XR Interaction Toolkit e Meta SDK, prototipagem e testes em dispositivos standalone (Meta Quest), além de demonstrações técnicas em workshops.

> Stack: Unity · Meta Quest · XR Toolkit · AR

---

## 💼 Experiência

| Período | Posição | Organização |
|---|---|---|
| Jul 2024 — Atual | Estagiário — Desenvolvimento VR/AR | Huawei ICT Academy · IFCE |
| 2026 | Mentor — Curso de Web 3.0 (Trilha Metaverso) | Irede · Fortaleza |
| Set 2024 | Palestrante — VR, AR e Realidade Mista na Educação | Semana de Engenharia · UFC |

---

## 🛠 Stack técnica

- **Engines e XR**: Unity 3D (2022/2023 LTS, 6.0), XR Interaction Toolkit, Meta SDK, OpenXR
- **Programação**: C#, Python
- **Build e Deploy**: Android (APK), otimização para dispositivos standalone
- **Interação e UI**: Interfaces imersivas, mecânicas de interação 3D, gamificação educacional
- **Banco de Dados**: MySQL
- **Controle de Versão**: Git, GitHub
- **Ferramentas**: VSCode, Eclipse

---

## 🎓 Formação

- **Bacharelado em Ciência da Computação** — IFCE · 2023 — 2027
- **Mentoria Técnica em Tecnologias Huawei** — Huawei ICT Academy · IFCE · 2024
- **Liderança Técnica — Habilidades para Inspirar e Transformar Equipes** — Rocketseat · Out 2025

---

## 🌍 Idiomas

- Português — Nativo
- Inglês — Leitura/escuta avançadas, conversação intermediária

---

## 📁 Estrutura do repositório

```
.
├── index.html       ← site estático (HTML único, sem build)
├── videos/          ← demos dos projetos em MP4
│   ├── video1.mp4   ← Rede de Experimentos Remotos
│   ├── video2.mp4   ← Laboratório Virtual de História
│   └── video3.mp4   ← Aplicações VR/AR — Huawei ICT Academy
└── README.md
```

O site é uma única página HTML, renderizada por JavaScript a partir de um objeto `DATA` no próprio arquivo. Usa **Tailwind (via CDN)** e as fontes **Fraunces** e **JetBrains Mono** do Google Fonts.

---

## 🚀 Rodar localmente

> ⚠ **Importante:** abrir o `index.html` com duplo-clique (`file://`) faz com que os navegadores bloqueiem os vídeos por política de segurança. Use um servidor HTTP local:

```bash
# Python (já vem instalado no Windows/macOS/Linux)
python -m http.server 8000

# Node (alternativa)
npx serve
```

Depois, acesse `http://localhost:8000` no navegador. Os vídeos passam a tocar normalmente.

No VSCode, a extensão **Live Server** (Ritwick Dey) também resolve com um clique direito → "Open with Live Server".

---

## ☁ Deploy (GitHub Pages)

1. Suba o repositório para o GitHub.
2. Em **Settings → Pages**, selecione a branch `main` e a pasta `/ (root)`.
3. Aguarde alguns instantes — o site fica disponível em `https://<seu-usuario>.github.io/<repo>/`.

> ⚠ Vídeos com mais de 100 MB excedem o limite por arquivo do GitHub. Para hospedar vídeos maiores, comprima com `ffmpeg` ou use YouTube/Vimeo (o site suporta links nativamente).

---

© Felipe Haiashida · Fortaleza · Brasil
