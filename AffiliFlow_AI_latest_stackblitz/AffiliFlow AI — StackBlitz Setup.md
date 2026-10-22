# AffiliFlow AI — StackBlitz Setup

AffiliFlow AI memerlukan Node server untuk menjana Tab 1, Tab 2 dan Tab 3. Jangan buka `index.html` sebagai static preview sahaja.

## Jalankan aplikasi

Buka Terminal StackBlitz pada folder yang mengandungi `package.json` dan `server.js`, kemudian jalankan:

```bash
GEMINI_API_KEY="API_KEY_GEMINI_ANDA" npm start
```

Untuk keselamatan, jangan commit atau kongsi API key dalam fail projek.

Server akan menyediakan:

```text
http://localhost:3000
http://localhost:3000/.netlify/functions/ai
```

Buka Preview untuk **port 3000**. Jika StackBlitz memaparkan static HTML/iframe atau mesej `Endpoint AI tidak memulangkan JSON`, hentikan preview lama dengan `Ctrl+C` dan jalankan semula `npm start` dari folder root projek.

## Struktur root yang betul

```text
index.html
app.js
style.css
server.js
package.json
netlify.toml
netlify/functions/ai.js
netlify/functions/prompts.js
```

Tab 1, Tab 2 dan Tab 3 semuanya menggunakan endpoint AI yang sama. Oleh itu ketiga-tiganya memerlukan server Node dan `GEMINI_API_KEY` yang aktif.
