<template>
  <div id="HotelRec">
    <div class="container">
      <!-- bagian judul -->
      <div class="row justify-content-between mt-5">
        <div class="col-lg-4"></div>
        <div class="col-lg-4 text-center rekomendasi mb-3">
          <h5>Rekomendasi Hotel</h5>
        </div>
        <div class="col-lg-4 text-end">
          <router-link to="ListView" href="">Lihat Semua</router-link>
        </div>
      </div>
      <!-- akhir bagian judul -->

      <!-- card -->
      <div class="row justify-content-between mt-4">
        <div class="col-lg-4">
          <div class="card shadow" style="width: 100%">
            <img src="../assets/amaris.png" class="img" alt="..." />
            <div class="card-body">
              <h5 class="Hotel Amaris">Amaris Hotel Palembang</h5>
              <p class="Harga Amaris">Rp.300k,-/malam</p>
              <div class="row">
                <div class="col text-start">
                  <router-link to="PemesananView" href="#" class="btn btn-primary">Pesan Sekarang</router-link>
                </div>
                <div class="col text-end mt-2">
                  <img src="../assets/Star1.png" alt="" />
                  <span>4.6 Rb</span>
                </div>
              </div>
            </div>
          </div>
        </div>
        <div class="col-lg-4">
          <div class="card shadow" style="width: 100%">
            <img src="../assets/arista.png" class="img" alt="..." />
            <div class="card-body">
              <h5 class="card-title">Arista Hotel Palembang</h5>
              <p class="card-text">Rp.300k,-/malam</p>
              <div class="row">
                <div class="col text-start">
                  <router-link to="PemesananView" class="btn btn-primary">Pesan Sekarang</router-link>
                </div>
                <div class="col text-end mt-2">
                  <img src="../assets/Star1.png" alt="" />
                  <span>4.6 Rb</span>
                </div>
              </div>
            </div>
          </div>
        </div>
        <div class="col-lg-4">
          <div class="card shadow" style="width: 100%">
            <img src="../assets/alts.png" class="img" alt="..." />
            <div class="card-body">
              <h5 class="card-title">The Alts Hotel Palembang</h5>
              <p class="card-text">Rp.300k,-/malam</p>
              <div class="row">
                <div class="col text-start">
                  <router-link to="PemesananView" href="#" class="btn btn-primary">Pesan Sekarang</router-link>
                </div>
                <div class="col text-end mt-2">
                  <img src="../assets/Star1.png" alt="" />
                  <span>4.6 Rb</span>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
      <!-- akhir bagian card -->
    </div>
  </div>
</template>

<script>
export default {
  name: "HotelRec",
};
</script>

<style>
</style>