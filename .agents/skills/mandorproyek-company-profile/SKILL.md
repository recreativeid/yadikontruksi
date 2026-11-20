---
name: mandorproyek-company-profile
description: Panduan komprehensif, standar desain UI/UX, sistem warna, copywriting konversi tinggi, dan blueprint kode untuk membuat website company profile jasa kontraktor, mandor proyek, bangun baru, dan renovasi bangunan dengan gaya profesional terpercaya seperti MandorProyek.com.
---

# MandorProyek-Style Contractor Company Profile Skill

Skill ini memandu perancangan dan pembuatan website company profile untuk **jasa kontraktor, pemborong, mandor proyek, arsitek, dan renovasi bangunan** di Indonesia dengan standar visual, arsitektur informasi, dan daya konversi tinggi seperti yang diterapkan pada `MandorProyek.com`.

---

## 🏗️ 1. Filosofi & Psikologi Desain (Trust & High Conversion)

Konsumen jasa konstruksi di Indonesia umumnya memiliki 4 ketakutan utama:
1. **Trauma Mandor Kabur**: Proyek ditinggalkan di tengah jalan setelah uang muka dibayarkan.
2. **Biaya Membengkak (Mark-Up Liar)**: RAB awal murah, tetapi di tengah jalan muncul tagihan tambahan tak terduga.
3. **Kualitas Asal-asalan**: Bangunan retak rambut, dak bocor, material tidak sesuai spek SNI.
4. **Waktu Molor**: Pengerjaan terlambat berbulan-bulan tanpa kepastian.

Website bergaya **MandorProyek.com** dirancang untuk **meruntuhkan keempat ketakutan tersebut** sejak 5 detik pertama pengunjung membuka halaman melalui kombinasi:
- Estetika industrial modern yang solid dan berwibawa (warna helm proyek/safety yellow + dark charcoal).
- Transparansi alur kerja bertahap (sistem termin & SPK resmi).
- Tombol aksi instan (Direct WhatsApp & Kalkulator Estimasi Biaya).
- Bukti pengerjaan nyata (*Before & After*, foto proyek riil di lapangan, testimoni lokal).

---

## 🎨 2. Design System & Design Tokens

### A. Palet Warna (The Construction Safety & Slate Palette)
| Token | Hex Code | Peran & Penggunaan |
| :--- | :--- | :--- |
| **Primary Accent (Safety Gold)** | `#F5B332` / `#FFB703` | Warna ikonik safety helmet, alat berat (CAT), tombol CTA utama, highlight nomor langkah (`01.`, `02.`), dan badge promo. |
| **Primary Dark (Charcoal Slate)** | `#1A1D20` / `#242424` | Warna latar hero banner, header gelap, teks heading h1-h3, dan footer. Memberikan kesan pondasi kokoh. |
| **Secondary Dark** | `#2D3238` / `#343A40` | Background card gelap, border kontras, dan hover states. |
| **Pure White** | `#FFFFFF` | Latar kartu utama, kartu layanan, dan background section putih. |
| **Soft Surface Gray** | `#F8F9FA` / `#F4F6F8` | Latar belakang section selang-seling (agar visual tidak monoton dan mata tidak lelah). |
| **Text Primary** | `#1A1D20` | Teks heading dan judul kartu (Font-weight: 700 - 800). |
| **Text Muted / Body** | `#4A5568` / `#64748B` | Paragraf penjelasan, deskripsi layanan, dan catatan kaki (Font-weight: 400 - 500). |
| **WhatsApp Green** | `#25D366` | Tombol CTA WhatsApp melayang (Floating button) & direct hotline konsultasi cepat. |
| **Border / Divider** | `#E2E8F0` / `#E5E7EB` | Garis pemisah halus antar komponen atau baris tabel RAB. |

### B. Tipografi
- **Headings (Display)**: `Kumbh Sans`, `Plus Jakarta Sans`, atau `Inter` (Weights: `600`, `700`, `800`). Karakter huruf tegas, modern, dengan tracking sedikit rapat (`letter-spacing: -0.02em`).
- **Body Text**: `Inter`, `Roboto`, atau `Hind` (Weights: `400`, `500`). Nyaman dibaca pada layar smartphone dengan line-height proporsional (`1.6` - `1.75`).
- **Step Counters**: Bold Serif / Sans Display (`font-weight: 800; color: #F5B332; font-size: 2rem;`).

