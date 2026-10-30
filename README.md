# Drib Camisas

Catálogo da Drib, loja de camisas de time. O cliente escolhe a camisa e o tamanho, e o botão de compra abre o WhatsApp da loja com a mensagem pronta.

Site estático: um único `index.html` e a pasta `img/`. Não precisa de instalação nem de build.

## Como atualizar

Tudo que muda no dia a dia fica no começo do `<script>` do `index.html`:

- `LOJA.whatsapp`: número do WhatsApp (DDI + DDD + número, só dígitos).
- `PRODUTOS`: cada camisa, com nome, preço, descrição, fotos e tamanhos.
  - `tamanhos`: tamanhos que a camisa tem.
  - `esgotados`: tamanhos que acabaram. Aparecem riscados e não podem ser escolhidos. Se todos acabarem, a camisa ganha a etiqueta "Esgotado".
- `MEDIDAS`: tabela de medidas masculina e feminina.

Fotos novas vão em `img/`, de preferência quadradas e com até 1000 px.

## Publicação

O site roda na Vercel como site estático. Cada envio para a branch `main` atualiza o site automaticamente.
