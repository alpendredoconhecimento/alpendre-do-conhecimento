# Alpendre do Conhecimento — site

## Antes de publicar, falta só 1 coisa no `index.html`
O link do canal já está preenchido (@alpendredoconhecimento). Falta:

1. `SUBSTITUA_PELO_LINK_DO_RENDER` → o link do simulador de forragem depois
   que você publicar ele no Render (ex: `https://simulador-forragem-api.onrender.com`)
2. (opcional) O texto `[Espaço reservado...]` na seção "Sobre", no final da página

## Sobre a imagem de fundo
A imagem que você mandou está em `assets/fundo.jpg`, aplicada como marca
d'água bem clara atrás de todo o conteúdo (opacidade de 8%). Para ajustar a
intensidade, procure por `opacity: 0.08;` no `<style>` do `index.html` e
mude o número (0 = invisível, 1 = imagem cheia).

Se quiser destacar vídeos específicos na própria página (não só o botão pro
canal), tem um comentário no meio do HTML, na seção de vídeos, explicando
como adicionar cada um — é só colar o ID do vídeo.

## Publicar no GitHub Pages (gratuito, ~5 minutos)

Se você já criou a conta do GitHub para o simulador (passo anterior), pode
reaproveitar — não precisa de conta nova.

1. No GitHub, clique **+** → **New repository**.
2. Nome sugerido: `alpendre-do-conhecimento` → pode deixar **Public** desta
   vez (sites do GitHub Pages no plano gratuito precisam ser públicos) →
   **Create repository**.
3. **Add file** → **Upload files** → arraste `index.html` e a pasta `icons/`
   inteira → **Commit changes**.
4. Vá em **Settings** (aba do repositório) → **Pages** (menu lateral
   esquerdo).
5. Em **Source**, selecione **Deploy from a branch** → branch **main** →
   pasta **/ (root)** → **Save**.
6. Aguarde ~1 minuto e atualize a página — o GitHub mostra o link do site,
   algo como `https://seu-usuario.github.io/alpendre-do-conhecimento/`.

Pronto — esse link já é público e funciona em qualquer dispositivo.

## Domínio próprio (opcional, pra depois)
Se no futuro você comprar um domínio (ex: `alpendredoconhecimento.com.br`),
dá pra apontar ele pro GitHub Pages sem trocar nada no site: é só configurar
o DNS do domínio e adicionar o endereço em **Settings → Pages → Custom
domain**. Me avise quando chegar nessa etapa que eu te guio.

## Adicionando a próxima ferramenta
Quando a segunda ferramenta estiver pronta, duplique o bloco `.tool-card` no
`index.html` (o que hoje diz "Em breve") e preencha com o nome, descrição e
link dela. Mesmo processo de upload do passo 3 para atualizar o site no ar.
