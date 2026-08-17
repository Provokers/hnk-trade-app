# Heineken × Provokers · Trade Toolkit (PWA v0)

App instalável (Progressive Web App) do playbook de trade para bares & restaurantes.
Roda offline, instala como ícone no celular e filtra o conteúdo por perfil (Vendas, Trade, Dono de Bar).

## 📦 Conteúdo do pacote
```
index.html                → o app completo (HTML/CSS/JS + logos embutidos)
manifest.json             → identidade do PWA (nome, cores, ícones)
sw.js                     → service worker (funciona offline)
icon-192.png              → ícone do app
icon-512.png              → ícone do app (alta resolução)
icon-maskable-512.png     → ícone adaptável (Android)
apple-touch-icon.png      → ícone para iPhone/iPad
favicon-32.png            → favicon do navegador
```
> **Importante:** mantenha todos os arquivos na **mesma pasta**. Os caminhos são relativos (`./`), então funciona tanto na raiz quanto em subpasta do GitHub Pages.

## 🚀 Deploy no GitHub Pages
1. Suba **todos** os arquivos acima para o repositório (raiz ou pasta `/docs`).
2. Vá em **Settings → Pages**.
3. Em *Source*, escolha a branch (`main`) e a pasta (`/root` ou `/docs`).
4. Salve. Em ~1 min o app estará em `https://SEU-USUARIO.github.io/SEU-REPO/`.
5. O PWA só instala em **HTTPS** — o GitHub Pages já entrega HTTPS. ✅

## 📱 Como instalar no celular
- **Android (Chrome):** aparece o botão de instalar no topo do app, ou menu ⋮ → *Instalar app*.
- **iPhone (Safari):** botão *Compartilhar* → *Adicionar à Tela de Início*.
- Depois de instalado, abre em tela cheia e funciona **sem internet**.

## 🔄 Atualizando o conteúdo
Todo o conteúdo vive em objetos JavaScript dentro do `index.html`
(`PROFILES`, `TABS`, `SECTIONS`, `DOWNLOADS`, `BEERS`).
Para editar textos/dados, basta alterar esses objetos — nenhuma outra parte do código precisa mudar.

> **Evolução sugerida (produção):** externalizar esses objetos para um `content.json`
> e carregá-lo via `fetch()`. Assim o time de Marketing atualiza os playbooks sem mexer no código.

## ⚠️ Placeholders a substituir na versão final
- Fotos reais de "Loja Perfeita" (hoje há placeholders responsivos).
- Valores de **preço (PSC)** e **KPIs** — atualmente ilustrativos para a v0.
- Links reais dos arquivos do **Download Center** (hoje em modo demo).

---
© 2026 · Documento confidencial · Uso interno rede parceira · Heineken × Provokers
