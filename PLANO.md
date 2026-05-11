# PLANO DO PROJETO: assistente-juridico-expo (2)

> Gerado automaticamente pelo SK Code Editor em 09/05/2026, 22:54:51
> **136 arquivo(s)** | **~41.082 linhas de codigo**

---

## RESUMO EXECUTIVO

- **Tipo de aplicacao:** Full-Stack (React + Express)
- **Frontend / Stack principal:** React + Vite, TypeScript, Tailwind CSS, Python
- **Backend / Dados:** Node.js + Express, PostgreSQL, Drizzle ORM
- **Versao:** 1.0.0

**Para rodar o projeto:**
```bash
npm install && npm run dev
```

---

## ESTRUTURA DE ARQUIVOS

```
assistente-juridico-expo (2)/
├── .sk/
│   └── memoria.json
├── api/
│   └── .ts
├── client/
│   ├── public/
│   │   ├── auditoria.html
│   │   ├── codigo-formatacao.txt
│   │   ├── comparador.html
│   │   ├── manifest.json
│   │   └── sw.js
│   ├── replit_integrations/
│   │   └── audio/
│   │       ├── audio-playback-worklet.js
│   │       ├── audio-utils.ts
│   │       ├── index.ts
│   │       ├── useAudioPlayback.ts
│   │       ├── useVoiceRecorder.ts
│   │       └── useVoiceStream.ts
│   ├── src/
│   │   ├── components/
│   │   │   ├── ui/
│   │   │   │   ├── accordion.tsx
│   │   │   │   ├── alert-dialog.tsx
│   │   │   │   ├── alert.tsx
│   │   │   │   ├── aspect-ratio.tsx
│   │   │   │   ├── avatar.tsx
│   │   │   │   ├── badge.tsx
│   │   │   │   ├── breadcrumb.tsx
│   │   │   │   ├── button.tsx
│   │   │   │   ├── calendar.tsx
│   │   │   │   ├── card.tsx
│   │   │   │   ├── carousel.tsx
│   │   │   │   ├── chart.tsx
│   │   │   │   ├── checkbox.tsx
│   │   │   │   ├── collapsible.tsx
│   │   │   │   ├── command.tsx
│   │   │   │   ├── context-menu.tsx
│   │   │   │   ├── dialog.tsx
│   │   │   │   ├── drawer.tsx
│   │   │   │   ├── dropdown-menu.tsx
│   │   │   │   ├── form.tsx
│   │   │   │   ├── hover-card.tsx
│   │   │   │   ├── input-otp.tsx
│   │   │   │   ├── input.tsx
│   │   │   │   ├── label.tsx
│   │   │   │   ├── menubar.tsx
│   │   │   │   ├── navigation-menu.tsx
│   │   │   │   ├── pagination.tsx
│   │   │   │   ├── popover.tsx
│   │   │   │   ├── progress.tsx
│   │   │   │   ├── radio-group.tsx
│   │   │   │   ├── resizable.tsx
│   │   │   │   ├── scroll-area.tsx
│   │   │   │   ├── select.tsx
│   │   │   │   ├── separator.tsx
│   │   │   │   ├── sheet.tsx
│   │   │   │   ├── sidebar.tsx
│   │   │   │   ├── skeleton.tsx
│   │   │   │   ├── slider.tsx
│   │   │   │   ├── switch.tsx
│   │   │   │   ├── table.tsx
│   │   │   │   ├── tabs.tsx
│   │   │   │   ├── textarea.tsx
│   │   │   │   ├── toast.tsx
│   │   │   │   ├── toaster.tsx
│   │   │   │   ├── toggle-group.tsx
│   │   │   │   ├── toggle.tsx
│   │   │   │   └── tooltip.tsx
│   │   │   ├── pwa-install.tsx
│   │   │   ├── theme-provider.tsx
│   │   │   ├── theme-toggle.tsx
│   │   │   └── tiptap-editor.tsx
│   │   ├── hooks/
│   │   │   ├── use-mobile.tsx
│   │   │   └── use-toast.ts
│   │   ├── lib/
│   │   │   ├── queryClient.ts
│   │   │   └── utils.ts
│   │   ├── pages/
│   │   │   ├── auditoria-financeira.tsx
│   │   │   ├── code-assistant.tsx
│   │   │   ├── comparador-juridico.tsx
│   │   │   ├── comunicacoes-cnj.tsx
│   │   │   ├── configuracoes.tsx
│   │   │   ├── consulta-corporativo.tsx
│   │   │   ├── consulta-pdpj.tsx
│   │   │   ├── consulta-processual.tsx
│   │   │   ├── filtrador.tsx
│   │   │   ├── jurisprudencia.tsx
│   │   │   ├── legal-assistant.tsx
│   │   │   ├── legal-assistant.tsx.recovered
│   │   │   ├── login.tsx
│   │   │   ├── not-found.tsx
│   │   │   ├── painel-processos.tsx
│   │   │   ├── playground.tsx
│   │   │   ├── previdenciario.tsx
│   │   │   ├── robo-djen.tsx
│   │   │   ├── token-generator.tsx
│   │   │   └── tramitacao.tsx
│   │   ├── App.tsx
│   │   ├── index.css
│   │   └── main.tsx
│   ├── api.ts
│   ├── index.html
│   └── index.ts
├── migrations/
│   ├── meta/
│   │   ├── _journal.json
│   │   └── 0000_snapshot.json
│   └── 0000_init.sql
├── public/
│   └── auditoria.html
├── script/
│   └── build.ts
├── server/
│   ├── replit_integrations/
│   │   ├── audio/
│   │   │   ├── client.ts
│   │   │   ├── index.ts
│   │   │   └── routes.ts
│   │   ├── batch/
│   │   │   ├── index.ts
│   │   │   └── utils.ts
│   │   ├── chat/
│   │   │   ├── index.ts
│   │   │   ├── routes.ts
│   │   │   └── storage.ts
│   │   └── image/
│   │       ├── client.ts
│   │       ├── index.ts
│   │       └── routes.ts
│   ├── db.ts
│   ├── djen.ts
│   ├── index.ts
│   ├── local-config.ts
│   ├── routes.ts
│   ├── static.ts
│   ├── storage.ts
│   └── vite.ts
├── shared/
│   ├── models/
│   │   └── chat.ts
│   └── schema.ts
├── .gitignore
├── app.json
├── App.tsx
├── babel.config.js
├── COMO_BUILDAR.md
├── components.json
├── drizzle.config.ts
├── eas.json
├── fix_buttons.txt
├── main.py
├── package.json
├── postcss.config.js
├── pyproject.toml
├── tailwind.config.ts
├── tsconfig.json
└── vite.config.ts
```

