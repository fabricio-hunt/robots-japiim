# 🤖 Robots.txt — SEO + LLMs + Social Crawlers

Este repositório contém a configuração oficial do **robots.txt** do site  
👉 **https://japiim.com.br**

O objetivo é **permitir indexação e leitura por buscadores, LLMs e bots de preview**, ao mesmo tempo em que **bloqueia crawlers abusivos e protege áreas sensíveis** da aplicação.

---

## 🎯 Objetivos da configuração

- ✅ Otimização para **SEO tradicional** (Google, Bing)
- ✅ Disponibilização clara para **LLMs / IA** (ChatGPT, Claude, Perplexity, OpenAI Search)
- ✅ Suporte a **bots de redes sociais** (preview de links)
- ❌ Bloqueio de bots conhecidos por **scraping agressivo**
- 🔒 Proteção de rotas privadas e administrativas
- 🌐 Compatível com **SPA (Vue.js)** + **API (FastAPI)**

---

## 🤖 Bots explicitamente PERMITIDOS

### 🔍 Buscadores
- Googlebot
- Bingbot
- BingPreview

### 🧠 LLMs / IA
- GPTBot
- OAI-SearchBot
- ClaudeBot
- Claude-Web
- PerplexityBot

### 📣 Social / Preview
- FacebookExternalHit
- FacebookBot
- Twitterbot
- LinkedInBot

### 🛠️ SEO
- Screaming Frog SEO Spider

---

## 🚫 Bots explicitamente BLOQUEADOS

Os bots abaixo são conhecidos por **scraping agressivo**, uso comercial não autorizado ou consumo excessivo de recursos:

- EtaoSpider
- CCBot (Common Crawl)
- Amazonbot
- FacebookBot-Mobile
- Bytespider (ByteDance)
- PetalBot (Huawei)

---

## 🔒 Rotas protegidas (para todos os bots)

Mesmo bots permitidos **não podem acessar**:

```txt
/auth/
/admin/
/private/
/api/