### C. Elemen Geometri & Efek Visual
- **Border Radius**: `8px` (`rounded-lg`) hingga `12px` (`rounded-xl`). Tidak terlalu bulat (pill) agar tetap mencerminkan karakter ketegasan arsitektural.
- **Card Shadow**: `box-shadow: 0 4px 20px -2px rgba(0, 0, 0, 0.06);` dengan transisi hover `translate-y: -4px` dan shadow lebih tegas saat di-hover.
- **Visual Cues**: Aksen garis kuning/emas di bawah judul section (`w-16 h-1 bg-[#F5B332] rounded-full mx-auto mt-3`).

---

## 📐 3. Cetak Biru Struktur Halaman (The 10-Part Master Layout)

Setiap halaman beranda (homepage) company profile kontraktor bergaya MandorProyek harus memiliki urutan seksi berikut:

```
┌────────────────────────────────────────────────────────┐
│ 1. TOPBAR (Telepon, WhatsApp, Jam Kerja, Minta Survei)  │
├────────────────────────────────────────────────────────┤
│ 2. STICKY NAVBAR (Logo, Menu Layanan, RAB, Portfolio)  │
├────────────────────────────────────────────────────────┤
│ 3. HERO BANNER + VALUE PROPOSITION + DUAL CTA BUTTON   │
│    [Konsultasi WhatsApp] [Hitung Estimasi Biaya]       │
├────────────────────────────────────────────────────────┤
│ 4. TRUST COUNTERS (+10 Thn, +250 Proyek, 100% Garansi) │
├────────────────────────────────────────────────────────┤
│ 5. 4 PILAR KEUNGGULAN (Quality, Integrity, Safety...)  │
├────────────────────────────────────────────────────────┤
│ 6. GRID LAYANAN UNGGULAN (Bangun, Renovasi, Desain...) │
├────────────────────────────────────────────────────────┤
│ 7. 4 LANGKAH ALUR KERJA (01 Survei -> 04 Serah Terima) │
├────────────────────────────────────────────────────────┤
│ 8. KALKULATOR ESTIMASI BIAYA INTERAKTIF (RAB Simpanan) │
├────────────────────────────────────────────────────────┤
│ 9. PORTOFOLIO SEBELUM & SESUDAH (Before / After Cards) │
├────────────────────────────────────────────────────────┤
│ 10. SOCIAL PROOF, TESTIMONI & REKANAN MATERIAL (SNI)   │
├────────────────────────────────────────────────────────┤
│ 11. FAQ ACCORDION (IMB/PBG, Termin, Garansi, Addendum) │
├────────────────────────────────────────────────────────┤
│ 12. FOOTER MEGA-LINKS & FLOATING WHATSAPP BUTTON (CTA) │
└────────────────────────────────────────────────────────┘
```

---

## 📝 4. Rincian & Copywriting Tiap Bagian

### 1. Top Bar Kontak Cepat
- **Tujuan**: Memudahkan klien menelepon langsung tanpa perlu mencari di halaman kontak.
- **Konten**:
  - Jam Layanan: *Senin - Sabtu: 08.00 - 17.00 WIB*
  - Hotline WhatsApp: *+62 8xx-xxxx-xxxx*
  - Email: *info@perusahaan.com*
  - Tombol aksi mini: *"Jadwalkan Survei Gratis"*

### 2. Hero Banner (The Hook)
- **Tagline Utama**: *"Jasa Bangun & Renovasi Rumah Profesional, Transparan & Bergaransi"*
- **Sub-tagline**: *"Wujudkan hunian impian Anda tanpa rasa cemas. Diawasi langsung oleh tim arsitek & mandor ahli, perhitungan RAB rinci tanpa biaya tersembunyi, serta jaminan garansi pemeliharaan tertulis."*
- **Aksi (CTA)**:
  - Tombol Utama (Kuning `#F5B332`): *"Konsultasi Gratis via WhatsApp"*
  - Tombol Sekunder (Outline / Netral): *"Hitung Estimasi Biaya (RAB)"*
- **Floating Badge**: *"Bebas Biaya Survei Lokasi & Konsultasi Awal"*

