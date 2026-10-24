# GOA Tecnologia — Landing Page

Projeto React 18 + Vite, responsivo, com identidade visual azul e branca e logo oficial fornecida.

## Publicar na Vercel usando GitHub (recomendado)

1. Extraia o ZIP. A pasta `goa-landing` contém `package.json`, `index.html`, `src/` e `public/`.
2. No GitHub, crie um repositório privado ou público, por exemplo `goa-site`.
3. No repositório, use **Add file > Upload files** e envie **o conteúdo da pasta `goa-landing`**, não o ZIP e não uma pasta adicional. O arquivo `package.json` precisa ficar na raiz do repositório.
4. Acesse https://vercel.com/new, conecte o GitHub e importe o repositório.
5. Em **Configure Project**: Framework Preset `Vite`; Root Directory `./`; Build Command `npm run build`; Output Directory `dist`. Normalmente a Vercel detecta tudo automaticamente.
6. Clique **Deploy**. Após o build, acesse a URL terminada em `.vercel.app` para testar.
7. Em **Project > Settings > Domains**, adicione seu domínio e configure os registros DNS **exatamente como a Vercel mostrar** no seu painel. Não altere registros de e-mail (MX/TXT) desnecessariamente.
8. Toda atualização enviada ao branch de produção do GitHub pode gerar novo deploy automaticamente.

## Executar no computador

Requer Node.js 20+.

```bash
npm install
npm run dev
```

Para testar build de produção:

```bash
npm run build
npm run preview
```

## Ajustes antes de publicar

- E-mail: variável `CONTACT_EMAIL` no início de `src/main.jsx`. O valor `contato@goa.com.br` é provisório e deve ser confirmado.
- Logo: `public/logo-goa.png`.
- Textos, serviços e skills: `src/main.jsx`.
- Cores e estilos: `src/styles.css`.
- O site não possui formulário de armazenamento de dados. Os botões de contato abrem o aplicativo de e-mail do visitante.
- Não há nomes de clientes nem cases identificáveis.

## Estrutura

```text
goa-landing/
├── index.html
├── package.json
├── public/
│   └── logo-goa.png
└── src/
    ├── main.jsx
    └── styles.css
```
