<template>
  <div class="home-page">
    <!-- hero -->
    <section
      class="relative h-screen bg-cover bg-center border-t border-black"
      :style="{ backgroundImage: `url(${heroImage})` }"
    >
      <div class="absolute inset-0 bg-gray-900/60"></div>

      <div class="relative z-10 h-full max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
        <div class="h-full flex flex-col justify-center items-start md:w-1/2 md:ml-auto">
          <h1 class="text-4xl md:text-5xl font-bold mb-6">
            Lari Lebih Ringan, <br />Barang Lebih Aman
          </h1>

          <p class="text-xl md:text-2xl font-semibold text-white mb-8 max-w-lg">
            Titip barang kamu di LAHRINGAN, <br />
            solusi penitipan untuk pelari, pejalan santai, dan komunitas aktif.
          </p>

          <RouterLink
            to="/contact"
            class="bg-black text-white px-4 py-2 rounded-md text-sm font-semibold hover:bg-gray-800 focus:outline-none cursor-pointer transition-all duration-300 hover:scale-115"
        >
            Kontak Kami
          </RouterLink>
        </div>
      </div>
    </section>

    <!-- profifl -->
    <section class="py-16">
      <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
        <div class="text-center mb-12">
          <h2 class="text-3xl md:text-4xl font-semibold mb-4">
            Kami Hadir untuk Menemani Langkahmu
          </h2>
          <h4 class="text-xl md:text-2xl font-normal mb-4">
            LAHRINGAN adalah layanan penitipan barang yang diciptakan untuk para pelari, komunitas aktif, dan siapa pun yang ingin bergerak tanpa beban.
          </h4>
        </div>

        <div class="grid grid-cols-1 md:grid-cols-3 gap-8 border-t border-b border-black divide-x-3 divide-dashed">
          <div class="bg-white text-black p-6">
            <h3 class="text-xl font-semibold mb-4 text-start">Ruang Antara Kantor <br> dan <br> Garis Start</h3>
          </div>

          <div class="bg-white text-black p-6">
            <h3 class="text-xl font-semibold mb-4 text-justify">Berawal dari keresahan kecil, ke mana harus menitipkan barang saat lari pagi di CFD, kami memutuskan untuk membuat solusi yang sederhana tapi berguna: penitipan aman, cepat, dan bisa dipercaya.</h3>
          </div>

          <div class="bg-white text-black p-6">
            <h3 class="text-xl font-semibold mb-4 text-justify">Kini, LAHRINGAN hadir di berbagai titik kota, membantu ratusan pelari menikmati kebebasan tanpa khawatir barang tertinggal.</h3>
          </div>
        </div>
        
      </div>
    </section>

  </div>
</template>

<script setup>
import heroImage from '@/assets/jogging.jpg'

</script>
