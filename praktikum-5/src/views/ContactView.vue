<template>
	<div class="contact">
		<!-- hero -->
		<section
			class="relative h-96 bg-cover bg-center border-t border-black"
			:style="{ backgroundImage: `url(${heroImage})` }"
		>
			<div class="absolute inset-0 bg-gray-900/60"></div>

			<div class="relative z-10 h-full max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
				<div class="h-full flex flex-col justify-center">
					<h1
						class="text-4xl text-center text-slate-100 font-extrabold mb-6 drop-shadow-4xl shadow-black"
					>
						Ayo Terhubung dengan kami
					</h1>
					<p
						class="text-lg text-center text-slate-100 font-semibold mb-6 drop-shadow-4xl shadow-black"
					>
						biar ga lepas kontak gitu loh
					</p>
				</div>
			</div>
		</section>

		<!-- info  -->
		<section class="py-16">
			<div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
				<div class="text-center mb-12">
					<h2 class="text-3xl md:text-4xl font-semibold mb-4">
						Hubungi kami untuk Informasi Lebih Lanjut atau <br> langsung OTW ke
						lokasi
					</h2>
				</div>

				<div class="grid grid-cols-1 md:grid-cols-2 gap-8">
					<div class="bg-white text-black p-6">
						<div class="md:col-span-2 mt-8 md:mt-0 md:pl-12 text-black">
							<h2 class="text-3xl font-semibold mb-6">Kontak Kami</h2>
							<h4 class="text-lg font-semibold mb-6">Datang Kesini</h4>
							<p class="mb-4 text-xl">
								Alamat: Ruko Golden Boulevard, Ruko Grand City AC20, Batu Ampar,
								Kota Balikpapan
							</p>
							<h4 class="text-lg font-semibold mb-6">Atau lewat online</h4>
							<p class="mb-4">Telepon: +628-8000-8080</p>
							<p class="mb-4">support@lahringan.id</p>
							<p class="mb-4">
								Jam Operasional: Senin - Jumat, 08.00 - 17.00 WIB
							</p>
						</div>
					</div>

					<div class="bg-white text-black p-6">
						<div
							class="relative bg-gray-200"
							:style="{ height: '400px', width: '600px' }"
						>
							<iframe
								class="absolute top-0 left-0 w-full h-full rounded-2xl"
								src="https://www.google.com/maps/embed?pb=!1m14!1m12!1m3!1d42520.75278603332!2d116.85811365339652!3d-1.2445973275210618!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!5e1!3m2!1sid!2sid!4v1762916513198!5m2!1sid!2sid"
								frameborder="0"
								style="border: 0"
								allowfullscreen=""
								loading="lazy"
								aria-hidden="false"
								referrerpolicy="no-referrer-when-downgrade"
							></iframe>
						</div>
						<div class="pt-5 text-center">
							<button
								@click="openInMaps"
								class="bg-black text-white px-4 py-2 rounded-md text-sm font-semibold hover:bg-gray-800 focus:outline-none cursor-pointer transition-all duration-300 hover:scale-115"
							>
								Buka di Maps
							</button>
						</div>
					</div>
				</div>
			</div>
		</section>
	</div>
</template>

<script setup>
import heroImage from '@/assets/cs.jpg';

function openInMaps() {
	window.open(
		'https://www.google.com/maps/embed?pb=!1m14!1m12!1m3!1d42520.75278603332!2d116.85811365339652!3d-1.2445973275210618!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!5e1!3m2!1sid!2sid!4v1762916513198!5m2!1sid!2sid',
		'_blank'
	);
}
</script>
