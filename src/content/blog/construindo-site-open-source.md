---
title: "Como construí este site com ferramentas open source (e o que aprendi no processo)"
excerpt: "Não comprei template, não assinei plataforma. Usei ferramentas gratuitas, de código aberto, e fui aprendendo enquanto construía. Astro, GitHub Pages, Decap CMS e a conexão com a Cumbuca Dev."
date: "2026-03-22"
tag: "open source"
readTime: "8 min de leitura"
---

Você está lendo este texto num site que eu construí do zero.

Não comprei um template. Não assinei uma plataforma. Não pedi para ninguém fazer por mim. Usei ferramentas gratuitas, de código aberto, e fui aprendendo enquanto construía.

Esse processo virou projeto. O projeto virou aprendizado. E o aprendizado virou este artigo.

Se você está começando na programação ou pensando em ter um espaço seu na internet, fica até o final. Vou contar exatamente o que usei, por que escolhi cada ferramenta e o que cada escolha me ensinou. Sem jargão desnecessário, sem README, mas com honestidade técnica.

---

## Por que ter um site pessoal em 2026

Antes de falar de ferramenta, preciso falar de motivação.

Eu trabalho com tecnologia, organizo comunidade, já palestrei em eventos regionais e nacionais. Mas por muito tempo minha presença digital era fragmentada. LinkedIn aqui, GitHub ali, Instagram da Python Floripa em outro lugar. Quem quisesse me conhecer profissionalmente precisava montar um quebra-cabeça.

Um site pessoal resolve isso. É o lugar onde você controla a narrativa. Onde a trajetória não-linear vira uma história com começo, meio e propósito. Onde o projeto que você fez às 23h para resolver um problema do time aparece com o contexto que merece.

E tem outra coisa: construir o próprio site é um projeto técnico real. Com decisões reais, trade-offs reais, e aprendizado que nenhum tutorial de "olá, mundo" entrega.

---

## A stack: o que é cada peça e por que escolhi

### Astro, o gerador de páginas

