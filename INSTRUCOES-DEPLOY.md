# 🚀 Instruções de Deploy - Dossiê Político Algoritmica

## 📦 Conteúdo do Backup

Este arquivo contém a landing page completa do **Dossiê Político da Algoritmica**:

- ✅ Código fonte Hono/TypeScript
- ✅ HTML standalone (`public/index.html`)
- ✅ 6 imagens principais (7MB total)
- ✅ Configurações Cloudflare Pages
- ✅ Git repository completo
- ✅ Paleta de cores laranja/vermelho
- ✅ Logo oficial Algoritmica

---

## 🎯 Opções de Deploy

### **Opção 1: Cloudflare Pages (Recomendado)**

#### Pré-requisitos
- Conta no Cloudflare (gratuita)
- Wrangler CLI instalado

#### Passos

1. **Extrair o backup:**
```bash
tar -xzf dossie-politico-algoritmica-completo.tar.gz
cd home/user/webapp
```

2. **Instalar dependências:**
```bash
npm install
```

3. **Build do projeto:**
```bash
npm run build
```

4. **Login no Cloudflare:**
```bash
npx wrangler login
```

5. **Criar projeto no Cloudflare Pages:**
```bash
npx wrangler pages project create dossie-politico --production-branch main
```

6. **Deploy:**
```bash
npx wrangler pages deploy public --project-name dossie-politico
```

7. **Pronto!** Sua URL será algo como:
```
https://dossie-politico.pages.dev
```

---

### **Opção 2: Deploy HTML Estático (Mais Simples)**

Se preferir usar apenas o HTML sem o backend Hono:

1. **Extrair apenas a pasta `public/`:**
```bash
tar -xzf dossie-politico-algoritmica-completo.tar.gz home/user/webapp/public/
```

2. **Fazer upload em qualquer host estático:**
   - Netlify (arrastar pasta `public/`)
   - Vercel (arrastar pasta `public/`)
   - GitHub Pages
   - Qualquer servidor web

3. **Ou usar Cloudflare Pages diretamente:**
```bash
cd home/user/webapp/public
npx wrangler pages deploy . --project-name dossie-politico
```

---

### **Opção 3: Servidor Local para Teste**

```bash
# Extrair
tar -xzf dossie-politico-algoritmica-completo.tar.gz
cd home/user/webapp

# Instalar
npm install

# Build
npm run build

# Testar localmente
npx wrangler pages dev public
```

Acesse: `http://localhost:8788`

---

## 📁 Estrutura do Projeto

```
webapp/
├── public/
│   ├── index.html              # Landing page HTML
│   └── static/
│       ├── images/              # 6 imagens principais
│       │   ├── logo-algoritmica.png
│       │   ├── dashboard-politico.png
│       │   ├── territorio-digital.png
│       │   ├── ia-especializada.png
│       │   ├── robo-sorridente.png
│       │   └── mapa-estrategico.png
│       └── style.css
├── src/
│   ├── index.tsx               # Backend Hono (opcional)
│   └── renderer.tsx
├── package.json
├── wrangler.jsonc             # Config Cloudflare
├── vite.config.ts
└── .git/                       # Histórico Git
```

---

## 🎨 Personalização

### Cores da Marca
No arquivo `public/index.html`, procure por:
- `#ff6b35` - Laranja principal
- `#f7931e` - Laranja dourado
- `#f44336` - Vermelho complementar

### Logo
Substitua `/static/images/logo-algoritmica.png` por sua versão

### Textos
Edite diretamente em `public/index.html`

### Integração Hotmart
No arquivo HTML, procure pela função `comprarPlano()` e adicione seus links:

```javascript
const links = {
    'essencial': 'https://pay.hotmart.com/SEU_LINK_ESSENCIAL',
    'profissional': 'https://pay.hotmart.com/SEU_LINK_PROFISSIONAL',
    'premium': 'https://pay.hotmart.com/SEU_LINK_PREMIUM'
};
```

---

## 🔧 Comandos Úteis

```bash
# Desenvolvimento local
npm run dev                    # Vite dev server
npm run build                  # Build para produção
npm run preview               # Preview do build

# Wrangler (Cloudflare)
npx wrangler pages dev public  # Dev local com Wrangler
npx wrangler pages deploy      # Deploy para produção
npx wrangler pages list        # Listar projetos
```

---

## ✅ Checklist Pré-Deploy

- [ ] Testar localmente
- [ ] Verificar todas as imagens carregam
- [ ] Testar responsividade (mobile/tablet/desktop)
- [ ] Adicionar links Hotmart reais
- [ ] Configurar domínio customizado (opcional)
- [ ] Adicionar Google Analytics (opcional)
- [ ] Testar todos os links e botões

---

## 🆘 Problemas Comuns

### Imagens não aparecem
- Verifique se a pasta `public/static/images/` existe
- Confirme que os paths são `/static/images/nome.png`

### Build falha
```bash
rm -rf node_modules package-lock.json
npm install
npm run build
```

### Erro no Wrangler
```bash
npx wrangler logout
npx wrangler login
```

---

## 📞 Suporte

Para dúvidas sobre o projeto:
- Revisar este documento
- Verificar logs: `npm run build` ou `npx wrangler pages deploy`
- Documentação Cloudflare: https://developers.cloudflare.com/pages

---

## 🎯 Próximos Passos Recomendados

1. ✅ Deploy para produção
2. ✅ Configurar domínio customizado
3. ✅ Adicionar Google Analytics
4. ✅ Integrar Hotmart
5. ✅ Adicionar pixel Facebook/Meta
6. ✅ Configurar e-mail marketing
7. ✅ Testar conversão

---

**🎉 Boa sorte com suas campanhas políticas!**

*Landing page desenvolvida com Hono + Cloudflare Pages + TailwindCSS*
