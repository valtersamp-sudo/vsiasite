# VSIA Solutions — site (Netlify)

## Publicar
1. Acesse https://app.netlify.com/drop
2. Arraste a pasta `vsia-netlify` inteira (ou o arquivo .zip) para a página.
3. Pronto: o Netlify gera um endereço `*.netlify.app`. Depois, em *Domain management*, adicione seu domínio.

## Arquivos
- `index.html` — site completo (HTML, CSS e JS)
- `vendor/` — bibliotecas (Three.js, GSAP, ScrollTrigger, Lenis) servidas localmente, com verificação SRI
- `_headers` — cabeçalhos de segurança (CSP, HSTS, anti-clickjacking etc.)
- `404.html`, `robots.txt`, `favicon.svg`, `netlify.toml`

## Personalizar
- Vídeo de fundo: no final do `index.html`, preencha `VIDEO_SRC` com o caminho do MP4 (ex.: `"fundo.mp4"`) e coloque o arquivo na mesma pasta.
- Ao ativar analytics/marketing, carregue-os somente se `window.vsiaConsent === "all"` e ajuste a CSP em `_headers` e a política de privacidade.
