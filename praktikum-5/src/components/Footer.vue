<template>
  <footer class="bg-slate-100 text-black border-t border-gray-700">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 py-12">
      <div class="grid grid-cols-1 md:grid-cols-4 gap-8">
        <div>
          <RouterLink to="/" class="text-3xl font-bold"> LAHRINGAN </RouterLink>
          <p class="text-xl font-semibold">
            Lari Senang Kalau
            <br />Barang Aman.
          </p>

		  <p class="text-sm mt-4 font-semibold text-amber-900">
			Tugas Praktikum <br> Vue Routing + Tailwind CSS
		  </p>
        </div>

        <!-- link -->
        <div>
          <h4 class="text-lg font-semibold mb-4">Navigasi Cepat</h4>
          <div class="grid grid-cols-2 gap-4 font-normal">
            <ul class="space-y-2">
              <li>
                <RouterLink to="/" class="hover:text-black transition">Home</RouterLink>
              </li>
              <li>
                <RouterLink to="/contact" class="hover:text-black transition">Contact</RouterLink>
              </li>
            </ul>
          </div>
        </div>

        <!-- sosmed -->
        <div>
          <h4 class="text-lg font-semibold mb-4">Ikuti Kami</h4>
          <ul class="space-y-2 font-normal">
            <li>
              <a href="http://instagram.com/najriiil" target="_blank" rel="noopener noreferrer" class="hover:text-white transition"
                >Instagram</a
              >
            </li>
            <li>
              <a href="http://twitter.com/" target="_blank" rel="noopener noreferrer" class="hover:text-white transition">X</a>
            </li>
            <li>
              <a href="http://facebook.com/" target="_blank" rel="noopener noreferrer" class="hover:text-white transition">Facebook</a>
            </li>
            <li>
              <a href="http://strava.com/" target="_blank" rel="noopener noreferrer" class="hover:text-white transition">Strava</a>
            </li>
          </ul>
        </div>

        <!-- Info kontak -->
        <div>
          <h4 class="text-lg font-semibold mb-4">Kontak Kami</h4>
          <ul class="space-y-2 text-sm font-normal">
            <li>Ruko Golden Boulevard, Ruko Grand City AC20, Batu Ampar, Kota Balikpapan</li>
            <li>+628-8000-8080</li>
            <li>support@lahringan.id</li>
          </ul>
        </div>
      </div>

      <div class="border-t border-gray-700 mt-8 pt-8 text-center">
        <p class="text-sm">&copy; {{ currentYear }} Lahringan. All rights reserved.</p>
      </div>
    </div>
  </footer>
</template>

<script setup>
defineOptions({ name: 'AppFooter' })
import { computed } from 'vue'

const currentYear = computed(() => new Date().getFullYear())
</script>
