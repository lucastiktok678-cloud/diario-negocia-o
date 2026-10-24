# Diário de Negociação

Site estático (HTML + CSS + JavaScript no mesmo arquivo), pronto para o GitHub Pages.

## Estrutura

```
/
├── index.html   ← o site inteiro (design, código e funcionalidades)
└── README.md    ← estas instruções
```

Não há outros arquivos: o `index.html` já contém todo o CSS e JavaScript. A única coisa externa são as fontes Inter e JetBrains Mono, carregadas do Google Fonts por endereço completo (`https://...`), que funciona em qualquer repositório.

## Como publicar (passo a passo)

1. Entre em https://github.com e faça login.
2. Clique em **New** (ou **+ → New repository**), escolha um nome (ex.: `diario-negociacao`), marque **Public** e clique em **Create repository**.
3. Na página do repositório, clique em **uploading an existing file**.
4. Arraste para lá os arquivos `index.html` e `README.md` (os arquivos em si, **não** a pasta nem o ZIP).
5. Clique em **Commit changes**.
6. Vá em **Settings → Pages**.
7. Em **Build and deployment → Source**, escolha **Deploy from a branch**.
8. Em **Branch**, selecione **main** e a pasta **/ (root)**, e clique em **Save**.
9. Aguarde 1 a 3 minutos. O endereço será:

   `https://SEU-USUARIO.github.io/NOME-DO-REPOSITORIO/`

## Por que aparecia o erro 404?

As causas mais comuns são:

- O arquivo não se chama exatamente `index.html` (tudo minúsculo). O arquivo que você enviou chamava-se `diario-negociacao__11_.html`; aqui ele já está renomeado.
- O `index.html` está dentro de uma subpasta, e não na raiz do repositório.
- O GitHub Pages não foi ativado em **Settings → Pages**, ou a branch/pasta escolhida está errada.
- Ainda não passaram alguns minutos desde a ativação.

## Atenção: seus dados ficam só no seu navegador

O site guarda trades, planos e configurações no **localStorage** do navegador. Isso significa que:

- Os dados **não** são enviados para o GitHub nem para nenhum servidor.
- Cada navegador/dispositivo tem os seus próprios dados (o computador e o telemóvel não se sincronizam).
- Limpar os dados do navegador apaga tudo.
- O endereço `SEU-USUARIO.github.io` guarda os dados separadamente de abrir o arquivo no computador (`file://`). Se você já tem dados no arquivo local, use **Exportar** no site antigo e **Importar** no novo.

Use regularmente o botão de **exportar cópia de segurança** do próprio site.

## Atualizar o site depois

No repositório, clique em `index.html` → ícone de lápis (ou **Add file → Upload files** para substituir) → **Commit changes**. A publicação é atualizada automaticamente.
