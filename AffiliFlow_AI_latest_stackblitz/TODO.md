# TODO — AffiliFlow AI

## Tab 1: 10 content pendek mengikut waktu

- [x] Hasilkan tepat 10 item mengikut slot masa yang disarankan.
- [x] Pastikan cerita pendek selaras dengan mood, rutin dan konteks waktu posting.
- [x] Paparkan metadata funnel TOFU/MOFU/BOFU, fasa AIDA, jenis hook dan tujuan CTA.
- [x] Kekalkan CTA yang pelbagai dan tidak hard-sell untuk semua item.

## Tab 2: 6-part daily content journey

- [x] Hasilkan enam bahagian berurutan: engagement opener, engagement follow-up + product bridge, educational, relatable problem, consideration/comparison dan soft BOFU decision.
- [x] Gunakan waktu 6:00 AM, 10:00 AM, 1:00 PM, 4:00 PM, 6:00 PM dan 9:00 PM.
- [x] Benarkan Part 1 kekal sebagai perbualan natural tanpa memaksa PAS, AIDA atau funnel.
- [x] Sediakan `readyPost` yang humanize dan `fallbackPost` untuk Part 2 apabila engagement sebenar belum berlaku.
- [x] Paparkan peranan journey, framework, funnel, CTA dan tujuh beat strategi dalam UI tanpa mencemarkan copy siap salin.
- [x] Halang dakwaan palsu seperti komen, recommendation atau interaksi komuniti yang belum berlaku.
- [x] Paksa julat `readyPost`: Part 1 25–60 perkataan, Parts 2–5 100–160 perkataan dan Part 6 120–180 perkataan.
- [x] Tolak `pautan rasmi`, engagement palsu dan Proof yang tidak bersandar pada fakta atau buyer-check.

## Tab 3: 3 post prompt video

- [x] Hasilkan tepat 3 idea video dengan 2–4 klip bersambung, setiap klip 8 saat.
- [x] Tambah metadata `videoRole`, `storyMode`, `targetEmotion`, `ctaMode` dan `totalDuration`.
- [x] Sediakan tujuan setiap klip serta variasi Hook → Problem/Curiosity → Product Value → CTA.
- [x] Gunakan Clip A dan B sebagai asas; tambah Clip C/D hanya apabila arc atau dialog memerlukan bahagian tambahan.
- [x] Hadkan dialog kepada maksimum 18 patah perkataan dan pastikan dialog selesai sebelum saat kelima.
- [x] Letakkan CTA pada klip terakhir sahaja; klip awal hanya boleh menggunakan curiosity atau soalan ringan.
- [x] Pastikan slash command sesuai dan prompt mengandungi continuity, visual, audio, dialog serta negative constraints.

## UI, Reset dan deployment

- [x] Sediakan UI workspace moden dengan form produk lengkap, upload gallery, advanced settings, responsive mobile, output cards dan modal bantuan.
- [x] Sediakan butang Reset yang mengosongkan semua input, gambar, checkbox, IndexedDB session dan hasil AI.
- [x] Sediakan `netlify.toml` dengan publish root, functions directory dan redirect `/api/ai` ke fungsi Netlify.
- [x] Beri mesej khusus apabila response HTML/iframe diterima menggantikan JSON endpoint AI.
- [x] Pastikan semua ID DOM yang diperlukan JavaScript tersedia dalam `index.html`.

## QA dan penghantaran

- [x] Luluskan syntax check, validator regression suite, static route check dan runtime JSON endpoint check.
- [ ] Live Gemini generation memerlukan `GEMINI_API_KEY` yang sah pada deployment.
- [ ] Browser E2E memerlukan pakej `playwright` yang tidak disertakan dalam repositori asal.
