# Despliegue en Cloudflare Workers & Pages

Este proyecto está configurado como sitio estático para Cloudflare Pages.

## Configuración recomendada en Cloudflare

- Framework preset: `None`
- Build command: `npm run build`
- Build output directory: `dist`
- Root directory: `/`

## Despliegue desde la terminal

```bash
npm install
npm run build
npm run deploy
```

El archivo `wrangler.toml` define `pages_build_output_dir = "dist"` para que Cloudflare use la misma carpeta de salida tanto en despliegues por Git como con Wrangler.
