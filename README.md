# meta-legal

Halaman legal publik untuk aplikasi Meta (MKA Ads Manager).

Disajikan sebagai situs statis lewat Cloudflare Pages, domain `legal.mka.my.id`.
Sumber tunggal: folder `public/`. Setiap `git push` ke `main` memicu deploy otomatis.

## Halaman

- `/` — indeks
- `/meta-privacy` — Privacy Policy
- `/meta-terms` — Terms of Service
- `/meta-data-deletion` — User Data Deletion
- `/icon-1024.png` — ikon aplikasi

Cloudflare Pages melayani `/meta-privacy` dari berkas `meta-privacy.html` tanpa perlu aturan tambahan.

## Deploy manual

```bash
git add -A && git commit -m "update" && git push
```

Build: tanpa perintah build, output directory `public`.

## Riwayat

Sebelumnya disajikan dari VPS lewat Caddy dan Cloudflare Tunnel. Dipindahkan ke
Cloudflare Pages agar tidak bergantung pada satu mesin. Salinan VPS tetap ada
sebagai cadangan dan bisa diaktifkan kembali dengan mengubah satu record DNS.
