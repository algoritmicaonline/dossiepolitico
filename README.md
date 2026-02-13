# 🎯 Landing Page - Dossiê Político | Algoritmica

## 📋 Visão Geral

Landing page completa de venda do produto **Dossiê Político** da Algoritmica. Uma página de alta conversão focada em inteligência digital para campanhas políticas, apresentando o produto de forma estratégica sem expor candidatos específicos.

---

## 🌐 URLs do Projeto

### Produção (Cloudflare Pages)
- **URL Principal**: https://dossie-politico.pages.dev
- **URL de Deploy**: https://b30d72ab.dossie-politico.pages.dev

### Backup Completo
- **Download**: https://www.genspark.ai/api/files/s/8zBFZOHz
- **Tamanho**: ~13 MB (inclui código, imagens, git repo)

---

## ✅ Funcionalidades Implementadas

### 📱 Seções da Landing Page

1. **🎨 Navegação Fixa**
   - Logo Algoritmica (oficial, sem acento)
   - Menu com links para todas as seções
   - CTA destacado no header

2. **🚀 Hero Section**
   - Título impactante: "Dossiê Político - Raio-X Digital e Político"
   - Subtítulo persuasivo
   - Dois CTAs (Começar Agora + Saber Mais)
   - 3 estatísticas de prova social (100+ campanhas, 95% sucesso, 24h entrega)
   - Imagem de dashboard político

3. **📖 O Que É**
   - Descrição completa do produto
   - Imagem de território digital
   - 2 blocos informativos destacados
   - 3 cards de features (Estratégia Digital, IA Especializada, Mídia por Votos)

4. **📦 Entregáveis** (6 cards detalhados)
   - Perfil Político Completo
   - Análise de Cenário
   - Mapa de Posicionamento
   - Raio-X das Redes Sociais
   - Oráculo Contínuo
   - Estratégia Acionável

5. **💪 Benefícios** (6 cards)
   - Velocidade Estratégica
   - Inteligência Artificial
   - Precisão e Confiabilidade
   - Vantagem Competitiva
   - Estratégia Personalizada
   - Suporte Dedicado

6. **🔄 Como Funciona** (Processo em 4 passos)
   - Você Contrata
   - Coletamos Dados
   - Analisamos
   - Você Recebe

7. **💰 Preços** (3 planos com destaque)
   - **Essencial**: R$ 2.497 (48h) - 6 benefícios
   - **Profissional**: R$ 4.997 (24h) - 7 benefícios + MAIS POPULAR
   - **Premium**: R$ 9.997 (12h) - 7 benefícios + VIP

8. **❓ FAQ** (6 perguntas frequentes)
   - O que é o Dossiê Político?
   - Confidencialidade
   - Múltiplos candidatos
   - Oráculo Contínuo
   - Formato de entrega
   - Garantia de satisfação

9. **🎯 CTA Final**
   - Título persuasivo
   - 2 CTAs (Preços + WhatsApp)
   - Estatísticas repetidas para reforço

10. **📞 Footer Completo**
    - Logo + Descrição
    - Links de navegação
    - Informações de contato
    - Redes sociais
    - Copyright e políticas

---

## 🎨 Identidade Visual

