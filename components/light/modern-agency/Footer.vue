<!-- <template>
  <footer class="modern-footer pt-80">
    <div class="footer-container">
      <div class="container ontop">
        <div class="row pb-30 bord-thin-bottom">
          <div class="col-lg-5">
            <div class="logo icon-img-120">
              <img src="/light/assets/imgs/logo-light.png" alt="" />
            </div>
          </div>
          <div class="col-lg-7">
            <div class="social-media d-flex justify-content-end">
              <ul class="rest d-flex align-items-center fz-14">
                <li class="hover-this cursor-pointer">
                  <a href="#0" class="hover-anim">
                    <i class="fab fa-facebook-f mr-10"></i> Facebook
                  </a>
                </li>
                <li class="hover-this cursor-pointer ml-50">
                  <a href="#0" class="hover-anim">
                    <i class="fab fa-dribbble mr-10"></i> Dribbble
                  </a>
                </li>
                <li class="hover-this cursor-pointer ml-50">
                  <a href="#0" class="hover-anim">
                    <i class="fab fa-linkedin-in mr-10"></i> LinkedIn
                  </a>
                </li>
                <li class="hover-this cursor-pointer ml-50">
                  <a href="#0" class="hover-anim">
                    <i class="fab fa-instagram mr-10"></i> Instagram
                  </a>
                </li>
              </ul>
            </div>
          </div>
        </div>
        <div class="row pt-80">
          <div class="col-lg-7">
            <div class="call-action">
              <h2 class="d-slideup wow fz-60 fw-600">
                <span class="sideup-text">
                  <span class="up-text">Have a project in mind?</span>
                </span>
                <span class="sideup-text">
                  <span class="up-text underline">
                    <a href="/light/page-contact3" class="main-color">
                      Let’s get to work.
                    </a>
                  </span>
                </span>
              </h2>
              <div class="info mt-80 d-flex align-items-center">
                <div>
                  <a href="#0" class="butn butn-md butn-bord-thin radius-30">
                    <span class="text">Support@Website.com</span>
                  </a>
                </div>
                <div>
                  <a
                    href="#0"
                    class="butn butn-md butn-bord-thin radius-30 ml-30"
                  >
                    <span class="text">+2 456 (343) 24 45</span>
                  </a>
                </div>
              </div>
            </div>
          </div>
          <div class="col-lg-4 offset-lg-1 bord-left">
            <div class="column">
              <h6 class="sub-title mb-30">Useful Links</h6>
              <div class="row">
                <div class="col-6">
                  <ul class="rest fz-14">
                    <li class="mb-15">
                      <a href="/light/page-about3">About</a>
                    </li>
                    <li class="mb-15">
                      <a href="/light/page-services">Services</a>
                    </li>
                    <li class="mb-15">
                      <a href="/light/blog-list2">Blog</a>
                    </li>
                    <li>
                      <a href="/light/page-contact3">Contact</a>
                    </li>
                  </ul>
                </div>
                <div class="col-6">
                  <ul class="rest fz-14">
                    <li class="mb-15">
                      <a href="/light/page-FAQS">FAQS</a>
                    </li>
                    <li class="mb-15">
                      <a href="/light/page-about2">Term & Conditions</a>
                    </li>
                    <li class="mb-15">
                      <a href="/light/page-about2">Privacy policy</a>
                    </li>
                    <li>
                      <a href="/light/page-about2">Help</a>
                    </li>
                  </ul>
                </div>
              </div>
            </div>
            <div class="subscribe-minimal mt-50">
              <form action="contact.php">
                <div class="form-group rest">
                  <input type="email" placeholder="Type Your Email" />
                  <button type="submit">
                    <i class="ti-arrow-top-right"></i>
                  </button>
                </div>
              </form>
            </div>
          </div>
        </div>
        <div class="text-center pt-30 pb-30 sub-bg mt-80">
          <p class="fz-14">
            © 2024 InFolio is Proudly Powered by
            <span class="underline main-color">
              <a href="https://themeforest.net/user/UiCamp" target="_blank">
                UiCamp
              </a>
            </span>
          </p>
        </div>
      </div>
    </div>
  </footer>
</template>
<script setup>
import { onMounted } from 'vue';
onMounted(() => {
  gsap.set('.footer-container', { yPercent: -50 });
  const uncover = gsap.timeline({ paused: true });
  uncover.to('.footer-container', { yPercent: 0, ease: 'none' });

  ScrollTrigger.create({
    trigger: 'main',
    start: 'bottom bottom',
    end: '+=50%',
    animation: uncover,
    scrub: true,
  });
});
</script> -->


<template>
  <footer class="bg-dark-red text-light py-5">
    <div class="container">
      <div class="row justify-content-between align-items-start">
        <!-- Logo dan Deskripsi -->
        <div class="col-md-4 mb-4">
          <div class="text-center text-md-start">
            <img src="/public/light/assets/imgs/logo.png" alt="Logo Mojokerto" class="mb-3 logo-footer">
            <p class="small">
              Website dikelola oleh: <br>
              Sekretariat Kabupaten Mojokerto | Bagian Hukum
            </p>
          </div>
        </div>

        <!-- Statistik Pengunjung -->
        <div class="col-md-4 mb-4">
          <h5 class="mb-3 text-uppercase">Statistik Pengunjung</h5>
          <ul class="list-unstyled">
            <li><i class="bi bi-person-fill me-2"></i>Pengunjung Website Hari ini: 269</li>
            <li><i class="bi bi-people-fill me-2"></i>Pengunjung Website Minggu ini: 3172</li>
            <li><i class="bi bi-calendar-event-fill me-2"></i>Pengunjung Website Bulan ini: 17362</li>
            <li><i class="bi bi-calendar3 me-2"></i>Pengunjung Website Tahun ini: 85619</li>
            <li><i class="bi bi-bar-chart-fill me-2"></i>Total Pengunjung: 170302</li>
          </ul>
        </div>

        <!-- Informasi Kontak -->
        <div class="col-md-4">
          <h5 class="mb-3 text-uppercase">Alamat</h5>
          <ul class="list-unstyled">
            <li>
              <i class="bi bi-geo-alt-fill me-2"></i>
              <strong>Lokasi:</strong><br>
              Jl. Ahmad Yani No.16, Mergelo, Purwotengah, Kec. Magersari, Kota Mojokerto, Jawa Timur 61311
            </li>
            <li class="mt-2">
              <i class="bi bi-telephone-fill me-2"></i>
              <strong>Call Center:</strong> 112
            </li>
            <li class="mt-2">
              <i class="bi bi-envelope-fill me-2"></i>
              <strong>Pengaduan:</strong> damarmojo.lapor.go.id
            </li>
          </ul>
        </div>
      </div>

      <!-- Border top and copyright -->
      <div class="border-top mt-4 pt-3 text-center small">
        &copy; 2024 Kabupaten Mojokerto. All Rights Reserved.
      </div>
    </div>
  </footer>
</template>

<script setup>
</script>

<style scoped>
.bg-dark-red {
  background-color: #000000;
}

footer img.logo-footer {
  max-width: 120px;
  display: block;
  margin: 0 auto;
}

footer p {
  font-size: 0.9rem;
  line-height: 1.5;
}

footer h5 {
  font-weight: bold;
  font-size: 1.1rem;
  letter-spacing: 0.05rem;
}

footer ul {
  font-size: 0.9rem;
}

footer i {
  color: #ffcc00;
}

footer .border-top {
  border-top: 1px solid #555;
  margin-top: 20px;
}

@media (max-width: 768px) {

  footer h5,
  footer ul {
    text-align: center;
  }
}
</style>
