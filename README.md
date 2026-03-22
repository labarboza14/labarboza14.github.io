# Site pessoal da Glória Barboza

Construído com Astro, hospedado no GitHub Pages, editável via Decap CMS.

## Como rodar localmente

```bash
npm install
npm run dev
```

O site abre em `http://localhost:4321`

## Estrutura de pastas

```
src/
  content/blog/     → posts do blog em Markdown
  pages/            → páginas do site (.astro)
  layouts/          → layout principal
  styles/           → CSS global
public/images/      → fotos e imagens
admin/              → painel do Decap CMS
```

## Adicionando um post novo

**Pelo CMS (recomendado):** acesse `/admin`, logue com GitHub e use a interface visual.

**Manualmente:** crie um arquivo `.md` em `src/content/blog/` com o frontmatter:

```markdown
---
title: "Título do post"
excerpt: "Resumo para a listagem."
date: "2026-04-01"
tag: "código"
readTime: "5 min de leitura"
---

Conteúdo do post aqui.
```

## Adicionando fotos

Coloque as imagens em `public/images/` com os nomes:

| Arquivo | Uso |
|---|---|
| `gloria-avatar.jpg` | Foto de perfil (hero e sobre) |
| `palco-python-floripa-2026.jpg` | Galeria |
| `palco-python-sul-2025.jpg` | Galeria |
| `palestrando.jpg` | Galeria |
| `sfd-porto-alegre.jpg` | Galeria |
| `ctrlz-2026.jpg` | Galeria |
| `work.jpg` | Galeria |

## Configurando o formulário de contato

1. Crie uma conta em [formspree.io](https://formspree.io)
2. Crie um novo formulário
3. Copie o ID gerado
4. Substitua `SEU_ID_FORMSPREE` em `src/pages/conversa.astro`

## Deploy

O deploy é automático via GitHub Actions a cada push na branch `main`.

Para configurar pela primeira vez:
1. Vá em Settings > Pages no repositório
2. Source: GitHub Actions
3. Faça um push qualquer — o deploy acontece automaticamente

## Configurando o Decap CMS

1. Ative o Netlify Identity no painel da Netlify (ou configure outro provider)
2. Ou use o modo `local_backend: true` para testar localmente
3. Acesse `/admin` e logue com sua conta GitHub
