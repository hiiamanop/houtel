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

        <div class="col-lg-4" v-for="hotel in hotelList.data" :key="hotel.id">
          <div class="card shadow" style="width: 100%">
            <img :src="'http://127.0.0.1:8000/storage/' + hotel.gambar" class="img" alt="..." />
            <div class="card-body">
              <h5 class="Hotel Amaris">{{hotel.nama_hotel}}</h5>
              <p class="Harga Amaris">harga</p>
              <div class="row">
                <div class="col text-start">
                  <router-link
                    to="PemesananView"
                    href="#"
                    class="btn btn-primary"
                    >Pesan Sekarang</router-link
                  >
                </div>
                <div class="col text-end mt-2">
                  <img src="../assets/Star1.png" alt="" />
                  <span>4.9 </span>
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
// axios sebagai pengkoneksi dari vue ke api
import axios from "axios";

export default {
  name: "HotelRec",
  // siapkan variable untuk menampung respon api dan list data hotel
  data() {
    return {
      response: "",
      hotelList: "",
    };
  },

  methods: {
    // siapkan method untuk menampung respon api dan list data hotel
    setData(dataAPI) {
      // mengubah variable listhotel, yang tadinya kosong menjadi ada isinya (data response dari API)
      this.hotelList = dataAPI;
    },

    // method/fungsi untuk request ke api
    async getRekomendasiHotel() {
      try {
        // isikan variable response dengan request API
        this.response = await axios.get(
          "http://127.0.0.1:8000/api/rekomendasi-hotel"
        );

        // cetak hasil response
        // console.log(this.response.data);

        // panggil function setData
        this.setData(this.response.data);
      } catch (error) {
        console.log(error);
      }
    },
  },

  // panggil mounted() function yang berfungsi menjalankan fungsi apa saat halaman pertama kali dibuka
  mounted() {
    this.getRekomendasiHotel();
  },
};
</script>

<style>
</style>