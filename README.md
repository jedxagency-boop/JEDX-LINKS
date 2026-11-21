# JEDX · Links

Página de links (link in bio) de JEDX, servida con **Cloudflare Workers** (static assets).

```
public/index.html   ← la página
wrangler.jsonc      ← configuración del Worker
```

## Publicar en Cloudflare (desde GitHub, sin instalar nada)

1. Cloudflare → **Workers & Pages** → **Create** → **Import a repository**.
2. Conecta GitHub y elige `jedxagency-boop/JEDX-LINKS`.
3. Deja los valores por defecto (comando de deploy: `npx wrangler deploy`) y pulsa **Deploy**.
4. Queda en `https://jedx-links.<tu-subdominio>.workers.dev`. Cada `git push` a `main` vuelve a publicar.

## Publicar desde tu PC

```bash
npm install
npx wrangler login
npm run deploy
```

## Editar

Los datos (WhatsApp, web, planes y proyectos) están al inicio del `<script>` en `public/index.html`, en el bloque **CONFIGURA AQUÍ**.