### 3. Empat Pilar Keunggulan (Why Choose Us)
Gunakan 4 pilar standar MandorProyek:
1. **Quality (Kualitas Pengerjaan & Material)**: Material SNI berkualitas pilihan (Semen Tiga Roda/Holcim, Bata Merah/Hebel standar industri, Baja Ringan Taso) dikerjakan oleh tukang spesialis.
2. **Integrity (Transparansi RAB & SPK Resmi)**: Rincian volume dan harga satuan bahan dijelaskan tuntas. Didukung Surat Perjanjian Kerja (SPK) legal bermeterai.
3. **Safety & Guarantee (Garansi Konstruksi)**: K3 ketat di area kerja dan pemberian Sertifikat Garansi Pemeliharaan (anti bocor, anti retak struktur) setelah serah terima kunci.
4. **Teamwork & Supervision (Pengawasan Proyek Ketat)**: Setiap proyek diawasi oleh Mandor Kepala & Project Manager berpengalaman dengan laporan progress berkala (foto & video).

### 4. Layanan Unggulan (Services Grid)
Sajikan 5-6 layanan utama dalam bentuk kartu interaktif:
1. **Jasa Bangun Rumah Baru**: Pembangunan dari nol (tanah kosong) hingga siap huni (Turnkey Project).
2. **Jasa Renovasi Rumah**: Renovasi tingkat (dak lantai 2), renovasi fasad tampak depan, perluasan dapur & ruang keluarga.
3. **Jasa Desain Arsitektur & 3D**: Pembuatan gambar kerja detail (DED), 3D render fotorealistik, dan pengurusan izin PBG/IMB.
4. **Pemasangan Atap Baja Ringan**: Penggantian struktur kayu lapuk ke rangka baja ringan anti karat dan genteng modern.
5. **Konstruksi Rooftop & Area Outdoor**: Pembuatan area santai keluarga, taman atap, dan ruang multifungsi bebas bocor.
6. **Desain Interior & Custom Furniture**: Kitchen set, wardrobe, partisi minimalis terintegrasi.

### 5. Alur Kerja 4 Langkah (The Proven 4-Step Workflow)
Tampilkan dengan nomor emas display berukuran besar (`#F5B332`):
- `01.` **Measurements & Konsultasi**: Anda mengirimkan permintaan dan tim surveyor kami datang ke lokasi untuk pengukuran eksisting (Gratis).
- `02.` **Calculation & RAB Terperinci**: Penyusunan Rencana Anggaran Biaya (RAB) detail dalam 24-48 jam dengan spesifikasi material yang disepakati.
- `03.` **Execution of Work & Termin**: Penandatanganan SPK resmi, eksekusi fisik di lapangan dengan skema pembayaran bertahap sesuai capaian progres nyata di lapangan.
- `04.` **Repairs are Ready & Serah Terima**: Inspeksi checklist bersama, serah terima kunci bangunan, dan penyerahan sertifikat garansi pemeliharaan (anti bocor & struktur).

### 6. Kalkulator Estimasi Biaya (Interactive RAB Estimator)
Komponen wajib untuk meningkatkan keterlibatan (*engagement*) pengunjung:
- **Input Pengunjung**:
  - Jenis Layanan: Bangun Baru / Renovasi Total / Renovasi Sebagian / Atap Baja Ringan
  - Estimasi Luas Bangunan ($m^2$)
  - Jumlah Lantai: 1 Lantai / 2 Lantai / 3 Lantai
  - Tipe Spesifikasi Material:
    - *Paket Standar* (Rp 3.500.000 - Rp 4.500.000 / $m^2$)
    - *Paket Menengah* (Rp 4.500.000 - Rp 6.000.000 / $m^2$)
    - *Paket Premium / Mewah* (Rp 6.500.000 - Rp 8.500.000+ / $m^2$)
- **Output Instan**:
  - Estimasi Range Biaya: e.g. `Rp 450.000.000 - Rp 520.000.000`
  - Tombol *"Kirim Hasil Perhitungan Ini ke WhatsApp untuk Detail RAB"*

### 7. Portofolio & Studi Kasus Riil (Before & After)
- Tampilkan foto nyata lapangan (bukan sekadar stok foto luar negeri).
- Format kartu portofolio:
  - Foto utama proyek (dengan slider/toggle *Sebelum & Sesudah* jika ada).
  - Judul: *"Renovasi Rumah 2 Lantai - Bpk. Anton, Jagakarsa"*
  - Spesifikasi: Luas: 160 $m^2$, Durasi: 90 Hari Kerja, Lingkup: Fasad & Dak Rooftop.

