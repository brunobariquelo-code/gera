# Gerador de RI para GitHub Pages

Versão totalmente estática. O DOCX é gerado no navegador a partir do modelo oficial; o PDF usa a impressão do navegador.

## Publicar
1. Envie `index.html` e `modelo-ri-template.docx` para a raiz do repositório.
2. Em **Settings > Pages**, selecione **Deploy from a branch**.
3. Escolha a branch `main` e a pasta `/ (root)`.
4. Aguarde a publicação e abra a URL do GitHub Pages.

## Observações
- Não envie `server.js`, `package.json` ou `node_modules`.
- A geração do DOCX exige internet para carregar PizZip e Docxtemplater pelo cdnjs.
- As fotos aparecem no PDF produzido pela opção **Imprimir / Salvar em PDF**. O DOCX informa que os registros fotográficos estão na versão PDF, pois a inserção de imagens no modelo exige módulo adicional ou backend.
- Os dados continuam no navegador por `localStorage`; não são enviados para servidor por esta versão.
