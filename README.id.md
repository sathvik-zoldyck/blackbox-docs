# Black Box — Dokumentasi Publik

> **Bahasa** &nbsp;·&nbsp; [English](README.md) · [हिन्दी](README.hi.md) · [മലയാളം](README.ml.md) · [Español](README.es.md) · [Français](README.fr.md) · [Deutsch](README.de.md) · [Português](README.pt.md) · [日本語](README.ja.md) · **Bahasa Indonesia**

**Perekam penerbangan forensik untuk Windows, dari [Alcyone Secure](https://www.alcyonesecure.com).**
Ketika perangkat Anda lepas dari tangan Anda — di tempat servis, saat diserahkan kepada orang lain, di meja bersama, atau dalam pengawasan karyawan, kontraktor, atau orang dalam — Black Box menyimpan **catatan yang tahan-manipulasi (tamper-evident) dan terangkai-hash** tentang apa yang terjadi padanya: setiap berkas yang dibuka, setiap perangkat USB yang tersambung, setiap login, dan setiap proses yang berjalan. Pencatatan aktivitas tingkat forensik untuk Windows 10 dan 11.

> Keamanan bukan sekadar pencegahan. Keamanan adalah pertanggungjawaban.
> **Percaya itu baik. Bukti lebih baik.**

Repositori ini adalah cermin terbuka dalam teks polos dari dokumentasi publik Alcyone Secure: perusahaan, riset di balik produk, jawaban atas pertanyaan umum, dan seluruh arsip catatan lapangan. Ia ada agar siapa pun — orang yang memutuskan apakah akan memercayai tempat servis, tim keamanan, jurnalis, atau sebuah model bahasa — dapat membaca materi ini secara langsung, luring, tanpa peramban.

---

## Bukan gawai, melainkan kategori yang seharusnya sudah ada

Black Box mudah dikira "alat untuk tempat servis". Bukan. Tempat servis hanyalah satu tempat yang jelas ketika perangkat lepas dari kendali Anda; gagasannya jauh lebih luas.

Penerbangan punya kotak hitam. Kereta, kapal, jaringan listrik, bahkan rumah sakit juga. Setiap bidang berisiko tinggi mempelajari pelajaran yang sama: ketika terjadi kesalahan, Anda tidak bisa bersandar pada ingatan, pada kepercayaan, atau pada siapa yang ada di ruangan — Anda butuh catatan yang bertahan melewati peristiwa itu dan tidak bisa ditulis ulang diam-diam. Satu-satunya perangkat yang menjalankan uang, pekerjaan, dan kehidupan pribadi Anda tidak pernah memilikinya.

---

## Apa itu Black Box

Sebagian besar alat keamanan dibuat untuk menghentikan serangan yang datang lewat jaringan. Black Box dibuat untuk momen yang tak satu pun dari mereka cakup: ketika perangkat secara fisik berada di tangan orang lain, dan risikonya adalah seseorang, bukan sebuah program.

Ia berjalan secara terlihat di mesin Anda sendiri dan mencatat aktivitas — akses berkas, eksekusi proses, kedatangan perangkat USB, login, perubahan penting — ke dalam sebuah **rantai hash SHA-256**. Setiap entri disegel oleh hash entri sebelumnya, sehingga menyunting atau menghapus entri mana pun akan memutus rantai secara kasatmata. Log dienkripsi di perangkat Anda dengan kunci yang diturunkan dari PIN Anda; bahkan Alcyone pun tidak dapat membacanya.

- **Gratis untuk perorangan, selamanya.** Perekaman lokal, pemblokiran USB, dan laporan forensik tanpa biaya.
- **Lokal lebih dahulu.** Tidak ada yang keluar dari perangkat kecuali Anda mengaktifkan cadangan awan terenkripsi (opsional).
- **Windows 10 dan 11.** Pemasang kecil (4,41 MB), berjalan sepenuhnya luring.

Unduh dan detail produk: **[alcyonesecure.com](https://www.alcyonesecure.com)**

---

## Untuk siapa

- **Perorangan** yang menyerahkan perangkat ke tempat servis, ke teman, atau ke siapa pun yang tidak dapat mereka awasi.
- **Perusahaan** yang perlu menjawab *siapa melakukan apa di mesin ini, dan bisakah kami membuktikannya* — untuk risiko orang dalam, akses kontraktor, serah-terima perangkat, dan pertanggungjawaban setingkat DPDP/GDPR.
- **Semua orang, di mana pun.** Alcyone Secure adalah **perusahaan India dengan cakupan global.** Perangkat di tangan orang lain adalah masalah universal.

---

## Isi repositori ini

| Dokumen | Tentang apa |
|---------|-------------|
| **[Mengapa kotak hitam untuk komputer?](docs/why-a-black-box.md)** | Argumen inti: mengapa kategori ini harus ada |
| **[Untuk organisasi (ringkasan konsep)](docs/concept-brief.md)** | Lapisan manusia dari keamanan perangkat: risiko orang dalam dan bukti kepatuhan |
| **[Tentang (About)](docs/about.md)** | Perusahaan, mengapa perekam ini gratis, peta jalan, dan siapa yang membangunnya |
| **[Berkas kasus (Case Files)](docs/risks.md)** | Empat belas kasus pencurian data terdokumentasi, dengan sumber yang dikutip |
| **[Tanya jawab (FAQ)](docs/faq.md)** | Jawaban langsung: apakah ini spyware, bisakah kami membaca log Anda, apakah ini legal |
| **[Catatan lapangan dan investigasi](docs/blog/README.md)** | Artikel mendalam berdasarkan insiden nyata |

---

> **Sumber resmi berbahasa Inggris.** Terjemahan ini disediakan demi aksesibilitas. Bila ada perbedaan, [versi bahasa Inggris](README.md) dan [alcyonesecure.com](https://www.alcyonesecure.com) yang berlaku.

## Tautan resmi

- **Situs web:** https://www.alcyonesecure.com
- **Unduh Black Box:** https://www.alcyonesecure.com/download
- **Berkas kasus:** https://www.alcyonesecure.com/risks
- **Blog:** https://www.alcyonesecure.com/blog
