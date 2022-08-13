<template>
  <div id="CityRec">
    <div class="container">
      <!-- bagian judul -->
      <div class="row justify-content-between">
        <div class="col-lg-4"></div>
        <div class="col-lg-4 text-center rekomendasi">
          <h5>Rekomendasi Hotel Berdasarkan Kota</h5>
        </div>
        <div class="col-lg-4 text-end">
          <router-link to="ListView" href="">Lihat Semua</router-link>
        </div>
      </div>
      <!-- akhir bagian judul -->

      <!-- Kota -->
      <div class="row kota mt-5">
        <div class="col-lg-3 mt-2">
          <div class="bg-KotaSatu shadow">
            <div class="row">
              <div class="col Kota">
                <h3>Kota Palembang</h3>
                <h5>110+ akomodasi</h5>
              </div>
            </div>
          </div>
        </div>
        <div class="col-lg-3 mt-2">
          <div class="bg-KotaDua shadow">
            <div class="row">
              <div class="col Kota">
                <h3>Kota Yogya</h3>
                <h5>110+ akomodasi</h5>
              </div>
            </div>
          </div>
        </div>
        <div class="col-lg-3 mt-2">
          <div class="bg-KotaTiga shadow">
            <div class="row">
              <div class="col Kota">
                <h3>Kota Denpasar</h3>
                <h5>110+ akomodasi</h5>
              </div>
            </div>
          </div>
        </div>
        <div class="col-lg-3 mt-2">
          <div class="bg-KotaEmpat shadow">
            <div class="row">
              <div class="col Kota">
                <h3>Kota jakarta</h3>
                <h5>110+ akomodasi</h5>
              </div>
            </div>
          </div>
        </div>
      </div>
      <!-- Akhir bagian Kota -->
    </div>
  </div>
</template>

<script>
export default {
  name: "CityRec",
};
</script>

<style>
#CityRec .bg-KotaSatu {
  background-image: url("/src/assets/palembang.png");
  width: 100%;
  height: auto;
  background-size: cover;
  border-radius: 15px;
  margin-bottom: 20px;
}
#CityRec .bg-KotaDua {
  background-image: url("/src/assets/yogya.png");
  width: 100%;
  height: auto;
  background-size: cover;
  border-radius: 15px;
  margin-bottom: 20px;
}
#CityRec .bg-KotaTiga {
  background-image: url("/src/assets/denpasar.png");
  width: 100%;
  height: auto;
  background-size: cover;
  border-radius: 15px;
  margin-bottom: 20px;
}
#CityRec .bg-KotaEmpat {
  background-image: url("/src/assets/jakarta.png");
  width: 100%;
  height: auto;
  background-size: cover;
  border-radius: 15px;
  margin-bottom: 20px;
}

</style>