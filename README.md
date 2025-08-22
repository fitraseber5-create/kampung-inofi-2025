
<html lang="id">
<head>
  <!-- Google tag (gtag.js) -->
<script async src="https://www.googletagmanager.com/gtag/js?id=G-4J85S9CN6X"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());

  gtag('config', 'G-4J85S9CN6X');
</script>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>KAMPUNG INOFI</title>
  <style>
    @keyframes waveIn {
      0% {
        opacity: 0;
        transform: translateY(30px);
        clip-path: polygon(0 100%, 10% 90%, 20% 100%, 30% 90%, 40% 100%, 50% 90%, 60% 100%, 70% 90%, 80% 100%, 90% 90%, 100% 100%);
      }
      100% {
        opacity: 1;
        transform: translateY(0);
        clip-path: polygon(0 0, 100% 0, 100% 100%, 0% 100%);
      }
    }

    .wave-in { animation: waveIn 1s ease forwards; }

    body {
      font-family: Arial, sans-serif;
      margin: 0;
      padding: 0;
      background-image: url('https://images.unsplash.com/photo-1507525428034-b723cf961d3e');
      background-size: cover;
      background-position: center;
      background-attachment: fixed;
      color: white;
      overflow-x: hidden;
    }

    header {
      background-image: url('https://images.unsplash.com/photo-1501785888041-af3ef285b470');
      background-size: cover;
      background-position: center;
      padding: 60px 20px;
      text-align: center;
      color: #f7f5f5;
      position: relative;
    }

    header::before {
      content: "";
      position: absolute;
      top: 0; left: 0;
      width: 100%;
      height: 100%;
      background-color: rgba(0, 0, 0, 0.5);
      z-index: 1;
    }

    header h1, header p { position: relative; z-index: 2; }

    .menu-button {
      position: absolute;
      top: 20px;
      right: 20px;
      z-index: 3;
      font-size: 28px;
      background: none;
      border: none;
      color: white;
      cursor: pointer;
    }

    .side-menu {
      height: 100%;
      width: 0;
      position: fixed;
      top: 0; right: 0;
      background-color: rgba(77, 225, 255, 0.95);
      overflow-x: hidden;
      transition: 0.3s;
      padding-top: 60px;
      z-index: 10;
    }

    .side-menu a {
      display: block;
      padding: 14px 24px;
      text-decoration: none;
      color: white;
      font-size: 18px;
    }

    .side-menu a:hover { background-color: #69d2fecc; }

    .close-btn {
      position: absolute;
      top: 20px;
      right: 20px;
      font-size: 30px;
      cursor: pointer;
      color: white;
    }

    .slide-section {
      display: none;
      background-color: rgba(0, 0, 0, 0.5);
      margin: 20px;
      padding: 20px;
      border-radius: 10px;
    }

    .slide-section.active { display: block; }

    footer {
      background-color: #426c9fcc;
      color: white;
      text-align: center;
      padding: 10px;
    }

    /* Struktur organisasi */
    .org-chart {
      display: flex;
      flex-direction: column;
      align-items: center;
      gap: 10px;
      margin-top: 20px;
      color: white;
    }

    .org-box {
      background-color: rgba(66, 108, 159, 0.85);
      padding: 10px 15px;
      border-radius: 10px;
      min-width: 160px;
      text-align: center;
      font-weight: bold;
      box-shadow: 2px 2px 5px rgba(0,0,0,0.3);
    }

    .org-line { width: 2px; height: 20px; background-color: white; }

    .org-group {
      display: flex;
      justify-content: center;
      gap: 15px;
      flex-wrap: wrap;
    }

    .org-subgroup {
      display: flex;
      justify-content: center;
      flex-wrap: wrap;
      gap: 10px;
      margin-top: 10px;
    }

    table {
  width: 100%;
  border-collapse: collapse;
  background-color: rgba(255, 255, 255, 0.9); /* supaya teks hitam lebih jelas */
  color: black; /* semua teks tabel jadi hitam */
}

table th, table td {
  color: black; /* pastikan semua cell teks hitam */
  border: 1px solid #ccc;
  padding: 8px;
}

table thead tr {
  background-color: #2f5b8a; /* header biru */
  color: white; /* teks header tetap putih agar kontras */
}


  </style>
</head>

<body>

<!-- Tombol menu -->
<button class="menu-button" onclick="openMenu()">☰</button>

<!-- Side menu -->
<div id="sideMenu" class="side-menu">
  <span class="close-btn" onclick="closeMenu()">&times;</span>
  <a href="#" onclick="showSection('sejarah-singkat')">Sejarah Singkat</a>
  <a href="#" onclick="showSection('struktur-pemerintahan')">Struktur Pemerintahan</a>
  <a href="#" onclick="showSection('lokasi dan wilayah')">Lokasi dan wilayah</a>
  <a href="#" onclick="showSection('objek')">Objek Wisata</a>
  <a href="#" onclick="showSection('data-kampung')">Data Kampung</a>
</div>

<header>
  <h1>Selamat Datang di Kampung Inofi</h1>
  <p>Informasi  Kampung</p>
</header>

<section id="sejarah-singkat" class="slide-section active">
  <h2>Sejarah Singkat</h2>
  <p>Kampung Inofi terletak di Distrik Biak Timur...</p>
  <button onclick="toggleSlide('profil-lanjutan')">Lihat Selengkapnya</button>
  <div id="profil-lanjutan" style="display: none; margin-top: 15px;" class="wave-in">
    <h3>Sejarah Singkat Terbentuknya Kampung Inofi</h3>
    <p style="text-align: justify;">
      Kampung Inof sebelum terbentuk menjadi kampung definitif, mulanya adalah Dusun II dari Kampung Bindusi. Jadi, Inof pada awalnya adalah bagian dari Kampung Bindusi di Distrik Biak Timur, Kabupaten Biak Numfor. Pada tahun 1990 sampai 2011, jumlah penduduk Kampung Bindusi meningkat signifikan, namun pembangunan tidak dirasakan secara merata, terutama di Dusun II (Inof).
    </p>
    <p style="text-align: justify;">
      Dengan dasar tersebut, Saudara <strong>Edmon Dimara, S.Sos</strong> menggagas pemekaran kampung dan mengajak masyarakat untuk mengusulkan pemekaran kampung kepada pemerintah daerah. Masyarakat merespons positif, dan Edmon membentuk <strong>Tim Kecil</strong> bernama <em>Tim Sembilan</em> untuk mengurus pemekaran.
    </p>

    <h4 style="margin-top: 15px;">Anggota Tim Sembilan:</h4>
    <table style="black:100%; border-collapse: collapse; color: #211e1e;">
      <thead>
        <tr style="background-color: #426c9f;">
          <th style="padding: 8px; border: 1px solid #ccc;">No</th>
          <th style="padding: 8px; border: 1px solid #ccc;">Nama</th>
          <th style="padding: 8px; border: 1px solid #ccc;">Jabatan</th>
          <th style="padding: 8px; border: 1px solid #ccc;">Perwakilan</th>
        </tr>
      </thead>
      <tbody>
        <tr><td>1</td><td>Edmon Dimara, S.Sos</td><td>Ketua</td><td>-</td></tr>
        <tr><td>2</td><td>Lamek N. Inggamer</td><td>Sekretaris</td><td>-</td></tr>
        <tr><td>3</td><td>Dominggus Inggamer</td><td>Anggota</td><td>Marga Inggamer</td></tr>
        <tr><td>4</td><td>Yohanis Ronsumbre</td><td>Anggota</td><td>Marga Ronsumbre</td></tr>
        <tr><td>5</td><td>Albertus Manggombo</td><td>Anggota</td><td>Marga Manggombo</td></tr>
        <tr><td>6</td><td>Lodwik Dimara</td><td>Anggota</td><td>Marga Dimara</td></tr>
        <tr><td>7</td><td>Dance Dimara</td><td>Anggota</td><td>Tokoh Masyarakat</td></tr>
        <tr><td>8</td><td>Marthen L.S. Parorrongan</td><td>Anggota</td><td>Tokoh Agama</td></tr>
        <tr><td>9</td><td>Elisabeth Obabur</td><td>Anggota</td><td>Tokoh Perempuan</td></tr>
      </tbody>
    </table>

    <p style="text-align: justify; margin-top: 15px;">
      Tim ini mulai menyiapkan administrasi penting untuk mengusulkan pemekaran. Tahun 1997 mereka mengirim surat ke Kepala Kampung Bindusi, Bapak Matheus Kurni (alm), yang merespons positif. Kepala Kampung ikut membantu proses surat menyurat kepada pemerintah Biak Numfor.
    </p>

    <p style="text-align: justify;">
      Hasilnya, pada akhir 1998, DPRD Biak Numfor menetapkan Inof sebagai <strong>Kampung Pilot Proyek</strong>. Pada September 1999, Kepala Distrik Biak Timur <strong>Agus Filma, S.Sos</strong> meresmikan Inof sebagai kampung persiapan dan menunjuk <strong>Paulus Dimara, S.IP</strong> sebagai pelaksana tugas administratif.
    </p>

    <p style="text-align: justify;">
      Tahun 2012, Bupati Biak Numfor <strong>Yusuf Maryen</strong> menetapkan 60 kampung pemekaran termasuk Inof, dan menunjuk pejabat serta kaur pemerintahan untuk pelayanan masyarakat. Tahun 2014 kampung ini masuk dalam agenda pemilihan kepala kampung definitif, dan pada Maret 2015, <strong>Michael Ronsumbre</strong> terpilih menjadi kepala kampung pertama.
    </p>

    <p style="text-align: justify;">
      Nama awal kampung ini adalah “<strong>Inof</strong>”, namun pada surat resmi Kementerian Dalam Negeri tahun 2018, mengalami perubahan menjadi “<strong>Inofi</strong>” dengan penambahan huruf “i”.
    </p>

    <p style="text-align: center; font-style: italic; font-size: 14px; color: hsl(0, 9%, 2%); margin-top: 20px;">
      Sumber: Lamek N. Inggamer – Sekretaris Tim IX<br>
    </p>
  </div>
</section>

<section id="struktur-pemerintahan" class="slide-section">
  <h2>Struktur Pemerintahan</h2>
  <ul>
    <li>Pj Kepala Kampung:Markus yarangga S.IP </li>
    <li>Sekretaris: Lamek N. Inggamer</li>
  </ul>
  <button onclick="toggleSlide('struktur-lanjutan')">Lihat Selengkapnya</button>

  <div id="struktur-lanjutan" style="display: none; margin-top: 15px;" class="wave-in">
    <h3 style="text-align:center;">Struktur Pemerintahan Kampung Inofi</h3>

    <div class="org-chart">
      <!-- Kepala Distrik -->
      <div class="org-box">Kepala Distrik</div>
      <div class="org-line"></div>

      <!-- Kepala Kampung dan Bamuskam sejajar -->
      <div style="display: flex; flex-direction: column; align-items: center;">
        <!-- Garis vertikal dari Kepala Distrik -->
        <div class="org-line"></div>
        <!-- Kotak sejajar + garis horizontal -->
        <div style="display: flex; align-items: center; justify-content: center;">
          <div class="org-box">Bamuskam</div>
          <div style="width: 40px; height: 2px; background-color: white;"></div>
          <div class="org-box">Kepala kampung</div>
        </div>
      </div>

      <!-- Garis ke Sekretaris -->
      <div class="org-line"></div>
      <div class="org-box">Sekretaris</div>
      <div class="org-line"></div>

      <!-- Garis ke Kaur -->
      <div class="org-line"></div>
      <div style="display: flex; flex-direction: column; align-items: center;">
        <div class="org-line"></div>
        <div style="display: flex; align-items: center; justify-content: center; flex-wrap: wrap; gap: 15px;">
          <div class="org-box">Kaur. Kesra</div>
          <div class="org-box">Kaur. Administrasi</div>
          <div class="org-box">Kaur. Keuangan</div>
          <div class="org-box">Kaur. Umum</div>
          <div class="org-box">Kaur. Pembangunan</div>
          <div class="org-box">Kaur. Pemerintah</div>
        </div>
      </div>

      <!-- Garis ke RW -->
      <div class="org-line"></div>
      <div style="display: flex; flex-direction: column; align-items: center;">
        <div class="org-line"></div>
        <div style="display: flex; align-items: center; justify-content: center; gap: 15px;">
          <div class="org-box">Ketua RW 01</div>
          <div class="org-box">Ketua RW 02</div>
        </div>
      </div>

      <!-- Garis ke RT -->
      <div class="org-line"></div>
      <div style="display: flex; flex-direction: column; align-items: center;">
        <div class="org-line"></div>
        <div style="display: flex; align-items: center; justify-content: center; gap: 10px; flex-wrap: wrap;">
          <div class="org-box">Ketua RT 01</div>
          <div class="org-box">Ketua RT 02</div>
          <div class="org-box">Ketua RT 03</div>
          <div class="org-box">Ketua RT 04</div>
        </div>
      </div>

    </div>

    <p style="font-style: italic; font-size: 14px; color: #ccc; text-align: center; margin-top: 15px;">
      *Struktur ini berdasarkan dokumen resmi Pemerintahan Kampung Inofi.
    </p>
  </div>
</section>

<section id="lokasi dan wilayah" class="slide-section">
  <h2>Lokasi dan Wilayah</h2>
  <p>Kampung Inofi terletak di distrik biak timur kabupaten biak numfor, dibagian timur berbatasan dengan kampung soryar,
     di bagian barat berbatasan dengan kampung bindusi, di bagian utara berbatasan dengan laut dan sebelah selatan berbatasan dengan kampung insumarires.
</p>

  <div class="lokasi-wilayah-container">
    <!-- Peta Batas Wilayah -->
    <div class="lokasi-wilayah">
      <img src="peta_batas_wilayah.jpg" alt="Batas Kampung Inofi" class="wave-in">
      <p>Ikon batas wilayah Kampung Inofi.</p>
    </div>

    <!-- Peta Administrasi -->
    <div class="lokasi-wilayah">
      <img src="peta_administrasi.jpg" alt="Peta Administrasi Kampung Inofi" class="wave-in">
      <p>Peta Administrasi Kampung Inofi (Distrik Biak Timur).</p>
    </div>
  </div>
</section>

<style>
  .lokasi-wilayah-container {
    display: flex;
    gap: 20px;
    justify-content: center;
    flex-wrap: wrap; /* biar rapi di layar kecil */
  }
  .lokasi-wilayah {
    flex: 1 1 400px;
    text-align: center;
    background-color: rgba(0,0,0,0.4);
    padding: 15px;
    border-radius: 10px;
  }
  .lokasi-wilayah img {
    max-width: 100%;
    border-radius: 10px;
    box-shadow: 0 2px 6px rgba(0,0,0,0.5);
    display: block;
    margin: 0 auto 10px;
  }
</style>
<section id="objek" class="slide-section">
  <h2>Objek Wisata</h2>
  <ul class="objek-wisata">
    <li>
      <figure style="margin:0;">
        <img src="segara_indah.webp" alt="Pantai" style="width: 4in; height: 4in; border-radius: 10px;">
        <figcaption style="color: white; margin-top: 8px;">Pemandangan pantai Segara Indah</figcaption>
      </figure>
    </li>
    <li>
      <figure style="margin:0;">
        <img src="tugu_karang.jpg" alt="Tugu Terumbu Karang" style="width: 4in; height: 4in; border-radius: 10px;">
        <figcaption style="color: rgb(255, 255, 255); margin-top: 8px;">TUGU TERUMBU KARANG</figcaption>
      </figure>
    </li>
  </ul>
</section>

<style>
  .objek-wisata {
    list-style: none;
    display: flex;
    gap: 20px; /* jarak antar gambar */
    flex-wrap: wrap; /* supaya tetap rapi di layar kecil */
    padding: 0;
    justify-content: center; /* posisi rata tengah */
  }

  .objek-wisata li {
    background-color: rgba(0,0,0,0.4);
    padding: 10px;
    border-radius: 10px;
    text-align: center;
    flex: 1 1 300px; /* agar responsif */
    max-width: 420px; /* batasi ukuran maksimal */
  }

  .objek-wisata img {
    width: 100%;
    height: auto;
    border-radius: 10px;
  }
</style>



<section id="data-kampung" class="slide-section">

  <h2>Data Kampung Inofi</h2>
  <table style="width:100%; border-collapse: collapse; background-color: rgba(66, 108, 159, 0.8); color: hsl(0, 3%, 6%);">
    <thead>
      <tr style="background-color: #2f5b8a;">
        <th style="padding: 8px; border: 1px solid #ccc;">No</th>
        <th style="padding: 8px; border: 1px solid #ccc;">Data</th>
        <th style="padding: 8px; border: 1px solid #ccc;">Keterangan</th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <td style="padding: 8px; border: 1px solid #ccc;">1</td>
        <td style="padding: 8px; border: 1px solid #ccc;">Nama Kampung</td>
        <td style="padding: 8px; border: 1px solid #ccc;">Inofi</td>
      </tr>
      <tr>
        <td style="padding: 8px; border: 1px solid #ccc;">2</td>
        <td style="padding: 8px; border: 1px solid #ccc;">Distrik</td>
        <td style="padding: 8px; border: 1px solid #ccc;">Biak Timur</td>
      </tr>
      <tr>
        <td style="padding: 8px; border: 1px solid #ccc;">3</td>
        <td style="padding: 8px; border: 1px solid #ccc;">Kabupaten</td>
        <td style="padding: 8px; border: 1px solid #ccc;">Biak Numfor</td>
      </tr>
      <tr>
        <td style="padding: 8px; border: 1px solid #ccc;">4</td>
        <td style="padding: 8px; border: 1px solid #ccc;">Provinsi</td>
        <td style="padding: 8px; border: 1px solid #ccc;">Papua</td>
      </tr>
      <tr>
        <td style="padding: 8px; border: 1px solid #ccc;">5</td>
        <td style="padding: 8px; border: 1px solid #ccc;">Jumlah Penduduk</td>
        <td style="padding: 8px; border: 1px solid #ccc;">± 243</td>
      </tr>
      <tr>
        <td style="padding: 8px; border: 1px solid #ccc;">6</td>
        <td style="padding: 8px; border: 1px solid #ccc;">Luas Wilayah</td>
        <td style="padding: 8px; border: 1px solid #ccc;">± 1.125.000 km²</td>
      </tr>
      <tr>
        <td style="padding: 8px; border: 1px solid #ccc;">7</td>
        <td style="padding: 8px; border: 1px solid #ccc;">Mata Pencaharian</td>
        <td style="padding: 8px; border: 1px solid #ccc;">Nelayan, Petani, Pedagang</td>
      </tr>
    </tbody>
  </table>

  <p style="text-align:center; font-style: italic; color: #ccc; margin-top: 10px;">
    *Data ini bersifat sementara dan dapat berubah sesuai perkembangan kampung.
  </p>
</section>

<footer>
  <p>&copy; KAMPUNG INOFI 2025</p>
</footer>

<script>
  function toggleSlide(id) {
    var slide = document.getElementById(id);
    if (!slide) return;
    if (slide.style.display === "none") {
      slide.style.display = "block";
      slide.classList.remove("wave-in");
      void slide.offsetWidth;
      slide.classList.add("wave-in");
    } else {
      slide.style.display = "none";
    }
  }

  function openMenu() { document.getElementById("sideMenu").style.width = "250px"; }
  function closeMenu() { document.getElementById("sideMenu").style.width = "0"; }

  function showSection(id) {
    var sections = document.querySelectorAll('.slide-section');
    sections.forEach(function(sec) { sec.classList.remove('active'); });

    var activeSection = document.getElementById(id);
    if (activeSection) {
      activeSection.classList.add('active');
      activeSection.classList.remove("wave-in");
      void activeSection.offsetWidth;
      activeSection.classList.add("wave-in");
    }
    closeMenu();
  }
</script>

</body>
</html>
