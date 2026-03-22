Perfeito — mantive o que você já fez (que está bom) e só adicionei **camadas estratégicas de contexto, clareza e posicionamento**, sem deixar longo.

Aqui vai a versão **pronta pra colar** 👇

---

````md
# Site pessoal da Glória Barboza

Este é meu site pessoal, criado para reunir minha trajetória, conteúdos e participação em comunidades de tecnologia.

O projeto foi pensado para ser simples de manter, com foco em autonomia na publicação e organização clara da informação.

Construído com Astro, hospedado no GitHub Pages e editável via Decap CMS.

---

## Como rodar localmente

```bash
npm install
npm run dev
````

O site abre em `http://localhost:4321`

---

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

---

## Adicionando um post novo

**Pelo CMS (recomendado):**
Acesse `/admin`, faça login com GitHub e use a interface visual.

**Manualmente:**
Crie um arquivo `.md` em `src/content/blog/` com o frontmatter:

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

---

## Adicionando fotos

Coloque as imagens em `public/images/`.

| Arquivo                         | Uso                           |
| ------------------------------- | ----------------------------- |
| `gloria-avatar.jpg`             | Foto de perfil (hero e sobre) |
| `palco-python-floripa-2026.jpg` | Galeria                       |
| `palco-python-sul-2025.jpg`     | Galeria                       |
| `palestrando.jpg`               | Galeria                       |
| `sfd-porto-alegre.jpg`          | Galeria                       |
| `ctrlz-2026.jpg`                | Galeria                       |
| `work.jpg`                      | Galeria                       |

---

## Configurando o formulário de contato

1. Crie uma conta em [https://formspree.io](https://formspree.io)
2. Crie um novo formulário
3. Copie o ID gerado
4. Substitua `SEU_ID_FORMSPREE` em `src/pages/conversa.astro`

---

## Deploy

O deploy é automático via GitHub Actions a cada push na branch `main`.

Para configurar pela primeira vez:

1. Vá em Settings > Pages no repositório
2. Source: GitHub Actions
3. Faça um push — o deploy acontece automaticamente

---

## Configurando o Decap CMS

1. Ative o Netlify Identity (ou outro provider)
2. Ou use `local_backend: true` para testes locais
3. Acesse `/admin` e faça login com GitHub

---

## Aprendizados

Este projeto envolveu:

* Estruturação de um site com Astro
* Organização de conteúdo em Markdown
* Integração com CMS (Decap)
* Deploy automático com GitHub Actions
* Uso de serviços externos como Formspree

Além da parte técnica, reforça a construção de um fluxo simples, sustentável e autônomo de publicação.

---

## Objetivo

Mais do que um site pessoal, este projeto funciona como um espaço de organização, expressão e evolução contínua na tecnologia.

```
<!-- trigger deploy -->
---

