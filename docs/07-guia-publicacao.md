# 7. Guia de publicação no GitHub Pages

## 1. Criar o repositório

1. Acesse o GitHub e selecione **New repository**.
2. Use o nome `case-data-quality-logistica`.
3. Marque o repositório como **Public**.
4. Não adicione arquivos automáticos, pois o pacote já contém README e `.gitignore` não é necessário.

## 2. Enviar o pacote

1. Abra o repositório criado.
2. Selecione **Add file → Upload files**.
3. Arraste o conteúdo desta pasta, preservando `assets`, `data` e `docs`.
4. Use a mensagem de commit: `Publica estudo de caso de Data Quality em logística`.
5. Confirme o commit na branch `main`.

> Envie o conteúdo da pasta, não o arquivo ZIP. O GitHub não extrai o ZIP automaticamente.

## 3. Ativar o GitHub Pages

1. Acesse **Settings → Pages**.
2. Em **Build and deployment**, selecione **Deploy from a branch**.
3. Selecione a branch `main`.
4. Selecione a pasta `/(root)`.
5. Clique em **Save**.

O endereço esperado será:

`https://laismoreira07.github.io/case-data-quality-logistica/`

## 4. Validar antes de divulgar

- abrir a página no computador;
- abrir no celular em modo vertical;
- conferir se a página escolheu o GIF mobile;
- testar menu, links e navegação;
- verificar se nenhuma informação real foi enviada;
- aguardar a conclusão do workflow de Pages caso a página ainda não apareça.

## 5. Atualizações futuras

Arquivos alterados na branch `main` serão republicados automaticamente. Para pequenos ajustes, é possível editar `README.md` ou `index.html` diretamente no GitHub.

