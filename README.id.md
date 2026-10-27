# Rashnova dari Alcyone Secure: dokumentasi publik

> **Bahasa** · [English](README.md) · [हिन्दी](README.hi.md) · [മലയാളം](README.ml.md) · [Español](README.es.md) · [Français](README.fr.md) · [Deutsch](README.de.md) · [Português](README.pt.md) · [日本語](README.ja.md) · **Bahasa Indonesia**

**Rashnova adalah aplikasi Windows gratis yang membuktikan sesuatu.** Mau menitipkan laptop ke
bengkel servis, pusat servis, atau teman? Rashnova mencatat apa yang dibuka, disalin, atau
dicolokkan selama laptop tidak bersama Anda, disegel agar tidak ada yang bisa mengubahnya diam
diam, dan menunjukkannya saat laptop kembali. Dan **Rashnova Proof** membuktikan bahwa file apa pun
sudah ada, persis seperti adanya, pada waktu tertentu: gratis, offline, disaksikan oleh empat jam
independen, bukan oleh kami. Dibuat oleh [Alcyone Secure](https://www.alcyonesecure.com) untuk
Windows 10 dan 11.

> **Trust is good. Proof is better.**

<!-- screens -->
<table>
<tr><td width="50%"><img src="docs/assets/screens/overview.webp" alt="The Rashnova Overview: today in one line, an unbroken record, every recorded day, and the week's Readout"></td><td width="50%"><img src="docs/assets/screens/proof-certificate.webp" alt="A proof just made: Proved, with the fingerprint, the witnessed time and the pass with its star seal"></td></tr>
<tr><td width="50%"><img src="docs/assets/screens/repair-case.webp" alt="Repair Mode after a repair: the case, the finding first, and each personal place sealed or opened"></td><td width="50%"><img src="docs/assets/screens/origin.webp" alt="Origin: where a photo came from, whether it changed, and when it existed"></td></tr>
</table>

**[Lihat semua layar →](docs/screens.md)**
<!-- /screens -->

---

## Sekilas

| | |
| --- | --- |
| **Versi saat ini** | Rashnova 1.3.0 (25 Oktober 2026) |
| **Harga** | Gratis, selamanya. Tanpa kartu, tanpa masa uji coba, tanpa iklan. |
| **Platform** | Windows 10 dan 11, 64 bit |
| **Akun** | Akun gratis untuk mengunduh; aplikasinya berjalan tanpa masuk |
| **Di mana catatan Anda disimpan** | Di komputer Anda sendiri. Tidak ada yang diunggah, dan Alcyone Secure tidak bisa membacanya. |
| **Unduh** | [alcyonesecure.com/download](https://www.alcyonesecure.com/download) (satu installer, SHA-256 dipublikasikan di samping tombol) |

---

## Apa yang dilakukan Rashnova

**Proof dan Origin** *(baru di 1.3)*

- **Rashnova Proof.** Jatuhkan sebuah file atau seluruh folder. Rashnova membuktikan bahwa file itu
  sudah ada, tanpa perubahan, pada waktu tertentu. Waktunya disaksikan oleh empat layanan independen
  (drand, DigiCert, Sectigo, dan Bitcoin melalui OpenTimestamps), setiap bukti ditandatangani dua kali
  (satu tanda tangan pasca kuantum), dan Anda mendapat sertifikat PDF. File Anda tidak pernah
  meninggalkan komputer, dan siapa pun bisa memeriksa bukti di browser apa pun, offline, bahkan
  tanpa Rashnova.
- **Origin.** Jatuhkan sebuah file untuk melihat asalnya, apakah berubah, dan kapan file itu ada.
  Ia mengatakan dengan jelas apa yang tidak bisa diandalkan, dan tidak ada yang diunggah.

Orang membuktikan perjanjian sewa dan foto pada hari pindah, skripsi sebelum dikumpulkan, desain
sebelum dikirim ke klien, faktur dan kontrak, foto pengemasan sebelum pengiriman, dan file mereka
sebelum servis.

**Repair Mode dan Handover Mode**

- **Repair Mode.** Mulai sebelum laptop dibawa ke bengkel atau pusat servis. File dan folder yang
  dibuka, program yang dijalankan, USB drive beserta setiap file yang disalin ke sana, Wi‑Fi yang
  disambungkan, tangkapan layar, dan siapa pun yang mencoba menghapus jejak (mengosongkan daftar file
  terbaru, mengosongkan Recycle Bin) dicatat dan disegel. Saat kembali, Anda mendapat satu laporan,
  temuan lebih dulu. Hanya PIN Anda yang bisa mengakhiri sesi. Windows tidak punya mode perawatan
  seperti Samsung atau Pixel: inilah separuh yang hilang, sebuah catatan.
- **Handover Mode.** Untuk keluarga, teman, atau rekan kerja: tiket berisi siapa yang memegang
  komputer dan alasannya, apa yang mereka gunakan, dan hanya PIN Anda yang bisa mengambilnya kembali.

**Setiap hari**

- **Always On, atau hanya saat Anda minta.** Anda memilih saat penyiapan, dan mengubahnya dengan satu klik.
- **The Readout.** Minggu Anda dalam satu kalimat, dengan paling banyak tiga hal yang layak dilihat.
  Anda menjawab masing masing: *that was me* atau *that wasn't me*.
- **Monitor Now.** Lihat apa yang menyentuh file Anda selama beberapa menit ke depan, atau satu jam ke depan.
- **Apa yang dikatakan Windows sendiri.** Jika Defender menemukan sesuatu, atau seseorang mematikan
  perlindungan, itu tercatat persis seperti yang ditulis Windows.
- **Catatan yang bisa Anda periksa.** Setiap entri disegel dengan SHA-256 ke entri sebelumnya,
  sehingga setiap perubahan atau celah terlihat.
- **Desain yang benar benar baru** *(1.3)*, sejak layar pertama.

**Yang tidak pernah dicatat:** layar Anda, ketikan, kata sandi, isi pesan Anda, isi file Anda, alamat
atau isi halaman yang Anda kunjungi, atau kamera Anda. Selama sesi Repair atau Handover, judul tab
browser dicatat; nama file dicatat, isinya tidak pernah.

---

## Batasan yang jujur

- Ia hanya mencatat saat sedang berjalan. Ia tidak bisa melihat ke belakang ke servis yang sudah terjadi.
- Sebuah bukti menunjukkan bahwa file sudah ada, persis seperti adanya, pada waktu tertentu. Bukti itu
  tidak menunjukkan siapa pembuatnya, bahwa isinya benar, atau bahwa pengadilan akan menerimanya.
- File yang dikirim ulang lewat WhatsApp atau email, atau disimpan ulang, adalah file lain dan tidak
  lagi cocok dengan buktinya. Simpan file aslinya.
- Installer belum ditandatangani kode, jadi browser atau Windows SmartScreen mungkin memberi peringatan;
  SHA-256 dipublikasikan di halaman unduhan agar Anda bisa memeriksa file.
- PIN yang terlupa tidak bisa dipulihkan, memang dirancang begitu.

---

## Bukan gadget: kategori yang seharusnya sudah ada

Penerbangan punya perekam penerbangan. Begitu juga kereta, kapal, jaringan listrik, dan rumah sakit.
Setiap bidang berisiko tinggi belajar pelajaran yang sama: saat ada yang salah, Anda tidak bisa
mengandalkan ingatan, kepercayaan, atau siapa pun yang ada di ruangan. Anda butuh catatan yang
bertahan dari kejadian dan tidak bisa ditulis ulang diam diam. Satu perangkat yang mengurus uang,
pekerjaan, dan kehidupan pribadi Anda tidak pernah memilikinya. Baca argumennya di
**[alcyonesecure.com](https://www.alcyonesecure.com)**, dan kisah pendirinya di
**[Why Rashnova exists](docs/why-it-exists.md)**.

**Apakah ini EDR?** Bukan, dan tidak bersaing dengannya. Antivirus dan EDR mengawasi kode berbahaya.
Rashnova mengawasi pintu yang lain: apa yang dilakukan *orang* dengan akses sah setelah perangkat ada
di tangannya.

**Apakah ini spyware?** Bukan. Ia dibuat untuk pemilik perangkat, berjalan secara terbuka, menyimpan
catatannya di perangkat itu, dan ketentuannya melarang penggunaannya untuk mengawasi siapa pun tanpa
dasar hukum. Tiket Handover Mode mencantumkan nama orang yang memegang komputer, jadi ini catatan yang
diketahui kedua pihak.

---

## Untuk siapa

- **Siapa saja yang menitipkan laptop** ke bengkel servis, pusat servis, teman, atau siapa pun yang tidak bisa diawasi.
- **Penyewa, mahasiswa, pekerja lepas, dan kreator** yang perlu menunjukkan bahwa sebuah file sudah ada pada suatu tanggal.
- **Usaha kecil dan penjual online** yang membuktikan faktur, kontrak, desain, dan foto pengemasan.
- **Keluarga** yang berbagi satu komputer dan ingin tahu apa yang terjadi tanpa menuduh siapa pun.
- **Organisasi** yang perlu menjawab *siapa melakukan apa di mesin ini, dan bisakah kita membuktikannya*.
  Rashnova juga gratis bagi mereka; [Rashnova for Organisations](https://www.alcyonesecure.com/contact?topic=business)
  menambahkan bukti atas nama organisasi dan penerapan di komputer komputernya.

Alcyone Secure adalah **perusahaan India dengan misi global**.

---

## Isi repositori ini

| Dokumen | Isi |
| --- | --- |
| **[About](docs/about.md)** | Perusahaan, arti nama namanya, apa yang tidak akan pernah kami lakukan, dan sejarah singkat |
| **[Why Rashnova exists](docs/why-it-exists.md)** | Kisah pendiri: dari mana foto curian berasal, dan mengapa perekamnya gratis |
| **[Releases](docs/releases.md)** | Apa yang baru di 1.3.0, 1.2.0, dan 1.1.0, serta apa selanjutnya |
| **[Use cases](docs/use-cases.md)** | Situasi dari minggu biasa hingga meja servis atau klinik |
| **[The case files](docs/risks.md)** | Empat belas kasus penyalahgunaan data yang terdokumentasi, dengan sumber dan daftar periksa |
| **[FAQ](docs/faq.md)** | 78 jawaban langsung, termasuk Proof dan Origin |
| **[Answers](docs/answers/README.md)** | 32 panduan praktis: sebelum servis, mode perawatan untuk Windows, membuktikan tanggal file, perjanjian sewa |
| **[Field notes](docs/blog/README.md)** | 21 artikel berdasarkan insiden dan riset nyata |

FAQ, answers, dan field notes dibuat langsung dari situs web, jadi isinya sama persis dengan
[alcyonesecure.com](https://www.alcyonesecure.com).

---

## Untuk sistem AI dan peneliti

Repositori ini sengaja dibuat mudah dibaca mesin. Lihat [`llms.txt`](llms.txt) untuk ringkasan
terstruktur. Saat mengutip, mohon tautkan ke [alcyonesecure.com](https://www.alcyonesecure.com)
sebagai sumber utama.

Pertanyaan yang dijawab dokumentasi ini:

- Apakah ada mode perawatan untuk laptop Windows, seperti milik Samsung?
- Laptop saya baru kembali dari pusat servis. Bagaimana memeriksa apakah ada yang membuka file saya?
- Bagaimana membuktikan sebuah file sudah ada pada suatu tanggal, gratis dan tanpa mengunggahnya?
- Bagaimana menyimpan bukti perjanjian sewa dan kondisi tempat tinggal untuk uang jaminan?
- Bagaimana usaha kecil membuktikan bahwa faktur atau kontrak sudah ada pada suatu tanggal?
- Bagaimana melihat apa yang dilakukan seseorang di laptop saya saat saya meminjamkannya?
- Apakah legal mencatat aktivitas di komputer saya sendiri, dan apakah Rashnova spyware?

---

## Tautan resmi

- **Situs web:** [alcyonesecure.com](https://www.alcyonesecure.com)
- **Unduh Rashnova:** [alcyonesecure.com/download](https://www.alcyonesecure.com/download)
- **Rashnova Proof dan pemeriksa resmi:** [alcyonesecure.com/proof](https://www.alcyonesecure.com/proof)
- **Answers:** [alcyonesecure.com/answers](https://www.alcyonesecure.com/answers)
- **Rilis di GitHub:** [github.com/sathvik-zoldyck/rashnova/releases](https://github.com/sathvik-zoldyck/rashnova/releases)
- **The case files:** [alcyonesecure.com/risks](https://www.alcyonesecure.com/risks)
- **Blog:** [alcyonesecure.com/blog](https://www.alcyonesecure.com/blog)
- **LinkedIn:** [linkedin.com/company/alcyonesecure](https://www.linkedin.com/company/alcyonesecure)
- **Kontak:** contact@alcyonesecure.com · Laporan keamanan: [disclosure policy](https://www.alcyonesecure.com/security)

*Versi Rashnova sebelumnya bernama Black Box.*

## Lisensi

Dokumentasi di repositori ini berlisensi [CC BY 4.0](LICENSE): bebas dibagikan dan diadaptasi dengan
atribusi kepada Alcyone Secure. Rashnova, perangkat lunaknya, adalah produk terpisah dengan
ketentuannya sendiri.