---

## STACK TECNOLOGICO DETECTADO

- **Frontend:** React + Vite, TypeScript, Tailwind CSS, Python
- **Backend:** Node.js + Express, PostgreSQL, Drizzle ORM
- **Todos os pacotes (116):** @google/genai, @hookform/resolvers, @jridgewell/trace-mapping, @radix-ui/react-accordion, @radix-ui/react-alert-dialog, @radix-ui/react-aspect-ratio, @radix-ui/react-avatar, @radix-ui/react-checkbox, @radix-ui/react-collapsible, @radix-ui/react-context-menu, @radix-ui/react-dialog, @radix-ui/react-dropdown-menu, @radix-ui/react-hover-card, @radix-ui/react-label, @radix-ui/react-menubar, @radix-ui/react-navigation-menu, @radix-ui/react-popover, @radix-ui/react-progress, @radix-ui/react-radio-group, @radix-ui/react-scroll-area, @radix-ui/react-select, @radix-ui/react-separator, @radix-ui/react-slider, @radix-ui/react-slot, @radix-ui/react-switch, @radix-ui/react-tabs, @radix-ui/react-toast, @radix-ui/react-toggle, @radix-ui/react-toggle-group, @radix-ui/react-tooltip, @tanstack/react-query, @tiptap/extension-color, @tiptap/extension-font-family, @tiptap/extension-highlight, @tiptap/extension-link, @tiptap/extension-table, @tiptap/extension-table-cell, @tiptap/extension-table-header, @tiptap/extension-table-row, @tiptap/extension-text-align, @tiptap/extension-text-style, @tiptap/extension-underline, @tiptap/pm, @tiptap/react, @tiptap/starter-kit, @types/jsonwebtoken, @types/multer, adm-zip, axios, class-variance-authority, clsx, cmdk, connect-pg-simple, date-fns, docx, drizzle-orm, drizzle-zod, embla-carousel-react, express, express-session, framer-motion, html-entities, input-otp, jsonwebtoken, lucide-react, mammoth, memorystore, multer, next-themes, openai, p-limit, p-retry, passport, passport-local, pdf-parse, pdfjs-dist, pg, postcss-selector-parser, react, react-day-picker, react-dom, react-hook-form, react-icons, react-resizable-panels, recharts, tailwind-merge, tailwindcss-animate, tw-animate-css, vaul, wouter, ws, zod, zod-validation-error, @replit/vite-plugin-cartographer, @replit/vite-plugin-dev-banner, @replit/vite-plugin-runtime-error-modal, @tailwindcss/typography, @tailwindcss/vite, @types/connect-pg-simple, @types/express, @types/express-session, @types/node, @types/passport, @types/passport-local, @types/react, @types/react-dom, @types/ws, @vitejs/plugin-react, autoprefixer, drizzle-kit, esbuild, postcss, tailwindcss, tsx, typescript, vite

---

## ROTAS DA API (endpoints detectados automaticamente)

