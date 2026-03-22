# Como configurar a senha do painel admin

O painel em `/admin` tem uma tela de login protegida por senha com hash SHA-256.
A senha nunca fica exposta no código — só o hash.

## Passo a passo

### 1. Gere o hash da sua senha

Abra o navegador, pressione F12 para abrir o console e cole este código:

```javascript
const senha = 'coloque_sua_senha_aqui';
const hash = await crypto.subtle.digest('SHA-256', new TextEncoder().encode(senha))
  .then(b => Array.from(new Uint8Array(b)).map(x => x.toString(16).padStart(2,'0')).join(''));
console.log('Seu hash:', hash);
```

Copie o hash gerado (uma string longa de letras e números).

### 2. Cole o hash no arquivo admin/index.html

Abra `admin/index.html` e encontre a linha:

```javascript
const PASS_HASH = 'COLE_O_HASH_SHA256_AQUI';
```

Substitua `COLE_O_HASH_SHA256_AQUI` pelo hash que você gerou.

### 3. Exemplo

Se sua senha for `floripa2026`, o hash gerado será algo como:
`a3f1b2c4...` (64 caracteres hexadecimais)

Nunca compartilhe a senha. O hash no código é seguro — não dá para reverter o hash para descobrir a senha original.

## Observação

Esta proteção é uma camada extra de segurança visual. Para proteção completa, configure também o Netlify Identity ou outro provider de autenticação no Decap CMS.
