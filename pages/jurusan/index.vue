<template>
  <div id="jurusan" class="container mt-5">
    <div class="row">
      <div class="col text-center">
        <h2 class="fw-bold">Jurusan</h2>
        <p class="text-muted">"SMKN 4 Tasikmalaya menyediakan berbagai jurusan yang menarik dan berkualitas."</p>
      </div>
    </div>

    <!-- Row Card Jurusan -->
    <div class="row mt-4">
      <!-- Card TKJ -->
      <div class="col-lg-4 col-md-6 mb-4">
        <div class="shadow card h-100 card-hover">
          <div class="card-body text-center bg-primary" style="color: white;">
            <img src="~/assets/img/tkj.png" alt="Logo Sekolah" width="40" height="45" class="me-2">
            <h5 class="card-title">Teknik Komputer dan Jaringan (TKJ)</h5>
            <p class="card-text">Teknik Komputer dan Jaringan (TKJ) adalah salah satu jurusan di bidang keahlian teknik yang fokus pada pengembangan, pemeliharaan, dan pengelolaan sistem komputer serta jaringan komputer. Jurusan ini sangat relevan dengan kebutuhan dunia kerja saat ini, terutama dengan pesatnya perkembangan teknologi informasi dan komunikasi (TIK). Lulusan dari jurusan TKJ diharapkan mampu mengatasi berbagai masalah terkait perangkat keras (hardware), perangkat lunak (software), serta pengaturan dan pemeliharaan jaringan komputer.

</p>
          </div>
        </div>
      </div>

      <!-- Card RPL -->
      <div class="col-lg-4 col-md-6 mb-4">
        <div class="shadow card h-100 card-hover">
          <div class="card-body text-center bg-success" style="color: white;">
            <img src="~/assets/img/rpl.png" alt="Logo Sekolah" width="40" height="45" class="me-2">
            <h5 class="card-title">Rekayasa Perangkat Lunak (RPL)</h5>
            <p class="card-text">Rekayasa Perangkat Lunak (RPL) adalah salah satu jurusan di bidang teknologi informasi yang fokus pada pembuatan, pengembangan, dan pemeliharaan perangkat lunak (software). Jurusan ini mempersiapkan siswa untuk bekerja dalam industri teknologi dengan menguasai berbagai keterampilan dalam pembuatan aplikasi komputer, desain sistem, pengujian perangkat lunak, dan pengelolaan proyek perangkat lunak.

</p>
          </div>
        </div>
      </div>

      <!-- Card DKV -->
      <div class="col-lg-4 col-md-6 mb-4">
        <div class="shadow card h-100 card-hover">
          <div class="card-body text-center bg-warning" style="color: white;">
            <img src="~/assets/img/dkv.png" alt="Logo Sekolah" width="40" height="45" class="me-2">
            <h5 class="card-title">Desain Komunikasi Visual (DKV)</h5>
            <p class="card-text">Desain Komunikasi Visual (DKV) adalah jurusan yang fokus pada pengembangan kemampuan untuk mengkomunikasikan pesan atau ide melalui elemen visual, seperti gambar, tipografi, warna, dan media digital. Jurusan ini memadukan kreativitas, seni, dan teknologi untuk menciptakan desain yang dapat menyampaikan pesan secara efektif kepada audiens.

</p>
          </div>
        </div>
      </div>

      <!-- Card TBSM -->
      <div class="col-lg-6 col-md-6 mb-4">
        <div class="shadow card h-100 card-hover">
          <div class="card-body text-center bg-danger" style="color: white;">
            <img src="~/assets/img/tsm.png" alt="Logo Sekolah" width="40" height="45" class="me-2">
            <h5 class="card-title">Teknik Bisnis Sepeda Motor (TBSM)</h5>
            <p class="card-text">Jurusan TBSM (Teknik Bisnis Sepeda Motor) adalah salah satu jurusan yang ada di SMK (Sekolah Menengah Kejuruan) yang fokus pada bidang teknologi dan keterampilan dalam perawatan dan perbaikan sepeda motor. Jurusan ini cocok bagi siswa yang memiliki minat di dunia otomotif, terutama yang berhubungan dengan sepeda motor.

</p>
          </div>
        </div>
      </div>

      <!-- Card TOI -->
      <div class="col-lg-6 col-md-6 mb-4">
        <div class="shadow card h-100 card-hover">
          <div class="card-body text-center bg-secondary" style="color: white;">
            <img src="~/assets/img/toi.png" alt="Logo Sekolah" width="40" height="45" class="me-2">
            <h5 class="card-title">Teknik Otomasi Industri (TOI)</h5>
            <p class="card-text">Jurusan TOI (Teknik Otomotif Industri) adalah salah satu jurusan yang ada di SMK (Sekolah Menengah Kejuruan) yang fokus pada bidang teknik otomotif, dengan penekanan pada industri otomotif secara umum. Jurusan ini lebih mengarah pada penerapan teknologi otomotif dalam dunia industri, termasuk dalam perawatan, perbaikan, dan inovasi sistem kendaraan bermotor yang digunakan dalam berbagai sektor industri.

</p>
          </div>
        </div>
      </div>
    </div>
  </div>
  <!-- Footer Section -->
  <footer class="bg-dark text-white text-center py-4">
      <p>&copy; 2024 SMKN 4 Tasikmalaya | Semua Hak Cipta Dilindungi</p>
    </footer>
</template>

<script>
export default {
  data() {
    return {
      jurusan: [
        { name: "Teknik Komputer dan Jaringan (TKJ)", description: "Mahir dalam jaringan komputer dan teknologi informasi.", students: 120 },
        { name: "Rekayasa Perangkat Lunak (RPL)", description: "Ahli dalam pengembangan perangkat lunak modern.", students: 100 },
        { name: "Desain Komunikasi Visual (DKV)", description: "Kreatif dalam seni desain dan komunikasi visual.", students: 90 },
        { name: "Teknik Bisnis Sepeda Motor (TBSM)", description: "Ahli dalam perbaikan dan manajemen bisnis sepeda motor.", students: 80 },
        { name: "Teknik Otomasi Industri (TOI)", description: "Mahir dalam sistem otomatisasi dan teknologi industri.", students: 70 }
      ]
    };
  }
};
</script>

<style scoped>
/* General Card Styles */
.card {
  border-radius: 15px;
  transition: transform 0.3s ease-in-out;
  cursor: pointer;
}
.card:hover {
  transform: translateY(-10px);
  box-shadow: 0 10px 30px rgba(0, 0, 0, 0.1);
}

/* Text Styling */
.card-title {
  font-weight: bold;
  font-size: 1.2rem;
}

.card-text {
  font-size: 1rem;
  line-height: 1.5;
}

/* Background Colors */
.bg-primary {
  background-color: #007bff !important;
}
.bg-success {
  background-color: #28a745 !important;
}
.bg-warning {
  background-color: #ffc107 !important;
}
.bg-danger {
  background-color: #dc3545 !important;
}
.bg-secondary {
  background-color: #6c757d !important;
}

/* Spacing */
.container {
  padding-left: 15px;
  padding-right: 15px;
}

.card-body {
  padding: 20px;
}

/* Responsive Design */
@media (max-width: 768px) {
  .card-title {
    font-size: 1.1rem;
  }

  .card-text {
    font-size: 0.9rem;
  }
}
</style>