O [Astro](https://astro.build) é o framework que gera as páginas do site. Ele pega seus arquivos de conteúdo e transforma em HTML estático que qualquer navegador entende.

Por que Astro e não WordPress, Wix ou outro? Porque eu queria entender o que estava fazendo. Wix é ótimo para quem quer um site rápido sem programar. Eu queria programar. E o Astro foi projetado para sites de conteúdo, é open source e tem uma comunidade ativa.

A grande vantagem de gerar HTML estático é que não precisa de servidor rodando constantemente. O site é um conjunto de arquivos. Isso significa hospedagem gratuita, velocidade e muito menos coisa para dar errado.

### Markdown, a linguagem dos posts

Cada post deste blog, incluindo este que você está lendo agora, é um arquivo `.md`. Markdown é uma linguagem de marcação simples, criada para que humanos escrevam texto formatado sem precisar de tags HTML.

Este trecho em Markdown:

```
**negrito**, *itálico*, [link](https://url.com)
```

Vira HTML automaticamente. É o formato que a Cumbuca Dev usa no blog deles, que o GitHub usa para READMEs, que boa parte da documentação técnica do mundo usa. Aprender Markdown é aprender a língua franca da escrita técnica.

### Decap CMS, editar sem tocar em código

Aqui está o ponto que mais me importava: quero escrever meus posts sem abrir o terminal.

O [Decap CMS](https://decapcms.org) resolve isso. É um painel de administração que vive dentro do próprio site, em `seusite.com/admin`. Você faz login com sua conta do GitHub, e aparece uma interface de edição visual. Escreve, salva, publica. O CMS faz o commit no repositório automaticamente.

É open source, gratuito e não depende de nenhuma empresa por trás para continuar funcionando. Isso importa. Ferramentas proprietárias encerram, mudam de política, cobram. Código aberto é de quem usa.

### GitHub Pages, hospedagem gratuita

O [GitHub](https://github.com) é onde o código fica guardado. O GitHub Pages é um serviço que pega esse código e publica como site automaticamente, também de graça.

O endereço padrão fica `labarboza14.github.io`. Domínio próprio pode vir depois, quando fizer sentido.

Todo o fluxo funciona assim: escrevo um post no Decap CMS, ele faz um commit no repositório do GitHub, o GitHub Pages detecta a mudança e publica o site atualizado. Automático. Sem eu precisar fazer nada além de escrever.

---

## A conexão com a Cumbuca Dev

Não dá para falar de open source e não falar da [Cumbuca Dev](https://cumbuca.dev).

A Cumbuca é uma organização que promove diversidade em tecnologia por meio da educação e do código aberto. Uma das coisas que mais admiro no que elas fazem é exatamente isso: o open source aparece não como curiosidade técnica, mas como vivência real. Contribuir para um projeto aberto é a forma mais honesta de aprender a trabalhar em equipe no desenvolvimento de software, porque você lida com revisão de código, convenções de projeto, comunicação assíncrona e a humildade de ter o seu trabalho avaliado por outra pessoa.

Projetos como o **GitCaos**, que existe para que iniciantes pratiquem Git sem medo de estragar algo de verdade, ou o **brutils-python**, que foi o primeiro laboratório colaborativo da comunidade, mostram que open source é uma forma de aprender fazendo, com segurança e com gente ao lado.

Este site segue esse mesmo espírito. O código está público no meu GitHub. Qualquer pessoa pode ver como foi construído, adaptar para o próprio uso, apontar melhorias. Não é um produto fechado. É um processo aberto.

---

## O que aprendi construindo

### Decisões técnicas são decisões humanas

Cada ferramenta que escolhi tem uma razão que vai além da técnica. Escolhi Astro porque queria aprender. Escolhi Decap CMS porque quero escrever com frequência sem atrito. Escolhi GitHub Pages porque não quero depender de cartão de crédito para manter um site no ar.

Essas são escolhas de valor, não de performance. E isso é algo que a gente raramente discute quando fala de tecnologia.

### Documentar o processo é parte do processo

Enquanto construía o site, fui anotando as decisões. Por que escolhi essa cor e não outra. Por que o formulário de contato usa Formspree em vez de um backend próprio. Por que os posts ficam em Markdown e não num banco de dados.

Essas anotações viraram este artigo. E este artigo vai ficar no site. E o site é o projeto. Tudo conectado.

### Open source não é só código

A Cumbuca Dev tem uma forma de ver o open source que eu uso muito: é conexão, prática e vivência concreta na tecnologia. Construir este site com ferramentas abertas foi exatamente isso. Consultei documentação escrita por voluntários, resolvi problemas em fóruns onde outra pessoa já tinha passado pela mesma dificuldade, e agora estou compartilhando o resultado para que alguém possa usar como referência.

O ciclo fecha quando você também compartilha.

---

## Quanto custa tudo isso

Zero reais por mês.

Astro é gratuito. GitHub é gratuito. GitHub Pages é gratuito. Decap CMS é gratuito. Formspree tem plano gratuito suficiente para começar.

O único custo possível é um domínio próprio, em torno de R$ 60 por ano, e isso é opcional. O site funciona perfeitamente sem ele.

---

## Por onde começar se você quiser fazer o mesmo

**1. Crie uma conta no GitHub** se ainda não tiver. É onde tudo vai ficar guardado.

**2. Instale o Node.js** no seu computador. O Astro precisa dele para funcionar.

**3. Crie um projeto Astro** com o comando `npm create astro@latest` no terminal. O assistente vai te guiar.

**4. Suba o código para o GitHub** e ative o GitHub Pages nas configurações do repositório.

**5. Configure o Decap CMS** seguindo a documentação oficial.

Cada passo desses merece um post próprio. E eu pretendo escrever sobre cada um.

---

## Um convite

Se você está aprendendo programação e quer ter experiência real com fluxo de desenvolvimento, contribuição em projetos abertos e trabalho colaborativo, a Cumbuca Dev é um lugar para olhar. Têm projetos em andamento, documentação em português e uma cultura de acolhimento genuíno para quem está chegando.

E se você já tem um site ou está construindo um, me conta. Quero ver o que as pessoas estão fazendo. É exatamente esse tipo de troca que torna a comunidade de tecnologia um lugar melhor do que seria se cada um ficasse no seu canto.

Bora construir coisas juntos. 🌸
