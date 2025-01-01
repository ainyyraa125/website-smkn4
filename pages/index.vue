<template>
  <div>
    <!-- Hero Section -->
    <section class="hero-section text-center text-white py-5">
      <div class="container">
        <h1 class="display-4 mb-4">Selamat Datang di SMKN 4 Tasikmalaya</h1>
        <p class="lead mb-4">Temukan informasi terbaru mengenai kegiatan, prestasi, dan program unggulan kami</p>
      </div>
    </section>

    <!-- Gambar di atas Sambutan Kepala Sekolah -->
    <section class="header-image-section">
      <img src="~/assets/img/home.jpg" alt="Selamat Datang Di Website SMKN 4" class="img-fluid w-100" />
    </section>

    <!-- Sambutan Kepala Sekolah -->
    <section class="sambutan-section py-5" id="sambutan">
      <div class="container text-center">
        <h2 class="mb-4">Sambutan Kepala Sekolah</h2>
        <div class="row align-items-center">
          <div class="col-md-4">
            <img src="~/assets/img/kepsek.png" alt="Kepala Sekolah" class="img-fluid rounded-circle" />
          </div>
          <div class="col-md-8">
            <p class="lead">Assalamualaikum warahmatullahi wabarakatuh,
Salam sejahtera bagi kita semua,Selamat datang di website SMKN 4 Tasikmalaya,
Alhamdulillah, puji syukur kita panjatkan kepada Tuhan Yang Maha Esa, karena berkat rahmat dan karunia-Nya, kita diberikan kesempatan untuk terus berkembang dalam dunia pendidikan. Website ini kami hadirkan sebagai sarana komunikasi dan informasi yang dapat mempermudah hubungan antara sekolah, siswa, orang tua, dan masyarakat luas.Di SMKN 4 Tasikmalaya, kami percaya bahwa pendidikan adalah investasi terbaik bagi masa depan bangsa. Oleh karena itu, kami selalu berkomitmen untuk memberikan layanan pendidikan yang berkualitas, mencetak generasi yang cerdas, berkarakter, serta siap menghadapi tantangan global.Kami juga sangat menghargai peran serta orang tua dan masyarakat dalam mendukung kemajuan sekolah ini. Semoga melalui informasi yang ada di website ini, kita dapat mempererat kerja sama yang telah terjalin dan membangun lingkungan belajar yang lebih baik.Terima kasih atas perhatian dan kepercayaan yang diberikan kepada kami. Semoga SMKN 4 Tasikmalaya dapat terus memberikan kontribusi terbaik untuk pendidikan dan kemajuan anak bangsa.Wassalamualaikum warahmatullahi wabarakatuh.</p>
            <p><small class="text-muted">Kepala Sekolah, SMKN 4 Tasikmalaya</small></p>
          </div>
        </div>
      </div>
    </section>

    <!-- Berita Terbaru -->
    <section class="berita-section py-5" id="berita">
      <div class="container text-center">
        <h2 class="mb-4">Berita Terbaru</h2>
        <div class="row">
          <div class="col-md-4 mb-4">
            <div class="card">
              <img src="~/assets/img/expo.webp" class="card-img-top" alt="Expo" />
              <div class="card-body">
                <h5 class="card-title">Expo Sekolah</h5>
                <p class="card-text">Expo sebuah acara yang penuh dengan kreativitas, inovasi, dan prestasi. Di sini, para siswa menunjukkan hasil karya mereka dalam berbagai bidang, mulai dari seni, teknologi, hingga ilmu pengetahuan. Expo ini merupakan wujud nyata dari proses pembelajaran yang mereka jalani, serta bukti komitmen kami dalam mencetak generasi yang siap bersaing di dunia global.

</p>
              </div>
            </div>
          </div>
          <div class="col-md-4 mb-4">
            <div class="card">
              <img src="~/assets/img/fair.jpg" class="card-img-top" alt="Job Fair" />
              <div class="card-body">
                <h5 class="card-title">Job Fair</h5>
                <p class="card-text">Acara ini merupakan kesempatan luar biasa bagi para siswa, alumni, dan pencari kerja untuk bertemu langsung dengan berbagai perusahaan terkemuka yang membuka peluang karier menarik.</p>
              </div>
            </div>
          </div>
          <div class="col-md-4 mb-4">
            <div class="card">
              <img src="~/assets/img/binsik.jpg" class="card-img-top" alt="Binsik" />
              <div class="card-body">
                <h5 class="card-title">Binsik</h5>
                <p class="card-text">Binsik adalah program yang dirancang untuk membantu siswa dalam mengembangkan potensi diri, mengatasi tantangan pribadi, serta merencanakan masa depan yang lebih baik.Acara ini bertujuan untuk memberikan dukungan emosional, psikologis, dan sosial bagi para siswa agar dapat menjalani kehidupan sekolah dengan lebih percaya diri dan seimbang.</p>
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>

    <!-- Footer Section -->
    <footer class="bg-dark text-white text-center py-4">
      <p>&copy; 2024 SMKN 4 Tasikmalaya | Semua Hak Cipta Dilindungi</p>
    </footer>
  </div>
</template>

<script>
export default {
  name: 'HomePage'
}
</script>

<style scoped>
/* Global Styles */
body {
  font-family: 'Arial', sans-serif;
}

/* Hero Section */
.hero-section {
  background: url('~/assets/img/hero-bg.jpg') no-repeat center center/cover;
  color: white;
  padding: 5rem 0;
}

.hero-section h1 {
  font-size: 3rem;
  font-weight: bold;
}

.hero-section .lead {
  font-size: 1.25rem;
}

/* Gambar di atas Sambutan Kepala Sekolah */
.header-image-section img {
  width: 100%;
  height: auto;
  margin-bottom: 2rem;
}

/* Sambutan Kepala Sekolah Section */
.sambutan-section {
  background-color: #f8f9fa;
}

.sambutan-section h2 {
  font-size: 2.5rem;
  font-weight: bold;
  color: #333;
}

/* Berita Terbaru Section */
.berita-section h2 {
  font-size: 2.5rem;
  font-weight: bold;
  color: #333;
}

.card {
  border-radius: 10px;
  box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1);
  transition: transform 0.3s;
}

.card:hover {
  transform: translateY(-5px);
}

.card-img-top {
  height: 200px;
  object-fit: cover;
}

/* Footer */
footer {
  background-color: #343a40;
}

footer p {
  margin: 0;
  color: #adb5bd;
}

/* Responsive Design */
@media (max-width: 768px) {
  .hero-section h1 {
    font-size: 2rem;
  }

  .hero-section .lead {
    font-size: 1rem;
  }

  .sambutan-section .row {
    flex-direction: column-reverse;
  }

  .sambutan-section img {
    width: 100%;
    height: auto;
  }
}
</style>
