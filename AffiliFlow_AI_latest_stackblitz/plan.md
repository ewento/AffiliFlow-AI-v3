# AffiliFlow AI — Penambahbaikan Tiga Tab

## Keperluan dan pendekatan

- Tab 1 menjana tepat 10 content pendek mengikut slot masa Malaysia. Setiap item mempunyai mood, konteks, funnel (TOFU/MOFU/BOFU), fasa AIDA, jenis hook, tujuan CTA dan cerita ringkas yang sesuai dengan waktu.
- Tab 2 menjana tepat 6 post panjang. Setiap post disusun Hook → Problem → Agitation → Solution → Benefit → Proof → CTA, tetapi hasil siap baca kekal sebagai cerita natural tanpa tajuk framework. Nada mesti humanize, santai dan soft-sell.
- Tab 3 menjana tepat 3 idea video. Setiap idea mempunyai minimum Clip A + Clip B, setiap klip berdurasi 8 saat, dengan Clip C/D dibenarkan jika arc dan dialog memerlukannya. Setiap klip mempunyai slash stack 2–5 arahan, prompt lengkap, dialog/audio apabila sesuai dan continuity antara klip.
- QA sedia ada dikekalkan dan diperluaskan untuk panjang Tab 1, metadata funnel, bilangan video, klip dinamik, section prompt, slash stack dan kesinambungan.

## Struktur projek

- `index.html`: borang input dan halaman statik.
- `app.js`: state, panggilan API, normalisasi, QA dan rendering tiga tab.
- `netlify/functions/prompts.js`: schema dan prompt Gemini untuk intel, tiga tab serta recommendation.
- `netlify/functions/ai.js`: handler Gemini dan cleanup video.
- `content-validator.js` dan `dev-tests/`: pemeriksaan regresi.
- `manus-routes.json`: manifest route halaman.

## Reka bentuk

Gaya yang dipilih ialah **calm creator studio**: panel gelap sedia ada dikekalkan supaya perubahan fokus kepada kebolehgunaan dan pembacaan output. Metadata funnel dipaparkan sebagai badge ringkas, manakala content kekal bersih untuk copy-paste. Tab video menggunakan tab klip dinamik supaya C/D muncul hanya apabila diperlukan.

Core principles: output terus boleh digunakan, konteks masa konsisten, dakwaan produk terkawal, dan keputusan AI mudah disemak.

Brand voice: santai, jelas, tidak memaksa. Contoh CTA: “Simpan dulu kalau nak semak kemudian.” dan “Kalau sesuai dengan rutin awak, buka listing dan tengok variasi yang ada.”