### 8. FAQ (Frequently Asked Questions)
Jawab langsung pertanyaan umum pelanggan:
1. *Apakah survei lokasi dan konsultasi awal benar-benar gratis?*
   - Ya, bebas biaya untuk wilayah jangkauan operasional kami tanpa kewajiban langsung kontrak.
2. *Bagaimana sistem pembayarannya? Apakah harus bayar penuh di depan?*
   - Tidak. Sistem pembayaran menggunakan sistem termin (misal: DP 20%, Termin 1 30%, Termin 2 30%, Termin Pelunasan 15%, Retensi Garansi 5%) berdasarkan progres fisik nyata di lapangan.
3. *Bagaimana jika ada perubahan material di tengah pengerjaan?*
   - Dikelola melalui dokumen resmi *Site Instruction* dan Addendum Kontrak agar biaya tetap transparan dan disetujui kedua pihak terlebih dahulu.
4. *Berapa lama garansi yang diberikan?*
   - Garansi pemeliharaan berkisar antara 3 hingga 6 bulan pasca serah terima kunci mencakup kebocoran atap/dak, kelistrikan, dan retak plesteran.

---

## 💻 5. Boilerplate & Kode Komponen Siap Pakai

Berikut adalah implementasi modern menggunakan **HTML5 + Tailwind CSS (atau Pure CSS) + Vanilla JS** yang siap disematkan langsung:

### A. Snippet Header & Topbar
```html
<!-- TOPBAR -->
<div class="bg-[#1A1D20] text-gray-300 text-xs py-2 px-4 border-b border-gray-800">
  <div class="max-w-7xl mx-auto flex flex-col md:flex-row justify-between items-center gap-2">
    <div class="flex items-center gap-6">
      <span><i class="fa-solid fa-clock text-[#F5B332] mr-1.5"></i>Senin - Sabtu: 08:00 - 17:00</span>
      <span><i class="fa-solid fa-location-dot text-[#F5B332] mr-1.5"></i>Jabodetabek & Sekitarnya</span>
    </div>
    <div class="flex items-center gap-4">
      <a href="tel:+6287888747476" class="hover:text-white transition"><i class="fa-solid fa-phone text-[#F5B332] mr-1.5"></i>+62 878-8874-7476</a>
      <a href="mailto:info@mandorproyek.com" class="hover:text-white transition"><i class="fa-solid fa-envelope text-[#F5B332] mr-1.5"></i>info@mandorproyek.com</a>
    </div>
  </div>
</div>

<!-- NAVBAR -->
<nav class="bg-white sticky top-0 z-50 shadow-sm border-b border-gray-100">
  <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 flex justify-between items-center h-20">
    <a href="#" class="flex items-center gap-3">
      <div class="w-10 h-10 bg-[#1A1D20] rounded flex items-center justify-center text-[#F5B332] font-black text-xl">
        <i class="fa-solid fa-helmet-safety"></i>
      </div>
      <div>
        <span class="text-xl font-extrabold text-[#1A1D20] tracking-tight">MANDOR<span class="text-[#F5B332]">PROYEK</span></span>
        <p class="text-[10px] tracking-wider text-gray-500 uppercase font-semibold">Kontraktor & Renovasi Bangunan</p>
      </div>
    </a>
    
    <div class="hidden md:flex items-center gap-8 font-medium text-gray-700 text-sm">
      <a href="#beranda" class="text-[#F5B332] font-semibold">Beranda</a>
      <a href="#keunggulan" class="hover:text-[#F5B332] transition">Keunggulan</a>
      <a href="#layanan" class="hover:text-[#F5B332] transition">Layanan</a>
      <a href="#alur-kerja" class="hover:text-[#F5B332] transition">Alur Kerja</a>
      <a href="#kalkulator" class="hover:text-[#F5B332] transition">Estimasi Biaya</a>
      <a href="#portofolio" class="hover:text-[#F5B332] transition">Portofolio</a>
    </div>

    <div>
      <a href="https://wa.me/6287888747476?text=Halo%20MandorProyek,%20saya%20ingin%20konsultasi%20proyek%20bangunan" 
         target="_blank"
         class="inline-flex items-center gap-2 bg-[#F5B332] hover:bg-[#e0a226] text-[#1A1D20] font-bold px-5 py-2.5 rounded-lg shadow-sm hover:shadow transition transform hover:-translate-y-0.5 text-sm">
        <i class="fa-brands fa-whatsapp text-lg text-emerald-800"></i>
        <span>Konsultasi Gratis</span>
      </a>
    </div>
  </div>
</nav>
```

