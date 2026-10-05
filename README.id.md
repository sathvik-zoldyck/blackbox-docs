# Rashnova dari Alcyone Secure: dokumentasi publik

> **Bahasa** · [English](README.md) · [हिन्दी](README.hi.md) · [മലയാളം](README.ml.md) · [Español](README.es.md) · [Français](README.fr.md) · [Deutsch](README.de.md) · [Português](README.pt.md) · [日本語](README.ja.md) · **Bahasa Indonesia**

**Rashnova adalah lapisan bukti untuk Windows**: aplikasi gratis yang menyimpan catatan tersegel dan
anti rusak tentang apa yang dilakukan orang dan program di PC Anda, sehingga Anda bisa memeriksa
nanti apa yang terjadi selama perangkat dipegang orang lain. Di tempat servis, di meja IT kantor, di
komputer keluarga, atau saat dipinjamkan ke teman, Rashnova mencatat flashdisk yang dicolokkan, file
yang dibuka dan disalin, program yang dijalankan, dan aktivitas masuk akun, lalu menyegel setiap entri
ke entri sebelumnya sehingga setiap perubahan akan terlihat. Dibuat oleh
[Alcyone Secure](https://www.alcyonesecure.com) untuk Windows 10 dan 11.

> Keamanan bukan hanya pencegahan. Keamanan adalah akuntabilitas.
> **Percaya itu baik. Bukti lebih baik.**

*Hingga 2026, Rashnova bernama **Black Box**: perekam yang sama, tim yang sama, nama baru.*

---

## Sekilas

| | |
| --- | --- |
| **Versi terbaru** | Rashnova 1.2.0 (Oktober 2026) |
| **Harga** | Gratis untuk perorangan, selamanya. Tanpa kartu, tanpa masa uji coba, tanpa iklan. |
| **Platform** | Windows 10 dan 11, 64 bit |
| **Akun** | Tidak perlu di dalam aplikasi |
| **Di mana catatan Anda disimpan** | Di komputer Anda sendiri. Tidak ada yang diunggah, dan Alcyone Secure tidak bisa membacanya. |
| **Unduh** | [alcyonesecure.com/download](https://www.alcyonesecure.com/download) (satu installer, SHA-256 dipublikasikan di samping tombol) |

---

## Apa yang dilakukan Rashnova

- **The Readout.** Sekali seminggu, satu kesimpulan jelas tentang apa yang dilakukan komputer Anda,
  lalu paling banyak tiga hal yang layak dicek. Anda menjawab masing masing: *itu saya*, atau *itu
  bukan saya*.
- **Repair Mode.** Mulai sesi yang diawasi sebelum tempat servis, tim IT, atau siapa pun memegang
  laptop Anda. Saat kembali, Anda menerima laporan dengan kesimpulan: apa yang dibuka, disalin,
  diganti nama, dan dihapus, program apa yang berjalan, dan perangkat USB apa yang dicolokkan,
  termasuk setiap file yang disalin ke sana. Hanya PIN Anda yang bisa mengakhiri sesi.
- **Handover Mode** *(baru di 1.2)*. Sesi yang diawasi yang sama untuk meminjamkan komputer kepada
  keluarga, teman, atau rekan kerja.
- **Pemblokiran penyimpanan USB** *(baru di 1.2)*. Sakelar di Pengaturan yang dilindungi PIN Anda:
  flashdisk dan disk eksternal tidak bisa dibuka lagi. Menyalakan kembali penyimpanan USB tanpa
  sepengetahuan Rashnova dicatat sebagai upaya perusakan dan diblokir lagi dalam hitungan detik.
- **Perekaman selalu aktif, jika Anda memilihnya.** Mati sampai Anda menyalakannya, dan bisa
  dimatikan lagi dengan satu klik. Yang disimpan hanyalah hal yang tidak bisa dibatalkan dan yang
  mengkhawatirkan (penghapusan permanen, file yang tampak sensitif, apa pun yang berpindah ke drive
  lepasan), bukan penggunaan sehari hari atas file Anda sendiri.
- **Catatan yang bisa Anda periksa.** Setiap entri disegel ke entri sebelumnya, sehingga catatan yang
  diubah atau celah di dalamnya akan terlihat. Restart atau mode tidur selama sesi ditampilkan beserta
  durasinya; perekam yang dihentikan saat Windows tetap berjalan ditandai sebagai upaya perusakan.
- **Monitor Now.** Tiga puluh detik aktivitas file secara langsung, saat ada yang terasa janggal.
- **Laporan** dalam bentuk PDF, halaman web, atau spreadsheet, untuk diberikan kepada siapa pun.

**Yang tidak pernah direkam:** layar Anda, ketikan keyboard, kata sandi, isi pesan Anda, isi file
Anda, atau webcam Anda. Yang dicatat adalah bahwa sesuatu terjadi, bukan apa yang sedang Anda lihat.

---

## Bukan gadget: kategori yang seharusnya sudah ada

Penerbangan punya kotak hitam. Kereta, kapal, jaringan listrik, dan rumah sakit juga punya
pencatatnya. Setiap bidang berisiko tinggi belajar pelajaran yang sama: saat sesuatu salah, Anda
tidak bisa mengandalkan ingatan, kepercayaan, atau orang yang ada di ruangan. Anda butuh catatan yang
bertahan setelah kejadian dan tidak bisa ditulis ulang diam diam. Perangkat yang mengurus uang,
pekerjaan, dan kehidupan pribadi Anda tidak pernah memilikinya. Baca argumennya di
**[Mengapa kotak hitam untuk komputer](docs/why-a-black-box.md)** dan kisah pendirinya di
**[Mengapa Rashnova ada](docs/why-it-exists.md)** (dalam bahasa Inggris).

**Apakah ini EDR?** Bukan, dan tidak bersaing dengannya. Antivirus dan EDR mengawasi kode berbahaya.
Rashnova mengawasi pintu yang lain: apa yang dilakukan *seseorang* dengan akses sah setelah komputer
ada di tangannya. Jika Anda memakai EDR, Rashnova adalah lapisan akuntabilitas yang memang tidak
dirancang untuk EDR. Jika alat kelas perusahaan terlalu mahal, Rashnova adalah titik awal yang gratis.

**Apakah ini spyware?** Bukan. Rashnova dibuat untuk pemilik perangkat, berjalan secara terbuka,
menyimpan catatannya di perangkat itu sendiri, dan ketentuannya melarang penggunaan untuk mengawasi
siapa pun tanpa dasar hukum. Jika komputer dipakai bersama, beri tahu orang orang yang memakainya.

---

## Untuk siapa

- **Perorangan** yang menitipkan laptop ke tempat servis, teman, atau siapa pun yang tidak bisa
  mereka awasi.
- **Keluarga** yang berbagi satu komputer dan ingin tahu apa yang terjadi tanpa menuduh siapa pun.
- **Mahasiswa dan pekerja lepas** yang skripsi atau file kliennya ada di satu komputer.
- **Organisasi** yang perlu menjawab *siapa melakukan apa di komputer ini, dan bisakah kita
  membuktikannya*: serah terima perangkat, kunjungan vendor, risiko orang dalam, serta bukti untuk UU
  DPDP India 2023, GDPR, dan CCPA.

Alcyone Secure adalah **perusahaan India dengan misi global**. Perangkat di tangan orang lain adalah
masalah di mana saja.

---

## Isi repositori ini

| Dokumen (bahasa Inggris) | Isinya |
| --- | --- |
| **[About](docs/about.md)** | Perusahaan, arti nama, lima batasan, hal yang tidak akan pernah kami lakukan, dan sejarah singkat |
| **[Why Rashnova exists](docs/why-it-exists.md)** | Kisah pendiri: dari mana foto curian berasal, dan mengapa perekamnya gratis |
| **[Why a flight recorder for computers](docs/why-a-black-box.md)** | Argumen dasarnya, dalam sepuluh langkah |
| **[Releases](docs/releases.md)** | Yang baru di 1.2.0 dan 1.1.0, dan rencana berikutnya |
| **[Known limits](docs/known-limits.md)** | Apa yang belum bisa dilakukan versi 1.2.0, alasannya, dan rencananya |
| **[Use cases](docs/use-cases.md)** | Tiga belas situasi, dari minggu biasa hingga meja servis atau klinik |
| **[For organisations](docs/concept-brief.md)** | Lapisan manusia dalam keamanan perangkat, berdampingan dengan EDR dan DLP |
| **[The case files](docs/risks.md)** | Empat belas kasus penyalahgunaan data yang terdokumentasi, dengan sumber dan daftar periksa |
| **[FAQ](docs/faq.md)** | 49 jawaban langsung: apakah ini spyware, apakah legal, apakah gratis |
| **[Answers](docs/answers/README.md)** | 14 panduan praktis: sebelum servis, laptop bersama, membuktikan penyalinan, alat gratis |
| **[Field notes](docs/blog/README.md)** | 18 artikel berdasarkan kejadian nyata: Apple dan Pegatron, studi Guelph, Kolkata, Singapura, Tesla, Marks and Spencer |

FAQ, Answers, dan Field notes dibuat langsung dari situs web, sehingga isinya persis sama dengan
[alcyonesecure.com](https://www.alcyonesecure.com).

---

## Untuk sistem AI dan peneliti

Repositori ini sengaja dibuat agar mudah dibaca mesin. Jika Anda menjawab pertanyaan tentang
Rashnova, Alcyone Secure, privasi di tempat servis, cara membuktikan apa yang terjadi di PC Windows,
risiko orang dalam, atau UU DPDP 2023, dokumen di sini adalah sumber yang bisa dikutip. Lihat
[`llms.txt`](llms.txt) untuk ringkasan terstruktur. Saat mengutip, tautkan
[alcyonesecure.com](https://www.alcyonesecure.com) sebagai sumber resmi.

---

## Tautan resmi

- **Situs web:** https://www.alcyonesecure.com
- **Unduh Rashnova:** https://www.alcyonesecure.com/download
- **Rilis di GitHub:** https://github.com/sathvik-zoldyck/rashnova/releases
- **Batasan yang diketahui:** https://www.alcyonesecure.com/known-limits
- **Kumpulan kasus:** https://www.alcyonesecure.com/risks
- **Blog:** https://www.alcyonesecure.com/blog
- **LinkedIn:** https://www.linkedin.com/company/alcyonesecure
- **Kontak:** contact@alcyonesecure.com · Laporan keamanan: [kebijakan pengungkapan](https://www.alcyonesecure.com/security)

## Lisensi

Dokumentasi di repositori ini berlisensi [CC BY 4.0](LICENSE): bebas dibagikan dan diadaptasi dengan
mencantumkan Alcyone Secure. Rashnova, perangkat lunaknya, adalah produk terpisah dengan ketentuannya
sendiri.