```
GET    /api/conversations  (em server/replit_integrations/audio/routes.ts)
GET    /api/conversations/:id  (em server/replit_integrations/audio/routes.ts)
POST   /api/conversations  (em server/replit_integrations/audio/routes.ts)
DELETE /api/conversations/:id  (em server/replit_integrations/audio/routes.ts)
POST   /api/conversations/:id/messages  (em server/replit_integrations/audio/routes.ts)
GET    /api/conversations  (em server/replit_integrations/chat/routes.ts)
GET    /api/conversations/:id  (em server/replit_integrations/chat/routes.ts)
POST   /api/conversations  (em server/replit_integrations/chat/routes.ts)
DELETE /api/conversations/:id  (em server/replit_integrations/chat/routes.ts)
POST   /api/conversations/:id/messages  (em server/replit_integrations/chat/routes.ts)
POST   /api/generate-image  (em server/replit_integrations/image/routes.ts)
GET    /sw.js  (em server/routes.ts)
GET    /api/auth/check  (em server/routes.ts)
POST   /api/auth/login  (em server/routes.ts)
POST   /api/auth/logout  (em server/routes.ts)
GET    /parecer/:id  (em server/routes.ts)
GET    /api/tjmg/fatores  (em server/routes.ts)
POST   /api/pdpj/test-connection  (em server/routes.ts)
GET    /api/pdpj/status  (em server/routes.ts)
POST   /api/pdpj/comunicacoes  (em server/routes.ts)
POST   /api/pdpj/representados  (em server/routes.ts)
POST   /api/pdpj/habilitacao  (em server/routes.ts)
POST   /api/pdpj/pessoa  (em server/routes.ts)
POST   /api/webhooks/tramitacao  (em server/routes.ts)
GET    /api/demo-key-status  (em server/routes.ts)
GET    /api/demo-key-config  (em server/routes.ts)
POST   /api/demo-key-config  (em server/routes.ts)
GET    /api/perplexity-key-status  (em server/routes.ts)
POST   /api/demo-key-test  (em server/routes.ts)
POST   /api/tts  (em server/routes.ts)
POST   /api/voice-chat  (em server/routes.ts)
USE    /api  (em server/routes.ts)
POST   /api/share/parecer  (em server/routes.ts)
GET    /api/snippets  (em server/routes.ts)
GET    /api/snippets/:id  (em server/routes.ts)
POST   /api/snippets  (em server/routes.ts)
PATCH  /api/snippets/:id  (em server/routes.ts)
DELETE /api/snippets/:id  (em server/routes.ts)
GET    /api/custom-actions  (em server/routes.ts)
POST   /api/custom-actions  (em server/routes.ts)
PATCH  /api/custom-actions/:id  (em server/routes.ts)
DELETE /api/custom-actions/:id  (em server/routes.ts)
GET    /api/ementas  (em server/routes.ts)
POST   /api/ementas  (em server/routes.ts)
PATCH  /api/ementas/:id  (em server/routes.ts)
DELETE /api/ementas/:id  (em server/routes.ts)
POST   /api/jurisprudencia/buscar  (em server/routes.ts)
GET    /api/ai-history  (em server/routes.ts)
POST   /api/ai-history  (em server/routes.ts)
DELETE /api/ai-history/:id  (em server/routes.ts)
DELETE /api/ai-history  (em server/routes.ts)
GET    /api/ai-usage-summary  (em server/routes.ts)
POST   /api/ai-usage-credit  (em server/routes.ts)
GET    /api/prompt-templates  (em server/routes.ts)
POST   /api/prompt-templates  (em server/routes.ts)
PATCH  /api/prompt-templates/:id  (em server/routes.ts)
DELETE /api/prompt-templates/:id  (em server/routes.ts)
GET    /api/doc-templates  (em server/routes.ts)
POST   /api/doc-templates  (em server/routes.ts)
PATCH  /api/doc-templates/:id  (em server/routes.ts)
DELETE /api/doc-templates/:id  (em server/routes.ts)
POST   /api/doc-templates/upload-docx  (em server/routes.ts)
POST   /api/export/word-with-template  (em server/routes.ts)
POST   /api/import/url  (em server/routes.ts)
POST   /api/upload/extract-text  (em server/routes.ts)
POST   /api/upload/transcribe  (em server/routes.ts)
POST   /api/ai/process  (em server/routes.ts)
POST   /api/ai/refine  (em server/routes.ts)
POST   /api/export/word  (em server/routes.ts)
POST   /api/jwt/generate  (em server/routes.ts)
GET    /api/jwt/status  (em server/routes.ts)
GET    /api/processos  (em server/routes.ts)
GET    /api/processos/:id  (em server/routes.ts)
POST   /api/processos  (em server/routes.ts)
PATCH  /api/processos/:id  (em server/routes.ts)
DELETE /api/processos/:id  (em server/routes.ts)
POST   /api/datajud/consulta  (em server/routes.ts)
POST   /api/datajud/consulta-oab  (em server/routes.ts)
GET    /api/corporativo/advogado/cpf/:cpf  (em server/routes.ts)
GET    /api/corporativo/advogado/oab/:uf/:inscricao  (em server/routes.ts)
GET    /api/corporativo/magistrados/:tribunal  (em server/routes.ts)
GET    /api/pdpj/status  (em server/routes.ts)
POST   /api/pdpj/test-connection  (em server/routes.ts)
POST   /api/pdpj/comunicacoes  (em server/routes.ts)
POST   /api/pdpj/representados  (em server/routes.ts)
POST   /api/pdpj/habilitacao  (em server/routes.ts)
POST   /api/pdpj/pessoa  (em server/routes.ts)
GET    /api/datajud/tribunais  (em server/routes.ts)
POST   /api/cnj/comunicacoes  (em server/routes.ts)
GET    /api/cnj/comunicacoes/certidao/:hash  (em server/routes.ts)
GET    /api/settings/:key  (em server/routes.ts)
PUT    /api/settings/:key  (em server/routes.ts)
GET    /api/settings/ai-config  (em server/routes.ts)
PUT    /api/settings/ai-config  (em server/routes.ts)
POST   /api/settings/database-reconnect  (em server/routes.ts)
GET    /api/settings/database-status  (em server/routes.ts)
GET    /api/settings/system-status  (em server/routes.ts)
PUT    /api/settings/app-password  (em server/routes.ts)
PUT    /api/settings/session-secret  (em server/routes.ts)
POST   /api/settings/test-ai-key  (em server/routes.ts)
GET    /api/tramitacao/clientes  (em server/routes.ts)
POST   /api/tramitacao/clientes  (em server/routes.ts)
GET    /api/tramitacao/clientes/:id  (em server/routes.ts)
PATCH  /api/tramitacao/clientes/:id  (em server/routes.ts)
GET    /api/tramitacao/notas  (em server/routes.ts)
POST   /api/tramitacao/notas  (em server/routes.ts)
DELETE /api/tramitacao/notas/:id  (em server/routes.ts)
GET    /api/tramitacao/usuarios  (em server/routes.ts)
GET    /api/tramitacao/test  (em server/routes.ts)
GET    /api/tramitacao/publicacoes  (em server/routes.ts)
POST   /api/tramitacao/sync-publicacoes  (em server/routes.ts)
PATCH  /api/tramitacao/publicacoes/:id/lida  (em server/routes.ts)
POST   /api/code/run  (em server/routes.ts)
POST   /api/previdenciario/extrair  (em server/routes.ts)
GET    /api/pesquisa/oab  (em server/routes.ts)
GET    /api/pesquisa/processo  (em server/routes.ts)
GET    /api/djen/config  (em server/routes.ts)
PUT    /api/djen/config  (em server/routes.ts)
GET    /api/djen/clientes  (em server/routes.ts)
POST   /api/djen/clientes  (em server/routes.ts)
DELETE /api/djen/clientes/:id  (em server/routes.ts)
GET    /api/djen/publicacoes  (em server/routes.ts)
GET    /api/djen/execucoes  (em server/routes.ts)
POST   /api/djen/executar  (em server/routes.ts)
POST   /api/djen/gerar-token  (em server/routes.ts)
POST   /api/code-assistant  (em server/routes.ts)
POST   /api/git-push  (em server/routes.ts)
USE    /sw.js  (em server/static.ts)
USE    /manifest.json  (em server/static.ts)
USE    /{*path}  (em server/static.ts)
USE    /{*path}  (em server/vite.ts)
```

