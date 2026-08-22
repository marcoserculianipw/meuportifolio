# Portfólio — Marcos Vinicius (versão simples)

Versão **sem Node, sem npm, sem terminal**. Só 3 arquivos: `index.html`,
`style.css` e `script.js`. Todas as imagens (sua foto e os prints dos
projetos) estão **embutidas diretamente dentro do `script.js`** — não existe
mais pasta de imagens. Isso significa que, não importa como você abra ou mova
esses 3 arquivos, as fotos sempre vão aparecer.

## Como ver o site

Dê **dois cliques no `index.html`**. Abre no navegador, sem instalar nada.

> Importante: se você baixou um `.zip`, **extraia ele primeiro** (botão
> direito → "Extrair Tudo...") antes de abrir o `index.html`. Abrir o arquivo
> de dentro do zip sem extrair pode causar problemas.

## O que tem de novo

- **Clique em qualquer projeto** para abrir uma janela com mais fotos e a
  descrição completa (problema, solução, tecnologias e seu papel).
- **Sua foto aparece logo na primeira seção** (Hero), não só lá embaixo.
- Por enquanto só os projetos **FNCASH** e **Viagens** estão no site — dá pra
  adicionar mais depois (veja como, abaixo).

## O que falta preencher

Abra o `script.js` em qualquer editor de texto (Bloco de Notas serve) e vá
até o topo do arquivo, na parte depois do bloco gigante de imagens em
base64 — procure por `SOCIAL_LINKS` e `PROJECTS`:

```js
const SOCIAL_LINKS = {
  github: '',   // ex: 'https://github.com/seu-usuario'
  linkedin: '', // ex: 'https://linkedin.com/in/seu-usuario'
  email: '',    // ex: 'seuemail@gmail.com'
};
```

E dentro de cada projeto em `PROJECTS`, procure pelos campos marcados com
`[ADICIONAR ...]` — é onde falta você preencher (por exemplo, seu papel em
cada projeto).

## Como adicionar um novo projeto no futuro

1. Adicione as fotos do novo projeto em algum site de imagem base64 (ex:
   [base64-image.de](https://www.base64-image.de/)) ou me peça para gerar.
2. Copie um dos blocos `{ ... }` dentro do array `PROJECTS` no `script.js`.
3. Cole logo abaixo, ajuste `id`, `name`, `description`, `problem`,
   `solution`, `role`, `stack` e as chaves de `gallery`/`cover` para apontar
   para as novas imagens dentro do objeto `IMAGES`.

## Como publicar no GitHub Pages

1. Crie uma conta no [github.com](https://github.com) se ainda não tiver.
2. Crie um repositório novo (botão verde **New**).
3. Na página do repositório, **Add file → Upload files**.
4. Arraste os 3 arquivos (`index.html`, `style.css`, `script.js`) e clique em
   **Commit changes**.
5. Vá em **Settings → Pages**.
6. Em **Source**, escolha **Deploy from a branch**, branch `main`, pasta
   `/root`, e **Save**.
7. Em 1-2 minutos, o site estará em:
   `https://SEU-USUARIO.github.io/NOME-DO-REPOSITORIO/`

Sem terminal, sem instalação — tudo pelo navegador.
