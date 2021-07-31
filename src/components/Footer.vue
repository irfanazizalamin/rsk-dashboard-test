<template>
  <!-- Footer -->
  <footer class="footer text-white">
    <!-- Section: Links  -->
    <section class="footer__body">
      <div class="container text-center text-md-start mt-5">
        <!-- Grid row -->
        <div class="row mt-3">
          <!-- Grid column -->
          <div class="col-md-3 col-lg-4 col-xl-3 mx-auto mb-4">
            <!-- Content -->
            <img
              class="footer__logo"
              src="../assets/img/icons/rsk-logo.svg"
              alt="rsk-logo"
            >
            <h6>Lokasi Kami</h6>
            <p>
              Jl. Bulungan No.26, Jakarta Selatan, DKI Jakarta 12130
            </p>
          </div>
          <!-- Grid column -->

          <!-- Grid column -->
          <div class="col-md-2 col-lg-2 col-xl-2 mx-auto mb-4">
            <!-- Links -->
            <h6 class="text-uppercase fw-bold mb-4">Peta Situs</h6>
            <p>
              <a href="#!" class="text-reset">Beranda</a>
            </p>
            <p>
              <a href="#!" class="text-reset">Perusahaan</a>
            </p>
            <p>
              <a href="#!" class="text-reset">Syarat & Ketentuan</a>
            </p>
            <p>
              <a href="#!" class="text-reset">Tentang Kami</a>
            </p>
          </div>
          <!-- Grid column -->

          <!-- Grid column -->
          <div class="col-md-2 col-lg-2 col-xl-2 mx-auto mb-4">
            <!-- Links -->
            <h6 class="text-uppercase fw-bold mb-4">Produk</h6>
            <p>
              <a href="#!" class="text-reset">Kelas</a>
            </p>
            <p>
              <a href="#!" class="text-reset">Prakerja</a>
            </p>
            <p>
              <a href="#!" class="text-reset">Lowongan</a>
            </p>
            <p>
              <a href="#!" class="text-reset">Kawan Cuan</a>
            </p>
          </div>
          <!-- Grid column -->

          <!-- Grid column -->
          <div class="col-md-3 col-lg-3 col-xl-3 mx-auto mb-4">
            <!-- Links -->
            <h6 class="text-uppercase fw-bold mb-4">Kontak Kami</h6>
            <p>
              <img
                class="sosmed-icon"
                src="../assets/img/icons/facebook.svg"
                alt="fb-logo"
              >
              <a href="#!" class="text-reset">Rumah Siap Kerja</a>
            </p>
            <p>
              <img
                class="sosmed-icon"
                src="../assets/img/icons/instagram.svg"
                alt="ig-logo"
              >
              <a href="#!" class="text-reset">@rumahsiapkerja</a>
            </p>
            <p>
              <img
                class="sosmed-icon"
                src="../assets/img/icons/mail.svg"
                alt="mail-logo"
              >
              <a href="#!" class="text-reset">info@rumahsiapkerja.com</a>
            </p>
            <p>
              <img
                class="sosmed-icon"
                src="../assets/img/icons/whatsapp.svg"
                alt="wa-logo"
              >
              <a href="#!" class="text-reset">0812 1244 1399</a>
            </p>
          </div>
          <!-- Grid column -->
        </div>
        <!-- Grid row -->
        <div class="copyright">
          © Rumah Siap Kerja 2021 - PT Samala Serasi Unggul. All Rights Reserved.
        </div>
      </div>
    </section>
    <!-- Section: Links  -->
  </footer>
  <!-- Footer -->
</template>

<script>
export default {
  name: 'Footer',
};
</script>

<style lang="scss">
.footer {
  background-color: #3c77bf;

  &__body {
    padding: 8px 0;
  }

  &__logo {
    width: 50%;
    margin: 0 0 20px -24px;
  }
}

a {
  text-decoration: none !important;
  font-size: 14px;
}

.sosmed-icon {
  width: 24px;
  margin-right: 12px;
}

.row {
  padding: 0 !important;
}

.copyright {
  font-size: 14px;
  margin-left: 12px;
}
</style>
