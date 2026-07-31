# Site High Speed

Site institucional da High Speed Internet Fibra Óptica — `index.html` na raiz, com as imagens organizadas na pasta `images/`.

## Como publicar no GitHub Pages

1. Crie um repositório novo no GitHub (pode ser público ou privado, desde que o plano permita Pages).
2. Envie o conteúdo desta pasta para o repositório:
   ```
   cd "C:\Users\lucio\Documents\Site Highspeed"
   git init
   git add .
   git commit -m "Publica site High Speed"
   git branch -M main
   git remote add origin https://github.com/SEU-USUARIO/SEU-REPOSITORIO.git
   git push -u origin main
   ```
3. No GitHub, vá em **Settings > Pages**.
4. Em "Build and deployment", selecione **Deploy from a branch**.
5. Escolha a branch **main** e a pasta **/ (root)**.
6. Salve. Em alguns minutos o site estará disponível em:
   `https://SEU-USUARIO.github.io/SEU-REPOSITORIO/`

O arquivo `.nojekyll` já está incluído para evitar que o GitHub Pages tente processar o site com Jekyll (não é necessário e pode causar problemas com arquivos grandes).

## Estrutura de arquivos

```
index.html      → página do site
images/          → todas as fotos, banners e logos usados (66 arquivos, ~4,9 MB)
.nojekyll         → evita processamento Jekyll no GitHub Pages
```

Mantenha a pasta `images/` no mesmo nível do `index.html` ao publicar — o site referencia as imagens por caminho relativo (ex.: `images/deezer.png`).