### B. Snippet Hero Banner
```html
<section id="beranda" class="relative bg-[#1A1D20] text-white py-20 lg:py-28 overflow-hidden">
  <div class="absolute inset-0 bg-cover bg-center opacity-15" style="background-image: url('https://images.unsplash.com/photo-1541888946425-d0fbb1861593?q=80&w=1600&auto=format&fit=crop');"></div>
  <div class="absolute inset-0 bg-gradient-to-r from-[#1A1D20] via-[#1A1D20]/90 to-transparent"></div>

  <div class="relative max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
    <div class="max-w-2xl">
      <div class="inline-flex items-center gap-2 px-3 py-1.5 rounded-full bg-[#F5B332]/10 border border-[#F5B332]/30 text-[#F5B332] text-xs font-semibold mb-6">
        <i class="fa-solid fa-certificate"></i>
        Bebas Biaya Survei Lokasi & Konsultasi RAB
      </div>
      
      <h1 class="text-3xl sm:text-5xl font-extrabold tracking-tight leading-tight mb-6">
        Jasa Bangun & Renovasi Rumah <span class="text-[#F5B332]">Profesional</span>, Transparan & Bergaransi.
      </h1>
      
      <p class="text-gray-300 text-base sm:text-lg mb-8 leading-relaxed">
        Solusi kontraktor terpercaya di Jabodetabek. Perhitungan anggaran transparan tanpa mark-up liar, diawasi mandor berpengalaman, pengerjaan tepat waktu, dan garansi pemeliharaan resmi tertulis.
      </p>

      <div class="flex flex-col sm:flex-row gap-4 mb-12">
        <a href="https://wa.me/6287888747476?text=Halo,%20saya%20ingin%20jadwalkan%20survei%20lokasi" 
           class="inline-flex items-center justify-center gap-2 bg-[#F5B332] hover:bg-[#e5a010] text-[#1A1D20] font-bold px-7 py-3.5 rounded-lg shadow-md hover:shadow-lg transition text-base">
          <i class="fa-brands fa-whatsapp text-xl text-emerald-900"></i>
          Konsultasi & Jadwal Survei
        </a>
        <a href="#kalkulator" 
           class="inline-flex items-center justify-center gap-2 bg-white/10 hover:bg-white/20 text-white font-semibold px-7 py-3.5 rounded-lg border border-white/20 transition text-base">
          <i class="fa-solid fa-calculator text-[#F5B332]"></i>
          Hitung Estimasi Biaya
        </a>
      </div>

      <!-- Trust Badges -->
      <div class="grid grid-cols-3 gap-4 border-t border-gray-800 pt-8">
        <div>
          <div class="text-2xl sm:text-3xl font-black text-[#F5B332]">10+ Thn</div>
          <div class="text-xs text-gray-400 font-medium">Pengalaman Lapangan</div>
        </div>
        <div>
          <div class="text-2xl sm:text-3xl font-black text-[#F5B332]">250+</div>
          <div class="text-xs text-gray-400 font-medium">Proyek Tuntas</div>
        </div>
        <div>
          <div class="text-2xl sm:text-3xl font-black text-[#F5B332]">100%</div>
          <div class="text-xs text-gray-400 font-medium">Garansi Pemeliharaan</div>
        </div>
      </div>
    </div>
  </div>
</section>
```

