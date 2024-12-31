<template>
    <div class="container mt-4">
      <!-- Konten Profil Sekolah -->
      <div class="d-flex align-items-center flex-wrap mb-4">
      <!-- Kolom Gambar Logo -->
        <div class="p-2 flex-fill text-center logo-container">
        </div>
      </div>
  
      <!-- Tabel Visi dan Misi Sekolah -->
      <div class="mt-4">
        <h3>Visi dan Misi</h3>
  
        <!-- Tabel Visi -->
        <table class="table table-bordered shadow-sm mb-4">
          <tbody>
            <tr>
              <th scope="row">Visi</th>
              <td>
                "TERWUJUDNYA LULUSAN YANG CERDAS, AKTIF, KOMPETITIF, ADAPTIF, DAN PRODUKTIF BERLANDASKAN IMAN DAN TAKWA
                (CAKAP BERIMTAK)"
              </td>
            </tr>
            <tr>
              <th scope="row">Misi 1</th>
              <td>
                • Menyiapkan Sumber Daya Manusia yang cerdas dan kompeten baik hardskill maupun softskill.<br />
                • Meningkatkan dan mengembangkan aktifitas serta kreatifitas seluruh warga sekolah dalam berbagai kegiatan
                positif.<br />
                • Mewujudkan manajemen pengelolaan yang efektif, efisien, transparan, akuntabel dan layanan prima.<br />
                • Menumbuhkan dan mengembangkan potensi dan kemampuan Sumber Daya Manusia yang berdaya saing tinggi melalui
                berbagai kegiatan akademik maupun non akademik.<br />
                • Menyelenggarakan berbagai program kegiatan dalam upaya meningkatkan Sumber Daya Manusia yang mampu
                menyesuaikan dengan perkembangan.<br />
                • Mengembangkan sarana prasarana dan lingkungan sekolah yang menyenangkan sebagai wadah menumbuhkembangkan daya
                kreasi dan inovasi untuk menghasilkan produk teknologi tepat guna.<br />
                • Membangun jiwa wirausaha yang handal melalui pembelajaran Teaching Factory (TEFA) dan Kelas Industri.<br />
                • Menjalin dan mengembangkan kemitraan dengan Industri dan Dunia Kerja (IDUKA) serta lembaga lainnya yang
                relevan.<br />
                • Menanamkan dan membudayakan sikap dan perilaku yang baik pada aktivitas di sekolah maupun dalam kehidupan
                sehari-hari.
              </td>
            </tr>
          </tbody>
        </table>
      </div>
  
      <!-- Sejarah Sekolah -->
      <h3>Sejarah</h3>
      <p>
        Sejalan dengan Program Pemerintah dibidang pendidikan Menengah Kejuruan pada saat itu yakni pemerataan akses ditambah
        pula dengan banyaknya keinginan masyarakat yang mengharapkan adanya SMK Negeri di daerah Kecamatan Purbaratu Kota
        Tasikmalaya, terutama untuk menampung tamatan dari SLTP yang ingin melanjutkan ke SMK maka beberapa tokoh masyarakat,
        unsur pejabat pemerintah di Kecamatan Purbaratu Kota Tasikmalaya mengusulkan kepada pemerintah Kota Tasikmalaya dan
        Pemerintah Provinsi Jawa Barat, agar berdirinya SMK Negeri di Kecamatan Purbaratu Kota Tasikmalaya.
        Setelah melalui perjuangan yang sangat panjang dari berbagai pihak khususnya Disdik Kota Tasikmalaya dan
        pihak-pihak terkait lainnya sesuai prosedur dan ketentuan yang berlaku pada waktu itu dengan mengucapkan syukur
        Alhamdulillah akhirnya pada tahun pelajaran 2010/2011 SMK Negeri 4 Tasikmalaya mulai berdiri, pada awalnya membuka
        Kompetensi Keahlian Teknik Komputer dan Jaringan dengan pendaftar peserta Didik Baru pada waktu itu berjumlah 44 orang.
        Pada awalnya tempat belajar menumpang di SMP Negeri 17 Kota Tasikmalaya, dan sekolah induknya adalah SMK Negeri 2 Kota
        Tasikmalaya, Untuk Tenaga pendidik dan Tenaga Kependidikan masih dibantu sepenuhnya oleh kedua sekolah tersebut.
        Pada tahun 2012 keluarlah surat Izin Pendirian berdasarkan keputusan kepala Badan Pelayanan Perizinan Terpadu Kota
        Tasikmalaya No. 420/9/SK-BPPT/2012 Tanggal 06 Februari 2012.
      </p>
    </div>
    <div>
    <!-- Konten Data -->
    <div id="data" class="container mt-3">
      <div class="row">
        <div class="col">
          <h2 class="display-4 text-drak font-weight-bold">Data Sekolah</h2>
          <p class="lead text-muted">Informasi jumlah guru, staf, dan murid di SMKN 4 Tasikmalaya.</p>
        </div>
      </div>

      <!-- Tabel Jumlah Guru, Staf, dan Pegawai -->
      <div class="row mt-4">
        <div class="col-lg-6 mb-4">
          <h3 class="text-drak">Jumlah Guru dan Staf</h3>
          <table class="table table-striped table-hover shadow-lg rounded">
            <thead class="thead-dark">
              <tr>
                <th>Kategori</th>
                <th>Jumlah</th>
              </tr>
            </thead>
            <tbody>
              <tr>
                <td>Guru</td>
                <td>{{ jumlahGuru }}</td>
              </tr>
              <tr>
                <td>Staf Administrasi</td>
                <td>{{ jumlahStafAdministrasi }}</td>
              </tr>
              <tr>
                <td>Pegawai Lainnya</td>
                <td>{{ jumlahPegawaiLainnya }}</td>
              </tr>
            </tbody>
          </table>
        </div>
      </div>

      <!-- Tabel Jumlah Murid Per Jurusan -->
      <div class="row mt-4">
        <div class="col">
          <h3 class="text-drak">Jumlah Murid Per Jurusan</h3>
          <table class="table table-bordered table-striped table-hover shadow-lg rounded">
            <thead class="thead-dark">
              <tr>
                <th>Jurusan</th>
                <th>Jumlah Murid</th>
              </tr>
            </thead>
            <tbody>
              <tr v-for="(jumlah, jurusan) in jumlahMuridPerJurusan" :key="jurusan">
                <td>{{ jurusan }}</td>
                <td>{{ jumlah }}</td>
              </tr>
            </tbody>
          </table>
        </div>
      </div>
    </div>
  </div>
  </template>
  
  <script>
    export default {
      name: 'ProfilPage',
        data() {
      return {
        // Data jumlah guru, staf, dan pegawai
        jumlahGuru: 50,
        jumlahStafAdministrasi: 15,
        jumlahPegawaiLainnya: 10,
  
        // Data jumlah murid per jurusan
        jumlahMuridPerJurusan: {
          "TEKNIK KOMPUTER JARINGAN": 120,
          "REKAYASA PERANGKAT LUNAK": 100,
          "TEKNIK BISNIS DAN SEPEDA MOTOR": 80,
          "TEKNIK OTOMASI INDUSTRI": 90,
  
        }
      }
    }
  }
  </script>
  
  <style scoped>
    h2, h3, h4 {
      margin-bottom: 20px;
      color: #2c3e50;
    }
  
    table {
      width: 100%;
      border-collapse: collapse;
    }
  
    th, td {
      text-align: left;
      vertical-align: middle;
      padding: 12px;
    }
  
    th {
      width: 25%;
      background-color: #f8f9fa;
      font-weight: bold;
      color: #495057;
    }
  
    td {
      background-color: #ffffff;
    }
  
    table tbody tr:hover {
      background-color: #f1f1f1;
    }
  
    .container {
      background-color: #f4f6f9;
      padding: 30px;
      border-radius: 8px;
    }
  
    .d-flex {
      gap: 20px;
    }
  
    .p-2 {
      padding: 10px;
    }
  
    .shadow-sm {
      box-shadow: 0 2px 8px rgba(0, 0, 0, 0.1);
    }
  
    .img-fluid {
      max-width: 100%;
      height: auto;
    }
  
    .text-center {
      display: flex;
      justify-content: center;
      align-items: center;
      max-width: 200px;
      margin: 0 auto;
    }
  
    .logo-container img {
      max-width: 150px;
      height: auto;
    }
  
    /* Responsiveness */
    @media (max-width: 768px) {
      .d-flex {
        flex-direction: column;
        align-items: center;
      }
  
      .p-2 {
        width: 100%;
      }
  
      h2 {
        font-size: 1.5rem;
      }
  
      .logo-container img {
        max-width: 120px;
      }
    }
/* Menambahkan beberapa styling untuk mempercantik tampilan */
.container {
  font-family: 'Roboto', sans-serif;
}

h2 {
  font-weight: 700;
}

table {
  border-collapse: collapse;
}

thead {
  background-color: #343a40;
  color: white;
}

th, td {
  padding: 10px;
  text-align: center;
}

.table-hover tbody tr:hover {
  background-color: #f8f9fa;
}

.shadow-lg {
  box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1);
}

.rounded {
  border-radius: 8px;
}

.text-muted {
  color: #6c757d;
}

.text-success {
  color: #28a745;
}

.text-info {
  color: #17a2b8;
}

.lead {
  font-size: 1.25rem;
  font-weight: 300;
}
</style>
  