---

## SCRIPTS DISPONIVEIS (package.json)

```bash
npm run dev           # NODE_ENV=development tsx server/index.ts
npm run build         # tsx script/build.ts
npm run start         # NODE_ENV=production node dist/index.cjs
npm run check         # tsc
npm run db:push       # drizzle-kit push
```

---

## VARIAVEIS DE AMBIENTE NECESSARIAS

Crie um arquivo `.env` na raiz com estas variaveis:

```env
DATABASE_URL=seu_valor_aqui
SESSION_SECRET=seu_valor_aqui
PORT=seu_valor_aqui
APP_PASSWORD=seu_valor_aqui
AI_INTEGRATIONS_OPENAI_API_KEY=seu_valor_aqui
AI_INTEGRATIONS_OPENAI_BASE_URL=seu_valor_aqui
PUBLIC_API_KEY=seu_valor_aqui
AI_INTEGRATIONS_GEMINI_API_KEY=seu_valor_aqui
AI_INTEGRATIONS_GEMINI_BASE_URL=seu_valor_aqui
PDPJ_PEM_PRIVATE_KEY=seu_valor_aqui
PUBLIC_API_MODEL=seu_valor_aqui
PUBLIC_API_URL=seu_valor_aqui
DATAJUD_API_KEY=seu_valor_aqui
PERPLEXITY_API_KEY=seu_valor_aqui
```

---

## ARQUIVOS PRINCIPAIS

- `App.tsx` — Componente raiz do frontend
- `client/index.html` — Arquivo principal
- `client/index.ts` — Arquivo principal
- `client/replit_integrations/audio/index.ts` — Arquivo principal
- `client/src/App.tsx` — Componente raiz do frontend
- `client/src/main.tsx` — Arquivo principal
- `main.py` — Aplicacao Python principal
- `server/index.ts` — Ponto de entrada do backend
- `server/replit_integrations/audio/index.ts` — Ponto de entrada do backend
- `server/replit_integrations/batch/index.ts` — Ponto de entrada do backend

---

## GUIA COMPLETO — O QUE CADA PARTE DO PROJETO FAZ

> Esta secao explica, em linguagem simples, o que e para que serve cada pasta e cada arquivo.

### 📁 Raiz do Projeto (pasta principal)
> Arquivos de configuracao e pontos de entrada ficam aqui.

**`.gitignore`** _(6 linhas)_
Lista de arquivos/pastas que o Git deve IGNORAR (nao versionar). Ex: node_modules, .env

**`App.tsx`** _(114 linhas)_
Componente RAIZ do frontend — e o pai de todos os outros componentes. Aqui ficam as rotas principais.

