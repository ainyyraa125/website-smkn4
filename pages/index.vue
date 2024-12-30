<template>
  <!-- Logo Section -->
  <div class="text-center mt-4">
    <img src="~/assets/img/home.jpg" alt="Logo SMKN 4 Tasikmalaya" class="img-fluid" />
  </div>

  <!-- Sambutan Kepala Sekolah Section -->
  <h2 class="bg-secondary text-white text-center py-3 mt-5 mb-4 rounded-3">SAMBUTAN KEPALA SEKOLAH</h2>
  <div class="d-flex align-items-center justify-content-center mt-4 shadow-sm rounded-lg" style="background-color: #f5f5f5; padding: 20px;">
    <img src="~/assets/img/kepsek.png" alt="Kepala Sekolah" class="rounded-circle border border-4 border-primary" style="width: 150px; height: 150px;"/>
    <div class="ms-4">
      <h3 class="text-dark fw-bold">Sambutan Kepala Sekolah</h3>
      <p class="text-muted">Selamat datang di situs resmi SMKN 4 Tasikmalaya. Kami berkomitmen untuk memberikan pendidikan terbaik bagi generasi muda, dengan fokus pada kompetensi di bidang Teknologi dan Komunikasi. Terima kasih telah mengunjungi kami!</p>
      <small class="text-muted">Kepala Sekolah, SMKN 4 Tasikmalaya</small>
    </div>
  </div>

  <!-- BERITA Section -->
  <h2 class="bg-secondary text-white text-center py-3 mt-5 rounded-3">BERITA</h2>
  <div class="card-group mt-4">
    <div class="card shadow-sm rounded-lg mx-2">
      <img src="~/assets/img/expo.webp" class="card-img-top" alt="Expo" />
      <div class="card-body">
        <h5 class="card-title text-dark">EXPO</h5>
        <p class="card-text">Latest update on our school expo.</p>
        <small class="text-muted">Last updated 3 mins ago</small>
      </div>
    </div>
    <div class="card shadow-sm rounded-lg mx-2">
      <img src="~/assets/img/expo.webp" class="card-img-top" alt="Expo" />
      <div class="card-body">
        <h5 class="card-title text-dark">EXPO</h5>
        <p class="card-text">Details about our upcoming event.</p>
        <small class="text-muted">Last updated 3 mins ago</small>
      </div>
    </div>
    <div class="card shadow-sm rounded-lg mx-2">
      <img src="~/assets/img/expo.webp" class="card-img-top" alt="Expo" />
      <div class="card-body">
        <h5 class="card-title text-dark">EXPO</h5>
        <p class="card-text">Highlights from the recent event.</p>
        <small class="text-muted">Last updated 3 mins ago</small>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'HomePage'
}
</script>

<style scoped>
/* Global Styling */
h3 {
  font-size: 1.75rem;
  font-weight: 600;
  color: #000000;
  margin-bottom: 1.25rem;
}

.card-group .card {
  margin: 0 10px;
}

.card-img-top {
  object-fit: cover;
  height: 200px;
  border-bottom: 4px solid #000000;
}

.bg-primary {
  background-color: #000000 !important;
}

.text-center {
  text-align: center;
}

.ms-4 {
  margin-left: 1.5rem;
}

.text-muted {
  font-size: 0.875rem;
}

.card-body p {
  font-size: 1rem;
  color: #333;
}

.card-body h5 {
  font-size: 1.25rem;
  font-weight: bold;
  color: #000000;
}

.card-body small {
  font-size: 0.875rem;
  color: #777;
}

.bg-secondary {
  background-color: #6c757d;
}

/* Improve the logo section */
.img-fluid {
  max-width: 100%;
  height: auto;
}

/* Sambutan Kepala Sekolah Section */
.shadow-sm {
  box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
}

.rounded-lg {
  border-radius: 10px;
}

.border-primary {
  border-color: #007bff;
}

/* News Section */
.card-title {
  font-weight: bold;
  color: #000;
}

.card-body .card-text {
  font-size: 1rem;
  color: #333;
}

.card-group .card {
  transition: transform 0.3s ease-in-out;
}

.card-group .card:hover {
  transform: translateY(-5px);
}

.card-body small {
  font-size: 0.875rem;
  color: #777;
}

/* Media Queries for responsiveness */
@media (max-width: 768px) {
  .d-flex {
    flex-direction: column;
    align-items: center;
  }

  .ms-4 {
    margin-left: 0;
  }

  .card-group {
    flex-direction: column;
  }

  .card {
    margin-bottom: 1rem;
  }

  .card-img-top {
    height: 180px;
  }

  h3 {
    font-size: 1.5rem;
  }

  .text-center h2 {
    font-size: 1.5rem;
  }
}
</style>