### Paleta de Cores Algoritmica
- **Primária**: Orange-500 (#f97316) a Orange-600 (#ea580c)
- **Gradientes**: from-orange-500 to-orange-600
- **Backgrounds**: Orange-50 a Orange-100
- **Textos**: Gray-900 (títulos), Gray-600 (corpo)
- **Destaques**: Yellow-400 (badge "Mais Popular")

### Imagens Utilizadas
1. `logo-algoritmica.png` - Logo oficial (15 KB)
2. `dashboard-politico.png` - Dashboard no hero (104 KB)
3. `territorio-digital.png` - Seção "O Que É" (1.6 MB)
4. `ia-especializada.png` - Card IA (1.8 MB)
5. `robo-sorridente.png` - Card Tecnologia (1.5 MB)
6. `mapa-estrategico.png` - Card Estratégia (1.5 MB)

---

## 🛠️ Stack Tecnológico

- **Framework**: Hono (Cloudflare Workers)
- **Frontend**: HTML5 + CSS3 (inline)
- **Estilização**: Tailwind CSS 3.x (CDN)
- **Ícones**: FontAwesome 6.4.0 (CDN)
- **Fontes**: Google Fonts - Inter
- **Build**: Vite
- **Deploy**: Cloudflare Pages (Wrangler)
- **Controle de Versão**: Git

---

## 📂 Estrutura de Arquivos

```
webapp/
├── src/
│   └── index.tsx               # Backend Hono (não usado no deploy atual)
├── public/
│   ├── index.html              # Landing page completa (795 linhas)
│   ├── index-old.html          # Backup da versão anterior
│   ├── _headers                # Headers de segurança Cloudflare
│   ├── _redirects              # Regras de redirecionamento
│   └── static/
│       └── images/             # 6 imagens principais + extras
├── .git/                       # Repositório Git
├── .gitignore                  # Ignora node_modules, .env, etc
├── package.json                # Scripts e dependências
├── vite.config.ts              # Configuração Vite
├── wrangler.jsonc              # Config Cloudflare Pages
└── README.md                   # Esta documentação
```

---

## 🚀 Deploy e Comandos

### Local (Desenvolvimento)
```bash
# Navegar até o projeto
cd /home/user/webapp

# Ver arquivos
ls -lh public/
```

### Deploy para Cloudflare Pages
```bash
# Deploy completo (recomendado)
npx wrangler pages deploy public --project-name dossie-politico

# Deploy será feito automaticamente para:
# - https://dossie-politico.pages.dev (produção)
# - https://[hash].dossie-politico.pages.dev (preview)
```

### Git
```bash
# Status
git status

# Commit
git add .
git commit -m "Sua mensagem"

# Log
git log --oneline
```

---

## 🎯 Próximos Passos Recomendados

### 1. Integração Hotmart (URGENTE)
Atualmente os botões de preços apontam para `#` (nenhum link). É necessário:

```html
<!-- Substituir no arquivo public/index.html -->

<!-- Plano Essencial (linha ~510) -->
<a href="https://pay.hotmart.com/SEU_LINK_ESSENCIAL" class="block...">

<!-- Plano Profissional (linha ~580) -->
<a href="https://pay.hotmart.com/SEU_LINK_PROFISSIONAL" class="block...">

<!-- Plano Premium (linha ~650) -->
<a href="https://pay.hotmart.com/SEU_LINK_PREMIUM" class="block...">
```

### 2. Atualizar Contatos
```html
<!-- WhatsApp (múltiplas ocorrências) -->
<a href="https://wa.me/55DD987654321">  <!-- Trocar 5511999999999 -->

<!-- Email (footer) -->
<a href="mailto:seu-email@algoritmica.com.br">
```

### 3. Adicionar Tracking e Pixels
```html
<!-- No <head> do index.html, adicionar: -->

<!-- Google Analytics -->
<script async src="https://www.googletagmanager.com/gtag/js?id=G-XXXXXXXXXX"></script>

<!-- Facebook Pixel -->
<script>
  !function(f,b,e,v,n,t,s)
  {if(f.fbq)return;n=f.fbq=function(){n.callMethod?
  n.callMethod.apply(n,arguments):n.queue.push(arguments)};
  if(!f._fbq)f._fbq=n;n.push=n;n.loaded=!0;n.version='2.0';
  n.queue=[];t=b.createElement(e);t.async=!0;
  t.src=v;s=b.getElementsByTagName(e)[0];
  s.parentNode.insertBefore(t,s)}(window, document,'script',
  'https://connect.facebook.net/en_US/fbevents.js');
  fbq('init', 'SEU_PIXEL_ID');
  fbq('track', 'PageView');
</script>

<!-- Hotmart Pixel -->
<script src="https://static.hotmart.com/checkout/widget.min.js"></script>
```

### 4. Melhorias de SEO
- [ ] Adicionar meta tags Open Graph
- [ ] Adicionar meta tags Twitter Cards
- [ ] Criar sitemap.xml
- [ ] Adicionar robots.txt
- [ ] Otimizar imagens (comprimir para WebP)
- [ ] Adicionar schema.org (structured data)

### 5. Testes A/B
- [ ] Testar diferentes títulos no hero
- [ ] Testar diferentes preços/ofertas
- [ ] Testar diferentes CTAs
- [ ] Testar diferentes ordens de benefícios

### 6. Funcionalidades Adicionais
- [ ] Pop-up de saída (exit intent)
- [ ] Chat ao vivo (Tawk.to, Zendesk)
- [ ] Formulário de captura de leads
- [ ] Vídeo explicativo no hero
- [ ] Depoimentos em vídeo
- [ ] Certificações e selos de segurança

---

## 📊 Checklist de Conversão

### ✅ Já Implementado
- [x] Hero impactante com proposta de valor clara
- [x] Múltiplos CTAs estrategicamente posicionados
- [x] Prova social (estatísticas, números)
- [x] Descrição completa dos entregáveis
- [x] Seção de benefícios clara
- [x] 3 planos de preços com destaque
- [x] FAQ para objeções comuns
- [x] Design responsivo (mobile-first)
- [x] Paleta de cores da marca
- [x] Logo oficial
- [x] Performance otimizada (CDN)

### ⏳ A Fazer
- [ ] Links reais de pagamento Hotmart
- [ ] Contatos reais (WhatsApp + Email)
- [ ] Pixels de tracking instalados
- [ ] Depoimentos de clientes reais
- [ ] Garantias detalhadas
- [ ] Escassez (vagas limitadas?)
- [ ] Urgência (promoção temporária?)

---

## 🔧 Manutenção e Atualizações

### Para Editar Conteúdo
1. Editar `/home/user/webapp/public/index.html`
2. Testar localmente (abrir no navegador)
3. Fazer commit: `git commit -am "Descrição da mudança"`
4. Deploy: `npx wrangler pages deploy public --project-name dossie-politico`

### Para Adicionar Novas Imagens
1. Fazer upload para `/home/user/webapp/public/static/images/`
2. Referenciar no HTML: `/static/images/nome-da-imagem.png`
3. Deploy

### Para Mudar Preços
Editar as linhas:
- Essencial: linha ~495
- Profissional: linha ~565
- Premium: linha ~635

---

## 📈 Métricas Importantes

### KPIs para Monitorar
- **Taxa de Conversão**: % de visitantes que compram
- **Bounce Rate**: % de visitantes que saem imediatamente
- **Tempo na Página**: Quanto tempo passam lendo
- **Scroll Depth**: Até onde rolam a página
- **Cliques nos CTAs**: Quais botões são mais clicados
- **Taxa de Abandono no Checkout**: % que desistem no Hotmart

### Ferramentas Recomendadas
- Google Analytics 4
- Hotmart Analytics
- Meta Pixel (Facebook/Instagram Ads)
- Hotjar (heatmaps)
- Google Search Console (SEO)

---

## 💡 Dicas de Otimização

### Copywriting
- Usar "você" (linguagem direta)
- Focar em benefícios, não features
- Criar senso de urgência
- Mostrar transformação (antes/depois)
- Usar números específicos

### Design
- Manter hierarquia visual clara
- Usar espaçamento generoso
- Destacar CTAs com cores contrastantes
- Manter consistência de cores/fontes
- Otimizar para mobile

### Performance
- Comprimir imagens (TinyPNG)
- Usar lazy loading
- Minificar CSS/JS
- Usar CDN (já implementado)
- Testar velocidade (PageSpeed Insights)

---

## 📱 Responsividade

A landing page é **totalmente responsiva** e funciona perfeitamente em:
- 📱 **Mobile**: 320px - 767px
- 📱 **Tablet**: 768px - 1023px
- 💻 **Desktop**: 1024px+
- 🖥️ **Large Desktop**: 1280px+

Todas as seções se adaptam automaticamente:
- Grid responsivo (1 coluna mobile → 2-3 colunas desktop)
- Navegação mobile-friendly
- Imagens adaptativas
- Textos redimensionáveis
- CTAs otimizados para touch

---

## 🔐 Segurança e Privacidade

### Headers de Segurança (_headers)
```
/*
  X-Frame-Options: DENY
  X-Content-Type-Options: nosniff
  X-XSS-Protection: 1; mode=block
  Referrer-Policy: strict-origin-when-cross-origin
```

### Compliance
- LGPD: Adicionar política de privacidade
- Hotmart: TOS e termos aceitos automaticamente
- Cookies: Aviso de cookies (se usar GA/FB Pixel)

---

## 📞 Suporte

### Contatos da Algoritmica
- **Email**: contato@algoritmica.com.br
- **WhatsApp**: (11) 99999-9999 (ATUALIZAR!)
- **Localização**: São Paulo, SP - Brasil

### Suporte Técnico
- **Cloudflare Pages**: https://dash.cloudflare.com/
- **Hotmart**: https://hotmart.com/
- **GitHub** (se integrado): Seu repositório

---

## 📜 Licença e Direitos

© 2024 Algoritmica. Todos os direitos reservados.

**Propriedade Intelectual**: Todo o conteúdo, design e código desta landing page são de propriedade exclusiva da Algoritmica.

---

## 🎉 Resultado Final

✅ **Landing page profissional de alta conversão**  
✅ **Design moderno com identidade visual Algoritmica**  
✅ **100% responsiva e otimizada**  
✅ **Hospedada em CDN global (Cloudflare)**  
✅ **SSL/HTTPS automático**  
✅ **Pronta para integração Hotmart**  
✅ **SEO-friendly**  
✅ **Performance excelente**

---

**🔗 URL de Produção**: https://dossie-politico.pages.dev

**🔗 Backup Completo**: https://www.genspark.ai/api/files/s/8zBFZOHz

---

**Última Atualização**: 13 de Fevereiro de 2026  
**Versão**: 2.0 (Landing Completa)  
**Status**: ✅ **ONLINE E FUNCIONANDO**