### C. Snippet Alur Kerja 4 Langkah (The Signature 01-04 Workflow)
```html
<section id="alur-kerja" class="py-20 bg-gray-50">
  <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
    <div class="text-center max-w-2xl mx-auto mb-16">
      <span class="text-xs uppercase font-bold text-[#F5B332] tracking-widest">Transparan & Terstruktur</span>
      <h2 class="text-3xl font-extrabold text-[#1A1D20] mt-1">4 Langkah Mudah Mewujudkan Proyek Anda</h2>
      <div class="w-16 h-1 bg-[#F5B332] rounded-full mx-auto mt-3"></div>
      <p class="text-gray-600 mt-3 text-sm">Semua tahap dilakukan secara profesional dengan transparansi anggaran dan kontrak legal.</p>
    </div>

    <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 gap-8">
      <!-- Step 1 -->
      <div class="bg-white p-7 rounded-xl shadow-sm border border-gray-100 hover:shadow-md transition relative">
        <div class="text-4xl font-extrabold text-[#F5B332] mb-3">01.</div>
        <h3 class="text-lg font-bold text-[#1A1D20] mb-2">Survei & Pengukuran</h3>
        <p class="text-gray-600 text-xs leading-relaxed">
          Konsultasikan kebutuhan Anda. Tim surveyor kami akan datang ke lokasi proyek untuk mengukur kondisi eksisting secara akurat tanpa dipungut biaya.
        </p>
      </div>

      <!-- Step 2 -->
      <div class="bg-white p-7 rounded-xl shadow-sm border border-gray-100 hover:shadow-md transition relative">
        <div class="text-4xl font-extrabold text-[#F5B332] mb-3">02.</div>
        <h3 class="text-lg font-bold text-[#1A1D20] mb-2">Penyusunan RAB</h3>
        <p class="text-gray-600 text-xs leading-relaxed">
          Kami menyusun Rencana Anggaran Biaya (RAB) terperinci lengkap dengan spesifikasi material pilihan dalam waktu 24 jam sesuai pagu anggaran Anda.
        </p>
      </div>

      <!-- Step 3 -->
      <div class="bg-white p-7 rounded-xl shadow-sm border border-gray-100 hover:shadow-md transition relative">
        <div class="text-4xl font-extrabold text-[#F5B332] mb-3">03.</div>
        <h3 class="text-lg font-bold text-[#1A1D20] mb-2">Kontrak & Pengerjaan</h3>
        <p class="text-gray-600 text-xs leading-relaxed">
          Penandatanganan SPK legal. Pelaksanaan pengerjaan fisik dengan sistem pembayaran termin bertahap sesuai capaian progres nyata di lapangan.
        </p>
      </div>

      <!-- Step 4 -->
      <div class="bg-white p-7 rounded-xl shadow-sm border border-gray-100 hover:shadow-md transition relative">
        <div class="text-4xl font-extrabold text-[#F5B332] mb-3">04.</div>
        <h3 class="text-lg font-bold text-[#1A1D20] mb-2">Serah Terima & Garansi</h3>
        <p class="text-gray-600 text-xs leading-relaxed">
          Inspeksi checklist bersama, serah terima kunci bangunan, dan penyerahan sertifikat garansi pemeliharaan (anti bocor & struktur).
        </p>
      </div>
    </div>
  </div>
</section>
```

