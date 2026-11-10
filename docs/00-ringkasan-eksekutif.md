# Ringkasan Eksekutif

**Objek studi:** serangan siber terhadap jaringan listrik Ukraina pada 23 Desember 2015, dieksekusi
dengan keluarga malware **BlackEnergy** (varian BlackEnergy3).

**Tesis utama:** serangan ini bukan demonstrasi exploitasi celah teknis yang rumit, melainkan
operasi yang bertumpu pada *human factor* (spear-phishing), kredensial sah yang dicuri, dan
persistensi jangka panjang — lalu dieksekusi sebagai aksi fisik melalui penguasaan HMI/SCADA.

## Angka kunci

| Indikator | Nilai | Sumber |
| --- | --- | --- |
| Pelanggan kehilangan listrik | ±225.000 | Lee et al. (2016) |
| Perusahaan distribusi (oblenergo) terdampak | 3 | Lee et al. (2016) |
| Gardu terdampak | >30 | Lee et al. (2016) |
| Durasi pemadaman | 1–6 jam | Lee et al. (2016); Greenberg (2019) |
| Korban jiwa | 0 | laporan terbuka |
| Waktu pemulihan penuh | hitungan jam, bukan hari | Lee et al. (2016) |

## Temuan pokok

1. **Rantai serangan linier dan dapat dipetakan.** Setiap tahap (reconnaissance sampai *actions on
   objectives*) meninggalkan jejak yang terdokumentasi dalam laporan E-ISAC/SANS, sehingga kasus ini
   menjadi bahan latihan ideal untuk pemetaan Cyber Kill Chain maupun MITRE ATT&CK for ICS.
2. **Pertahanan yang menentukan justru bersifat low-tech.** Pemulihan cepat terjadi karena operator
   mendatangi gardu secara fisik dan menutup breaker manual — bukan karena alat deteksi canggih.
3. **Atribusi bersifat teknis-kontekstual.** Sandworm/Unit 74455 GRU dinilai paling mungkin, namun
   tanpa pengakuan resmi; laporan primer E-ISAC sendiri tidak melakukan atribusi formal.
4. **Dampak bersifat asimetris.** Tim penyerang berukuran kecil menghasilkan gangguan layanan publik
   berskala ratusan ribu pelanggan dengan biaya operasi yang relatif rendah.
5. **Kasus ini berulang dan berevolusi.** 2016 (CrashOverride/Industroyer) membuktikan otomatisasi
   serangan terhadap protokol industri; 2017 (NotPetya) menunjukkan eskalasi menjadi kerusakan global.

## Peta repositori

| Berkas | Isi |
| --- | --- |
| `docs/01`–`docs/06` | Analisis Bagian A: konteks, aktor, kill chain, prinsip ofensif, dampak, mitigasi |
| `docs/07`–`docs/09` | Bagian B: strategi pertahanan, evaluasi etis-hukum, relevansi Indonesia |
| `docs/10`–`docs/12` | FAQ pemantik, glosarium, metodologi dan batasan |
| `data/` | Dataset terstruktur (kill chain, dampak, pemetaan ATT&CK, timeline) |
| `slides/` | Kerangka deck dan narasi presenter |
| `scripts/` | Validator data, generator dokumentasi, pengemas rilis |

> Catatan: seluruh angka pada repositori ini bersumber dari laporan terbuka. Tidak ada data
> korban, kredensial, atau artefak malware yang disertakan.
