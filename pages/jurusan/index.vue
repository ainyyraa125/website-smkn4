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
            <p class="card-text">Mahir dalam jaringan komputer dan teknologi informasi.</p>
            <p class="card-text"><strong>Jumlah Murid: 120</strong></p>
          </div>
        </div>
      </div>

      <!-- Card RPL -->
      <div class="col-lg-4 col-md-6 mb-4">
        <div class="shadow card h-100 card-hover">
          <div class="card-body text-center bg-success" style="color: white;">
            <img src="~/assets/img/rpl.png" alt="Logo Sekolah" width="40" height="45" class="me-2">
            <h5 class="card-title">Rekayasa Perangkat Lunak (RPL)</h5>
            <p class="card-text">Ahli dalam pengembangan perangkat lunak modern.</p>
            <p class="card-text"><strong>Jumlah Murid: 100</strong></p>
          </div>
        </div>
      </div>

      <!-- Card DKV -->
      <div class="col-lg-4 col-md-6 mb-4">
        <div class="shadow card h-100 card-hover">
          <div class="card-body text-center bg-warning" style="color: white;">
            <img src="~/assets/img/dkv.png" alt="Logo Sekolah" width="40" height="45" class="me-2">
            <h5 class="card-title">Desain Komunikasi Visual (DKV)</h5>
            <p class="card-text">Kreatif dalam seni desain dan komunikasi visual.</p>
            <p class="card-text"><strong>Jumlah Murid: 90</strong></p>
          </div>
        </div>
      </div>

      <!-- Card TBSM -->
      <div class="col-lg-6 col-md-6 mb-4">
        <div class="shadow card h-100 card-hover">
          <div class="card-body text-center bg-danger" style="color: white;">
            <img src="~/assets/img/tsm.png" alt="Logo Sekolah" width="40" height="45" class="me-2">
            <h5 class="card-title">Teknik Bisnis Sepeda Motor (TBSM)</h5>
            <p class="card-text">Ahli dalam perbaikan dan manajemen bisnis sepeda motor.</p>
            <p class="card-text"><strong>Jumlah Murid: 80</strong></p>
          </div>
        </div>
      </div>

      <!-- Card TOI -->
      <div class="col-lg-6 col-md-6 mb-4">
        <div class="shadow card h-100 card-hover">
          <div class="card-body text-center bg-secondary" style="color: white;">
            <img src="~/assets/img/toi.png" alt="Logo Sekolah" width="40" height="45" class="me-2">
            <h5 class="card-title">Teknik Otomasi Industri (TOI)</h5>
            <p class="card-text">Mahir dalam sistem otomatisasi dan teknologi industri.</p>
            <p class="card-text"><strong>Jumlah Murid: 70</strong></p>
          </div>
        </div>
      </div>
    </div>
  </div>
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
