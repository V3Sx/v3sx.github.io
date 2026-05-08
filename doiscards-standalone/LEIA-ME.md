# dois cards — PWA

Uma sala privada para dois. Dois cards por dia.

## Como instalar no celular (sem app store)

### iPhone / iPad (Safari)
1. Abra o arquivo `index.html` em um servidor web (veja abaixo)
2. No Safari, toque no botão de **compartilhar** (ícone de caixa com seta)
3. Role até encontrar **"Adicionar à Tela de Início"**
4. Toque em **Adicionar**
5. O app aparece na tela inicial como qualquer app nativo

### Android (Chrome)
1. Abra o app no Chrome
2. Toque nos **três pontos** (menu)
3. Toque em **"Instalar app"** ou **"Adicionar à tela inicial"**
4. Confirme

---

## Como hospedar (opções gratuitas)

### Opção 1 — Netlify Drop (mais fácil, 2 minutos)
1. Acesse https://app.netlify.com/drop
2. Arraste a **pasta doiscards-standalone** inteira para a página
3. Copie o link gerado e compartilhe com o parceiro
4. Pronto!

### Opção 2 — GitHub Pages
1. Crie um repositório no GitHub
2. Suba os arquivos desta pasta
3. Vá em Settings → Pages → Source: main branch
4. Seu app estará em `https://seu-usuario.github.io/nome-repo`

### Opção 3 — Vercel
1. Instale: `npm i -g vercel`
2. Na pasta: `vercel --prod`
3. Link gerado automaticamente

---

## Como usar

1. **Criar sala**: uma pessoa cria e compartilha o código (5 letras)
2. **Entrar**: a outra pessoa digita o código
3. **Publicar**: cada um escreve seu card do dia
4. **Ler**: após publicar, o card do parceiro fica visível
5. **Avaliar**: 1–5 estrelas com rótulo emocional

Os dados ficam salvos no dispositivo (localStorage). Para sincronizar entre celulares diferentes, use a mesma rede ou hospede em servidor compartilhado.

---

## Estrutura
```
doiscards-standalone/
├── index.html      ← app completo (React via CDN)
├── manifest.json   ← config PWA
├── icon-192.png    ← ícone
└── icon-512.png    ← ícone
```
