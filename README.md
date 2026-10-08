# Envio de Mensagens WhatsApp

Página simples para enviar uma mensagem de WhatsApp para uma lista de contatos, usando a API do [Whapi.Cloud](https://whapi.cloud/pt/). Não precisa saber programar.

## Publicar no GitHub Pages (uma vez só)

1. Crie um repositório no GitHub (pode ser privado se sua conta permitir Pages privado; senão, público — a página não contém nenhum token).
2. Envie o arquivo `index.html` para o repositório (botão **Add file → Upload files**).
3. Vá em **Settings → Pages**.
4. Em **Source**, escolha **Deploy from a branch**, selecione a branch `main` e a pasta `/ (root)`. Clique em **Save**.
5. Em 1 a 2 minutos o link aparece no topo dessa tela, algo como `https://seu-usuario.github.io/nome-do-repositorio/`.
6. Mande esse link para quem vai usar.

## Como usar (para o usuário final)

1. **Conectar**: cole o token do seu canal (no painel do Whapi) e clique em **Testar conexão**.
2. **Contatos**: importe uma planilha Excel/CSV com uma coluna **telefone** (e, se quiser, **nome**), ou cole a lista, um contato por linha.
3. **Mensagem**: escreva o texto. Use o botão **Inserir nome do contato** para personalizar.
   Se quiser, anexe uma **imagem (JPG, PNG, WEBP) ou um PDF** de até 10 MB. O texto vira a legenda do anexo.
4. **Enviar**: clique em **Enviar teste para mim** para conferir, depois em **Começar envio**. Deixe a página aberta até terminar.

Ao final, clique em **Baixar relatório** para ter a planilha com o resultado de cada envio.

## Boas práticas

- Envie só para quem conhece você ou pediu para receber, e ofereça a opção "responda SAIR".
- Número novo: comece com 20 a 30 mensagens por dia e aumente aos poucos.
- A página espera de 20 a 60 segundos entre mensagens e envia no máximo 50 por vez (ajustável em *Configurações avançadas*).
- A página lembra quem já recebeu e não reenvia, mesmo se for fechada no meio.

## Privacidade

O token e a lista de contatos ficam salvos apenas no navegador de quem usa a página. Eles são enviados somente para o Whapi, nunca para o GitHub.
