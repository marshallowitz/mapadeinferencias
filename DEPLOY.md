# Como publicar o site

## Estrutura de arquivos

```
/
├── index.html        ← landing page (página inicial)
├── calculadora.html  ← engine de inferência
├── docs.html         ← documentação de referência
└── DEPLOY.md         ← este arquivo
```

## Opção 1 — Netlify (recomendado, grátis, 2 minutos)

1. Acesse https://netlify.com e crie uma conta gratuita
2. No dashboard, clique em **"Add new site" → "Deploy manually"**
3. **Arraste a pasta inteira** (com os 3 arquivos HTML) para a área de upload
4. Pronto — o Netlify gera uma URL como `https://nome-aleatorio.netlify.app`

### Para usar domínio próprio no Netlify:
1. No painel do site, vá em **Domain management → Add custom domain**
2. Aponte o DNS do seu domínio para o Netlify (eles mostram os valores exatos)
3. HTTPS é ativado automaticamente

---

## Opção 2 — GitHub Pages (grátis, requer conta GitHub)

1. Crie um repositório público no GitHub (ex: `inference-engine`)
2. Faça upload dos 3 arquivos HTML
3. Vá em **Settings → Pages → Source: Deploy from branch → main / root**
4. URL fica: `https://seu-usuario.github.io/inference-engine/`

---

## Opção 3 — Vercel (grátis, similar ao Netlify)

1. Acesse https://vercel.com
2. **"Add New → Project → Browse" → selecione a pasta**
3. Clique em **Deploy** — pronto

---

## Atualizando o site depois

Para qualquer das opções acima, basta repetir o upload com os arquivos modificados.
No Netlify: **Deploys → Drag & drop** uma nova versão da pasta.

---

## SEO básico (opcional)

Para melhorar indexação nos buscadores, adicione no `<head>` de cada página:

```html
<meta property="og:title" content="Engine de Inferência Estatística">
<meta property="og:description" content="Inferências com base científica real — cobertura ponderada pelos pesos da literatura original.">
<meta property="og:type" content="website">
<link rel="canonical" href="https://SEU-DOMINIO.com/">
```

---

Gerado em julho de 2025.
