# BlackEnergy (2015) — Studi Kasus Serangan Siber pada Jaringan Listrik Ukraina

Repositori riset terbuka tentang serangan 23 Desember 2015 yang memadamkan listrik ±225.000 pelanggan di tiga wilayah Ukraina. Fokus: rantai serangan, prinsip ofensif, respons pertahanan, serta evaluasi etis-hukumnya.

`versi 0.1.0` · `2026-11-03` · `lisensi MIT` · `7 berkas`

## Ringkasan

Serangan tidak bertumpu pada exploitasi celah teknis, melainkan pada kombinasi spear-phishing, kredensial sah yang dicuri, dan persistensi berbulan-bulan sebelum eksekusi fisik melalui HMI/SCADA. Pemulihan cepat terjadi justru karena operator menutup breaker secara manual di gardu.

## Status rilis

| Versi | Tanggal | Fokus | Status |
| --- | --- | --- | --- |
| `v0.1.0` | 2026-11-03 | Kerangka dan ruang lingkup | **rilis saat ini** |
| `v0.2.0` | 2026-11-04 | Bagian A — analisis inti | direncanakan |
| `v0.3.0` | 2026-11-06 | Bagian B — strategi, hukum, relevansi | direncanakan |
| `v0.4.0` | 2026-11-07 | Materi presentasi dan visual | direncanakan |
| `v1.0.0` | 2026-11-09 | Rilis stabil — tooling lengkap | direncanakan |

## Struktur repositori

```text
blackenergy-cyberwarfare/
    .gitignore
    CHANGELOG.md
    LICENSE
    README.md
    VERSION
    docs/
        00-ringkasan-eksekutif.md
    references/
        daftar-pustaka.md
```

## Peta dokumen

| Dokumen | Isi |
| --- | --- |
| `docs/00-ringkasan-eksekutif.md` | Ringkasan eksekutif, angka kunci, temuan pokok |

## Cara pakai

```bash
git clone <url-repositori>
cd blackenergy-cyberwarfare
```

## Sumber

Rujukan utama: Lee et al. (2016) DUC 5, Assante et al. (2017) DUC 6, Greenberg (2019), Pollard (2024), serta literatur Indonesia tentang keamanan SCADA. Daftar lengkap pada `references/daftar-pustaka.md`.

> Repositori ini tidak memuat kode eksploitasi, kredensial, atau instruksi operasional untuk menyerang infrastruktur. Seluruh isi bersifat analitis dan defensif.

## Lisensi

MIT — lihat `LICENSE`.
