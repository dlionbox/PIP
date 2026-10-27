# Pulse + Nitro — Painel de indicadores

Aplicação estática em HTML, CSS e JavaScript, sem etapa de build.

## Executar localmente

1. Baixe ou clone este repositório.
2. Abra `index.html` no navegador.

Para desenvolvimento, também é possível servir a pasta com um servidor HTTP local, por exemplo a extensão Live Server do VS Code.

## Publicar com GitHub Pages

1. Crie um repositório no GitHub e envie `index.html` para a raiz.
2. Abra **Settings → Pages**.
3. Em **Build and deployment**, selecione **Deploy from a branch**.
4. Escolha a branch principal (por exemplo, `main`) e a pasta `/ (root)`.
5. Salve e aguarde o GitHub gerar o link do site.

Também é possível publicar o repositório com Cloudflare Pages selecionando o repositório e usando a raiz como diretório de saída. Como o site é estático, não é necessário comando de build.

## Importante: persistência dos dados

Na versão atual, os dados são armazenados no `localStorage` do navegador. Isso significa que:

- cada pessoa terá seus próprios dados no próprio navegador;
- o cadastro feito por uma pessoa **não** aparecerá automaticamente para o restante do time;
- limpar os dados do navegador ou trocar de dispositivo pode fazer os dados locais deixarem de estar disponíveis;
- os botões de backup e exportação são úteis para cópias manuais, mas não substituem um banco de dados compartilhado.

**Publicar este repositório não cria, por si só, um banco de dados compartilhado.** Para o uso colaborativo pretendido, a próxima etapa é integrar um backend/banco (por exemplo, Supabase/PostgreSQL), definir autenticação e configurar políticas de acesso. Não publique chaves secretas no HTML ou no Git.

## Estrutura

```text
pulse-nitro-repositorio/
├── index.html
├── README.md
└── .gitignore
```
