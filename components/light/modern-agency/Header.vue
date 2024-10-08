<template>
  <header class="slider slider-prlx">
    <div class="swiper-container parallax-slider">
      <Swiper effect="Parallax" class="swiper-container parallax-slider" v-bind="swiperOptions">
        <SwiperSlide>
          <div class="bg-img valign" data-background="/light/assets/imgs/header/full/5.jpg" data-overlay-dark="4">
            <div class="container">
              <div class="mt-100 caption text-center">
                <h3 class="mb-30" data-swiper-parallax="-2000">JDIH</h3>
                <h6>Pencarian Dokumen dan Informasi Hukum di Lingkungan Kabupaten Mojokerto</h6>
                <div class="c-search-wrapper">
                  <form action="#" method="GET">
                    <input type="hidden" name="cari_peraturan" value="">
                    <div class="row">
                      <div class="col-md-4 search-col search-col-divider">
                        <div class="input-group c-search-wrapper-text c-search-wrapper-divider">
                          <span class="input-group-text" id="search"><i class="fas fa-search"></i></span>
                          <input name="tentang" type="text" class="form-control" placeholder="Masukan Kata Pencarian"
                            aria-label="Search" aria-describedby="search">
                        </div>
                      </div>
                      <div class="col-md-4 search-col search-col-divider">
                        <select name="kategori" class="form-select c-search-wrapper-divider" aria-label="Kategori">
                          <option selected value="all">Pilih Jenis Peraturan</option>
                          <option value="1">Produk Hukum Daerah</option>
                          <option value="2">Produk Hukum Pusat</option>
                        </select>
                      </div>
                      <div class="col-md-2 search-col search-col-divider search-col-tahun">
                        <select name="tahun" class="form-select" aria-label="Tahun">
                          <option selected value="all">Tahun</option>
                          <option value="2024">2024</option>
                          <option value="2023">2023</option>
                          <option value="2022">2022</option>
                          <option value="2021">2021</option>
                        </select>
                      </div>
                      <div class="col-md-2 search-col search-col-submit">
                        <button type="submit" class="btn btn-secondary mb-3 text-white">Cari Peraturan</button>
                      </div>
                    </div>
                  </form>
                </div>
              </div>
            </div>
          </div>
        </SwiperSlide>
        <SwiperSlide>
          <div class="bg-img valign" data-background="/light/assets/imgs/header/full/3.jpg" data-overlay-dark="4">
            <div class="container">
              <div class="caption text-center">
                <h2 class="mb-30" data-swiper-parallax="-2000">
                  We Create Impactful
                </h2>
                <h1>
                  <span data-swiper-parallax="-1000">Digital Experiences</span>
                </h1>
              </div>
            </div>
          </div>
        </SwiperSlide>
        <SwiperSlide>
          <div class="bg-img valign" data-background="/light/assets/imgs/header/full/4.jpg" data-overlay-dark="4">
            <div class="container">
              <div class="caption text-center">
                <h2 class="mb-30" data-swiper-parallax="-2000">Elevate your</h2>
                <h1>
                  <span data-swiper-parallax="-1000">Brand & Fuel Growth</span>
                </h1>
              </div>
            </div>
          </div>
        </SwiperSlide>
      </Swiper>
    </div>
    <div class="slider-contro main-bg">
      <div class="swiper-button-prev swiper-nav-ctrl cursor-pointer">
        <div>
          <span>Prev</span>
        </div>
      </div>
      <div class="ml-30 mr-30">
        <span>/</span>
      </div>
      <div class="swiper-button-next swiper-nav-ctrl cursor-pointer">
        <div>
          <span>Next</span>
        </div>
      </div>

      <div class="shap-left-bottom">
        <svg viewBox="0 0 11 11" fill="none" xmlns="http://www.w3.org/2000/svg" class="w-11 h-11">
          <path d="M11 1.54972e-06L0 0L2.38419e-07 11C1.65973e-07 4.92487 4.92487 1.62217e-06 11 1.54972e-06Z"
            fill="#1a1a1a"></path>
        </svg>
      </div>
      <div class="shap-right-top">
        <svg viewBox="0 0 11 11" fill="none" xmlns="http://www.w3.org/2000/svg" class="w-11 h-11">
          <path d="M11 1.54972e-06L0 0L2.38419e-07 11C1.65973e-07 4.92487 4.92487 1.62217e-06 11 1.54972e-06Z"
            fill="#1a1a1a"></path>
        </svg>
      </div>
    </div>
    <div class="swiper-pagination"></div>
  </header>
</template>

<style scoped>
.c-search-wrapper {
  margin-top: 11px;
  padding: 5px 15px;
  width: 100%;
  max-width: 1000px;
  height: 50px;
  background: #ffffff;
  border: 1px solid #ecedf2;
  box-shadow: 0px 6px 15px rgba(64, 79, 104, 0.05);
  border-radius: 120px;
  margin: 11px auto auto;
  /* This centers the element horizontally */
}

.c-search-wrapper .input-group-text {
  background-color: transparent;
  border: none;
}

.c-search-wrapper .form-control {
  border-radius: 120px;
  border: none;
  box-shadow: 1px;
}

.c-search-wrapper .form-select {
  border-radius: 120px;
  border: 1px solid #ecedf2;
}

.c-search-wrapper .btn {
  border-radius: 120px;
}
</style>

<script setup>
import { Swiper, SwiperSlide } from 'swiper/vue';
import { Navigation, Pagination, Parallax } from 'swiper';
import { onMounted } from 'vue';
//= Common Scripts
import loadBackgroudImages from '@/common/loadBackgroudImages';

// Initialize background images when component is mounted
onMounted(() => {
  loadBackgroudImages();
});
const swiperOptions = {
  modules: [Navigation, Parallax, Pagination],

  spaceBetween: 30,
  speed: 600,
  navigation: {
    nextEl: '.slider-contro .swiper-button-next',
    prevEl: '.slider-contro .swiper-button-prev',
  },
  pagination: {
    el: '.swiper-pagination',
  },
};
</script>