**`COMO_BUILDAR.md`** _(71 linhas)_
Arquivo de documentacao em Markdown (texto formatado com #titulos, **negrito**, listas).

**`app.json`** _(47 linhas)_
Arquivo de dados ou configuracao no formato JSON (chave: valor).

**`babel.config.js`** _(7 linhas)_
Arquivo de CONSTANTES/CONFIGURACAO — valores fixos usados em varios lugares do projeto.

**`components.json`** _(20 linhas)_
Arquivo de dados ou configuracao no formato JSON (chave: valor).

**`drizzle.config.ts`** _(15 linhas)_
Configuracao do Drizzle ORM — gerencia a conexao e migracao do banco de dados.

**`eas.json`** _(26 linhas)_
Arquivo de dados ou configuracao no formato JSON (chave: valor).

**`fix_buttons.txt`** _(64 linhas)_
Arquivo TXT — parte do projeto.

**`main.py`** _(7 linhas)_
Arquivo Python — codigo de logica ou script de automacao.

**`package.json`** _(142 linhas)_
Registro de dependencias e scripts do projeto. Aqui ficam os comandos (npm run dev, npm start) e os pacotes instalados.

**`postcss.config.js`** _(7 linhas)_
Configuracao do PostCSS, necessaria para o Tailwind processar os estilos.

**`pyproject.toml`** _(9 linhas)_
Arquivo TOML — parte do projeto.

**`tailwind.config.ts`** _(108 linhas)_
Configuracao do Tailwind CSS — a biblioteca de estilos visuais usada no projeto.

**`tsconfig.json`** _(24 linhas)_
Configuracao do TypeScript. Diz para o computador como interpretar o codigo .ts e .tsx.

**`vite.config.ts`** _(39 linhas)_
Configuracao do Vite (servidor de desenvolvimento). Define a porta, alias de caminhos e plugins usados.

---

### 📁 `.sk/`
> Pasta '.sk' — agrupamento de arquivos relacionados.

**`memoria.json`** _(1 linha)_
Arquivo de dados ou configuracao no formato JSON (chave: valor).

---

### 📁 `api/`
> Comunicacao com servidor, banco de dados ou APIs externas.

**`.ts`** _(1 linha)_
Arquivo TypeScript/JavaScript — logica, funcoes ou modulo do projeto.

---

### 📁 `client/`
> Pasta 'client' — agrupamento de arquivos relacionados.

**`api.ts`** _(1 linha)_
Arquivo de SERVICO/API — funcoes para comunicar com o servidor ou API externa.

**`index.html`** _(31 linhas)_
Pagina HTML raiz do projeto. E o ponto de entrada que o browser carrega primeiro.

**`index.ts`** _(47 linhas)_
Arquivo INDEX — ponto de entrada da pasta, exporta tudo que esta dentro.

---

### 📁 `migrations/`
> Historico de alteracoes do banco de dados.

**`0000_init.sql`** _(141 linhas)_
Script SQL — contem comandos para criar tabelas, inserir ou consultar dados no banco.

---

### 📁 `public/`
> Arquivos estaticos: imagens, icones, fontes, arquivos publicos.

**`auditoria.html`** _(35 linhas)_
Arquivo HTML — parte do projeto.

---

### 📁 `script/`
> Pasta 'script' — agrupamento de arquivos relacionados.

**`build.ts`** _(71 linhas)_
Arquivo TypeScript/JavaScript — logica, funcoes ou modulo do projeto.

---

### 📁 `server/`
> Pasta 'server' — agrupamento de arquivos relacionados.

**`db.ts`** _(2 linhas)_
Arquivo TypeScript/JavaScript — logica, funcoes ou modulo do projeto.

**`djen.ts`** _(384 linhas)_
Arquivo TypeScript/JavaScript — logica, funcoes ou modulo do projeto.

**`index.ts`** _(196 linhas)_
Arquivo INDEX — ponto de entrada da pasta, exporta tudo que esta dentro.

**`local-config.ts`** _(67 linhas)_
Arquivo de CONSTANTES/CONFIGURACAO — valores fixos usados em varios lugares do projeto.

**`routes.ts`** _(5980 linhas)_
Arquivo de ROTAS — define as URLs/enderecos respondidos pelo servidor.

**`static.ts`** _(31 linhas)_
Arquivo TypeScript/JavaScript — logica, funcoes ou modulo do projeto.

**`storage.ts`** _(460 linhas)_
Arquivo TypeScript/JavaScript — logica, funcoes ou modulo do projeto.

**`vite.ts`** _(56 linhas)_
Arquivo TypeScript/JavaScript — logica, funcoes ou modulo do projeto.

---

### 📁 `shared/`
> Pasta 'shared' — agrupamento de arquivos relacionados.

**`schema.ts`** _(267 linhas)_
Arquivo de MODELO — define a estrutura dos dados (tabelas, campos, tipos).

---

### 📁 `client/public/`
> Arquivos estaticos: imagens, icones, fontes, arquivos publicos.

**`auditoria.html`** _(259 linhas)_
Arquivo HTML — parte do projeto.

**`codigo-formatacao.txt`** _(123 linhas)_
Arquivo TXT — parte do projeto.

**`comparador.html`** _(494 linhas)_
Arquivo HTML — parte do projeto.

**`manifest.json`** _(53 linhas)_
Manifesto do PWA — define nome, icone e configuracoes para instalar o app no celular.

**`sw.js`** _(58 linhas)_
Arquivo TypeScript/JavaScript — logica, funcoes ou modulo do projeto.

---

### 📁 `client/src/`
> Codigo-fonte principal do projeto. Nao apague esta pasta.

**`App.tsx`** _(183 linhas)_
Componente RAIZ do frontend — e o pai de todos os outros componentes. Aqui ficam as rotas principais.

**`index.css`** _(351 linhas)_
Arquivo de estilos visuais — cores, tamanhos, fontes, espacamentos da interface.

**`main.tsx`** _(12 linhas)_
Ponto de entrada do React — monta o componente App na pagina HTML.

---

### 📁 `migrations/meta/`
> Pasta 'meta' — agrupamento de arquivos relacionados.

**`0000_snapshot.json`** _(871 linhas)_
Arquivo de dados ou configuracao no formato JSON (chave: valor).

**`_journal.json`** _(13 linhas)_
Arquivo de dados ou configuracao no formato JSON (chave: valor).

---

### 📁 `shared/models/`
> Modelos de dados — representacao das tabelas do banco de dados.

**`chat.ts`** _(35 linhas)_
Arquivo TypeScript/JavaScript — logica, funcoes ou modulo do projeto.

---

### 📁 `client/replit_integrations/audio/`
> Pasta 'audio' — agrupamento de arquivos relacionados.

**`audio-playback-worklet.js`** _(113 linhas)_
Arquivo TypeScript/JavaScript — logica, funcoes ou modulo do projeto.

**`audio-utils.ts`** _(37 linhas)_
Funcoes UTILITARIAS — ferramentas reutilizaveis de uso geral no projeto.

**`index.ts`** _(46 linhas)_
Arquivo INDEX — ponto de entrada da pasta, exporta tudo que esta dentro.

**`useAudioPlayback.ts`** _(106 linhas)_
HOOK React personalizado para gerenciar estado/comportamento de 'audioplayback'.

**`useVoiceRecorder.ts`** _(53 linhas)_
HOOK React personalizado para gerenciar estado/comportamento de 'voicerecorder'.

**`useVoiceStream.ts`** _(92 linhas)_
HOOK React personalizado para gerenciar estado/comportamento de 'voicestream'.

---

### 📁 `client/src/components/`
> Pecas visuais reutilizaveis da interface (botoes, cards, formularios...).

**`pwa-install.tsx`** _(86 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`theme-provider.tsx`** _(47 linhas)_
Componente PROVIDER — 'fornece' dados/funcoes para todos os componentes filhos via Context API do React.

**`theme-toggle.tsx`** _(19 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`tiptap-editor.tsx`** _(542 linhas)_
Componente EDITOR — area de edicao de texto, codigo ou conteudo rico.

---

### 📁 `client/src/hooks/`
> Hooks React customizados — logica reutilizavel de estado e efeitos.

**`use-mobile.tsx`** _(20 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`use-toast.ts`** _(192 linhas)_
HOOK React personalizado para gerenciar estado/comportamento de '-toast'.

---

### 📁 `client/src/lib/`
> Funcoes auxiliares reutilizaveis em varios lugares do projeto.

**`queryClient.ts`** _(58 linhas)_
Arquivo de SERVICO/API — funcoes para comunicar com o servidor ou API externa.

**`utils.ts`** _(7 linhas)_
Funcoes UTILITARIAS — ferramentas reutilizaveis de uso geral no projeto.

---

### 📁 `client/src/pages/`
> Telas completas do app — cada arquivo aqui e uma pagina navegavel.

**`auditoria-financeira.tsx`** _(25 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`code-assistant.tsx`** _(1000 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`comparador-juridico.tsx`** _(25 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`comunicacoes-cnj.tsx`** _(403 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`configuracoes.tsx`** _(484 linhas)_
Componente de CONFIGURACOES — tela onde o usuario ajusta preferencias do app.

**`consulta-corporativo.tsx`** _(479 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`consulta-pdpj.tsx`** _(671 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`consulta-processual.tsx`** _(656 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`filtrador.tsx`** _(732 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`jurisprudencia.tsx`** _(3837 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`legal-assistant.tsx`** _(5410 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`legal-assistant.tsx.recovered`** _(3763 linhas)_
Arquivo RECOVERED — parte do projeto.

**`login.tsx`** _(119 linhas)_
Componente de LOGIN/AUTENTICACAO — tela de entrada com usuario e senha.

**`not-found.tsx`** _(33 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`painel-processos.tsx`** _(758 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`playground.tsx`** _(1473 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`previdenciario.tsx`** _(770 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`robo-djen.tsx`** _(1053 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`token-generator.tsx`** _(450 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`tramitacao.tsx`** _(828 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

---

### 📁 `server/replit_integrations/audio/`
> Pasta 'audio' — agrupamento de arquivos relacionados.

**`client.ts`** _(275 linhas)_
Arquivo de SERVICO/API — funcoes para comunicar com o servidor ou API externa.

**`index.ts`** _(15 linhas)_
Arquivo INDEX — ponto de entrada da pasta, exporta tudo que esta dentro.

**`routes.ts`** _(137 linhas)_
Arquivo de ROTAS — define as URLs/enderecos respondidos pelo servidor.

---

### 📁 `server/replit_integrations/batch/`
> Pasta 'batch' — agrupamento de arquivos relacionados.

**`index.ts`** _(8 linhas)_
Arquivo INDEX — ponto de entrada da pasta, exporta tudo que esta dentro.

**`utils.ts`** _(183 linhas)_
Funcoes UTILITARIAS — ferramentas reutilizaveis de uso geral no projeto.

---

### 📁 `server/replit_integrations/chat/`
> Pasta 'chat' — agrupamento de arquivos relacionados.

**`index.ts`** _(4 linhas)_
Arquivo INDEX — ponto de entrada da pasta, exporta tudo que esta dentro.

**`routes.ts`** _(204 linhas)_
Arquivo de ROTAS — define as URLs/enderecos respondidos pelo servidor.

**`storage.ts`** _(44 linhas)_
Arquivo TypeScript/JavaScript — logica, funcoes ou modulo do projeto.

---

### 📁 `server/replit_integrations/image/`
> Pasta 'image' — agrupamento de arquivos relacionados.

**`client.ts`** _(60 linhas)_
Arquivo de SERVICO/API — funcoes para comunicar com o servidor ou API externa.

**`index.ts`** _(4 linhas)_
Arquivo INDEX — ponto de entrada da pasta, exporta tudo que esta dentro.

**`routes.ts`** _(32 linhas)_
Arquivo de ROTAS — define as URLs/enderecos respondidos pelo servidor.

---

### 📁 `client/src/components/ui/`
> Componentes de UI (interface) basicos e genericos.

**`accordion.tsx`** _(57 linhas)_
Componente ACCORDION — secoes que abrem/fecham ao clicar, economizando espaco na tela.

**`alert-dialog.tsx`** _(140 linhas)_
Componente de NOTIFICACAO/ALERTA — mensagem temporaria que aparece na tela (ex: 'Salvo com sucesso!').

**`alert.tsx`** _(60 linhas)_
Componente de NOTIFICACAO/ALERTA — mensagem temporaria que aparece na tela (ex: 'Salvo com sucesso!').

**`aspect-ratio.tsx`** _(6 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`avatar.tsx`** _(52 linhas)_
Componente AVATAR — foto ou iniciais do usuario em formato circular.

**`badge.tsx`** _(39 linhas)_
Componente BADGE (etiqueta) — pequeno indicador com numero ou status (ex: '3 novas mensagens').

**`breadcrumb.tsx`** _(116 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`button.tsx`** _(63 linhas)_
Componente de BOTAO — elemento clicavel reutilizavel com estilo padrao do projeto.

**`calendar.tsx`** _(69 linhas)_
Componente CALENDARIO/AGENDA — visualizacao e selecao de datas e eventos.

**`card.tsx`** _(86 linhas)_
Componente CARD (cartao) — exibe uma informacao em um bloco visual com borda e sombra. Muito usado para listas de items.

**`carousel.tsx`** _(261 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`chart.tsx`** _(366 linhas)_
Componente de GRAFICO — visualizacao de dados em forma de grafico (barras, linhas, pizza...).

**`checkbox.tsx`** _(29 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`collapsible.tsx`** _(12 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`command.tsx`** _(152 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`context-menu.tsx`** _(199 linhas)_
CONTEXT do React — mecanismo para compartilhar dados entre componentes sem passar por props.

**`dialog.tsx`** _(123 linhas)_
Componente DIALOG — caixa de dialogo que exige resposta do usuario (confirmar, cancelar...).

**`drawer.tsx`** _(119 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`dropdown-menu.tsx`** _(199 linhas)_
Componente de MENU/DROPDOWN — lista de opcoes que aparece ao clicar em um botao.

**`form.tsx`** _(179 linhas)_
Componente de FORMULARIO — campos de entrada de dados (texto, selecao, etc.) com validacao.

**`hover-card.tsx`** _(30 linhas)_
Componente CARD (cartao) — exibe uma informacao em um bloco visual com borda e sombra. Muito usado para listas de items.

**`input-otp.tsx`** _(70 linhas)_
Componente de CAMPO DE ENTRADA — elemento de input com estilo personalizado.

**`input.tsx`** _(24 linhas)_
Componente de CAMPO DE ENTRADA — elemento de input com estilo personalizado.

**`label.tsx`** _(25 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`menubar.tsx`** _(257 linhas)_
Componente de MENU/DROPDOWN — lista de opcoes que aparece ao clicar em um botao.

**`navigation-menu.tsx`** _(129 linhas)_
Componente de NAVEGACAO/CABECALHO — barra superior com logo, menu e links de navegacao.

**`pagination.tsx`** _(118 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`popover.tsx`** _(30 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`progress.tsx`** _(29 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`radio-group.tsx`** _(43 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`resizable.tsx`** _(46 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`scroll-area.tsx`** _(47 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`select.tsx`** _(161 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`separator.tsx`** _(30 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`sheet.tsx`** _(141 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`sidebar.tsx`** _(728 linhas)_
Componente de BARRA LATERAL — menu ou painel que aparece na lateral da tela.

**`skeleton.tsx`** _(16 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`slider.tsx`** _(27 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`switch.tsx`** _(28 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`table.tsx`** _(118 linhas)_
Componente de TABELA — exibe dados em linhas e colunas.

**`tabs.tsx`** _(54 linhas)_
Componente de ABAS — permite alternar entre diferentes secoes de conteudo com clique.

**`textarea.tsx`** _(23 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`toast.tsx`** _(128 linhas)_
Componente de NOTIFICACAO/ALERTA — mensagem temporaria que aparece na tela (ex: 'Salvo com sucesso!').

**`toaster.tsx`** _(34 linhas)_
Componente de NOTIFICACAO/ALERTA — mensagem temporaria que aparece na tela (ex: 'Salvo com sucesso!').

**`toggle-group.tsx`** _(62 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`toggle.tsx`** _(44 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`tooltip.tsx`** _(31 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

---

## CONTEXTO PARA IA (copie e cole para continuar o projeto)

> Use este bloco para explicar o projeto para qualquer IA ou desenvolvedor:

```
Projeto: assistente-juridico-expo (2)
Tipo: Full-Stack (React + Express)
Stack: React + Vite, TypeScript, Tailwind CSS, Python, Node.js + Express, PostgreSQL, Drizzle ORM
Arquivos: 136 | Linhas: ~41.082
Rotas API: 131 endpoint(s) detectado(s)
Variaveis de ambiente necessarias: DATABASE_URL, SESSION_SECRET, PORT, APP_PASSWORD, AI_INTEGRATIONS_OPENAI_API_KEY, AI_INTEGRATIONS_OPENAI_BASE_URL, PUBLIC_API_KEY, AI_INTEGRATIONS_GEMINI_API_KEY, AI_INTEGRATIONS_GEMINI_BASE_URL, PDPJ_PEM_PRIVATE_KEY, PUBLIC_API_MODEL, PUBLIC_API_URL, DATAJUD_API_KEY, PERPLEXITY_API_KEY

Estrutura principal:
  .gitignore
  .sk/memoria.json
  App.tsx
  COMO_BUILDAR.md
  api/.ts
  app.json
  babel.config.js
  client/api.ts
  client/index.html
  client/index.ts
  client/public/auditoria.html
  client/public/codigo-formatacao.txt
  client/public/comparador.html
  client/public/manifest.json
  client/public/sw.js
  client/replit_integrations/audio/audio-playback-worklet.js
  client/replit_integrations/audio/audio-utils.ts
  client/replit_integrations/audio/index.ts
  client/replit_integrations/audio/useAudioPlayback.ts
  client/replit_integrations/audio/useVoiceRecorder.ts
  client/replit_integrations/audio/useVoiceStream.ts
  client/src/App.tsx
  client/src/components/pwa-install.tsx
  client/src/components/theme-provider.tsx
  client/src/components/theme-toggle.tsx
  client/src/components/tiptap-editor.tsx
  client/src/components/ui/accordion.tsx
  client/src/components/ui/alert-dialog.tsx
  client/src/components/ui/alert.tsx
  client/src/components/ui/aspect-ratio.tsx
  client/src/components/ui/avatar.tsx
  client/src/components/ui/badge.tsx
  client/src/components/ui/breadcrumb.tsx
  client/src/components/ui/button.tsx
  client/src/components/ui/calendar.tsx
  client/src/components/ui/card.tsx
  client/src/components/ui/carousel.tsx
  client/src/components/ui/chart.tsx
  client/src/components/ui/checkbox.tsx
  client/src/components/ui/collapsible.tsx
  client/src/components/ui/command.tsx
  client/src/components/ui/context-menu.tsx
  client/src/components/ui/dialog.tsx
  client/src/components/ui/drawer.tsx
  client/src/components/ui/dropdown-menu.tsx
  client/src/components/ui/form.tsx
  client/src/components/ui/hover-card.tsx
  client/src/components/ui/input-otp.tsx
  client/src/components/ui/input.tsx
  client/src/components/ui/label.tsx
  client/src/components/ui/menubar.tsx
  client/src/components/ui/navigation-menu.tsx
  client/src/components/ui/pagination.tsx
  client/src/components/ui/popover.tsx
  client/src/components/ui/progress.tsx
  client/src/components/ui/radio-group.tsx
  client/src/components/ui/resizable.tsx
  client/src/components/ui/scroll-area.tsx
  client/src/components/ui/select.tsx
  client/src/components/ui/separator.tsx
  client/src/components/ui/sheet.tsx
  client/src/components/ui/sidebar.tsx
  client/src/components/ui/skeleton.tsx
  client/src/components/ui/slider.tsx
  client/src/components/ui/switch.tsx
  client/src/components/ui/table.tsx
  client/src/components/ui/tabs.tsx
  client/src/components/ui/textarea.tsx
  client/src/components/ui/toast.tsx
  client/src/components/ui/toaster.tsx
  client/src/components/ui/toggle-group.tsx
  client/src/components/ui/toggle.tsx
  client/src/components/ui/tooltip.tsx
  client/src/hooks/use-mobile.tsx
  client/src/hooks/use-toast.ts
  client/src/index.css
  client/src/lib/queryClient.ts
  client/src/lib/utils.ts
  client/src/main.tsx
  client/src/pages/auditoria-financeira.tsx
  client/src/pages/code-assistant.tsx
  client/src/pages/comparador-juridico.tsx
  client/src/pages/comunicacoes-cnj.tsx
  client/src/pages/configuracoes.tsx
  client/src/pages/consulta-corporativo.tsx
  client/src/pages/consulta-pdpj.tsx
  client/src/pages/consulta-processual.tsx
  client/src/pages/filtrador.tsx
  client/src/pages/jurisprudencia.tsx
  client/src/pages/legal-assistant.tsx
  client/src/pages/legal-assistant.tsx.recovered
  client/src/pages/login.tsx
  client/src/pages/not-found.tsx
  client/src/pages/painel-processos.tsx
  client/src/pages/playground.tsx
  client/src/pages/previdenciario.tsx
  client/src/pages/robo-djen.tsx
  client/src/pages/token-generator.tsx
  client/src/pages/tramitacao.tsx
  components.json
  drizzle.config.ts
  eas.json
  fix_buttons.txt
  main.py
  migrations/0000_init.sql
  migrations/meta/0000_snapshot.json
  migrations/meta/_journal.json
  package.json
  postcss.config.js
  public/auditoria.html
  pyproject.toml
  script/build.ts
  server/db.ts
  server/djen.ts
  server/index.ts
  server/local-config.ts
  server/replit_integrations/audio/client.ts
  server/replit_integrations/audio/index.ts
  server/replit_integrations/audio/routes.ts
  server/replit_integrations/batch/index.ts
  server/replit_integrations/batch/utils.ts
  server/replit_integrations/chat/index.ts
  server/replit_integrations/chat/routes.ts
  server/replit_integrations/chat/storage.ts
  server/replit_integrations/image/client.ts
  server/replit_integrations/image/index.ts
  server/replit_integrations/image/routes.ts
  server/routes.ts
  server/static.ts
  server/storage.ts
  server/vite.ts
  shared/models/chat.ts
  shared/schema.ts
  tailwind.config.ts
  tsconfig.json
  vite.config.ts
```

---

*Plano gerado pelo SK Code Editor — 09/05/2026, 22:54:51*