### D. Snippet Kalkulator RAB Interaktif (High Conversion Widget)
```html
<section id="kalkulator" class="py-20 bg-white">
  <div class="max-w-4xl mx-auto px-4 sm:px-6">
    <div class="bg-[#1A1D20] text-white rounded-2xl p-8 sm:p-12 shadow-xl border border-gray-800">
      <div class="text-center mb-8">
        <span class="text-xs uppercase font-bold text-[#F5B332] tracking-wider">Simulasi Anggaran</span>
        <h2 class="text-2xl sm:text-3xl font-extrabold mt-1">Kalkulator Estimasi Biaya Bangun / Renovasi</h2>
        <p class="text-gray-400 text-xs sm:text-sm mt-2">Dapatkan perkiraan biaya konstruksi awal secara instan sebelum melakukan survei.</p>
      </div>

      <div class="grid grid-cols-1 md:grid-cols-3 gap-6 mb-8 text-sm">
        <!-- Jenis Pekerjaan -->
        <div>
          <label class="block text-gray-300 font-semibold mb-2">Jenis Proyek</label>
          <select id="calc-tipe" class="w-full bg-[#2A2E33] border border-gray-700 text-white rounded-lg px-4 py-3 focus:outline-none focus:border-[#F5B332]">
            <option value="bangun">Bangun Rumah Baru</option>
            <option value="renovasi">Renovasi Menyeluruh</option>
            <option value="atap">Atap Baja Ringan & Plafon</option>
          </select>
        </div>

        <!-- Luas Bangunan -->
        <div>
          <label class="block text-gray-300 font-semibold mb-2">Luas Bangunan (m²)</label>
          <input type="number" id="calc-luas" value="100" min="20" max="2000" 
                 class="w-full bg-[#2A2E33] border border-gray-700 text-white rounded-lg px-4 py-3 focus:outline-none focus:border-[#F5B332]" />
        </div>

        <!-- Kualitas Material -->
        <div>
          <label class="block text-gray-300 font-semibold mb-2">Paket Material</label>
          <select id="calc-paket" class="w-full bg-[#2A2E33] border border-gray-700 text-white rounded-lg px-4 py-3 focus:outline-none focus:border-[#F5B332]">
            <option value="3500000">Standar (Rp 3,5 - 4,2 Jt/m²)</option>
            <option value="5000000" selected>Menengah (Rp 4,5 - 5,5 Jt/m²)</option>
            <option value="7500000">Premium / Mewah (Rp 6,5 - 8+ Jt/m²)</option>
          </select>
        </div>
      </div>

      <div class="bg-[#2A2E33] rounded-xl p-6 text-center border border-gray-700 mb-8">
        <div class="text-gray-400 text-xs uppercase font-medium tracking-wider mb-1">Perkiraan Total Anggaran</div>
        <div id="calc-result" class="text-3xl sm:text-4xl font-black text-[#F5B332]">Rp 500.000.000</div>
        <div class="text-gray-400 text-[11px] mt-1">*Estimasi belum termasuk furnish custom & izin PBG. RAB resmi dihitung pasca survei.</div>
      </div>

      <div class="text-center">
        <button id="calc-wa-btn" 
                class="inline-flex items-center gap-2 bg-[#F5B332] hover:bg-[#e0a226] text-[#1A1D20] font-bold px-8 py-3.5 rounded-lg shadow-md transition text-sm">
          <i class="fa-brands fa-whatsapp text-lg"></i>
          Kirim Rincian Simulasi Ini ke WhatsApp
        </button>
      </div>
    </div>
  </div>
</section>

<script>
  function updateEstimasi() {
    const luas = parseFloat(document.getElementById('calc-luas').value) || 0;
    const rate = parseFloat(document.getElementById('calc-paket').value) || 0;
    const total = luas * rate;
    document.getElementById('calc-result').innerText = 'Rp ' + total.toLocaleString('id-ID');
  }
  document.getElementById('calc-luas').addEventListener('input', updateEstimasi);
  document.getElementById('calc-paket').addEventListener('change', updateEstimasi);
  document.getElementById('calc-tipe').addEventListener('change', updateEstimasi);

  document.getElementById('calc-wa-btn').addEventListener('click', () => {
    const tipe = document.getElementById('calc-tipe').options[document.getElementById('calc-tipe').selectedIndex].text;
    const luas = document.getElementById('calc-luas').value;
    const paket = document.getElementById('calc-paket').options[document.getElementById('calc-paket').selectedIndex].text;
    const hasil = document.getElementById('calc-result').innerText;
    
    const msg = `Halo MandorProyek, saya ingin konsultasi estimasi:\n- Proyek: ${tipe}\n- Luas: ${luas} m2\n- Spesifikasi: ${paket}\n- Estimasi Awal: ${hasil}\n\nMohon info jadwal survei lokasi dan penyusunan RAB resminya. Terima kasih!`;
    window.open('https://wa.me/6287888747476?text=' + encodeURIComponent(msg), '_blank');
  });
</script>
```

---

## 🎯 6. Checklist Implementasi MandorProyek Style

Saat Anda diminta membangun website company profile kontraktor bergaya MandorProyek, pastikan item berikut terpenuhi:
- [ ] **Warna & Aksen**: Gunakan warna primer Charcoal Slate (`#1A1D20`) dan Safety Amber Gold (`#F5B332`).
- [ ] **Nomor Langkah Menyerupai MandorProyek**: Seksi Alur Kerja menggunakan nomor display besar berkarakter `01.`, `02.`, `03.`, `04.` dengan warna `#F5B332`.
- [ ] **Copywriting Anti-Cemas**: Masukkan frasa "Bebas Biaya Survei", "RAB Rinci Tanpa Mark-Up Liar", "Kontrak SPK Legal", "Pembayaran Bertahap Sesuai Progress", dan "Garansi Pemeliharaan Tertulis".
- [ ] **Kalkulator Biaya (Estimasi Cepat)**: Sediakan alat estimasi instan per meter persegi yang langsung bisa diteruskan ke WhatsApp tim penjualan.
- [ ] **Floating WhatsApp Button**: Tombol chat WA di pojok kanan bawah yang selalu tampak di desktop maupun mobile.
- [ ] **Mobile First & Fast Loading**: Struktur HTML ringan, pemuatan CSS cepat, gambar teroptimasi agar calon klien di ponsel pintar dapat membuka web dengan instan.
