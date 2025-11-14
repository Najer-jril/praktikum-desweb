<template>
	<header class="bg-slate-100 shadow-md sticky top-0 z-50">
		<div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
			<div class="flex justify-between items-center h-16">
				<div class="flex items-center">
					<RouterLink to="/" class="text-3xl text-black font-bold">
						Muhammad Nazril Ilham
					</RouterLink>
				</div>

				<nav class="hidden md:flex space-x-8">
					<RouterLink to="/" v-slot="{ isActive }">
						<span
							:class="[
								'hover:text-red-700 hover:-translate-y-0.5 transition-all duration-200 font-semibold cursor-pointer',
								isActive
									? 'text-red-700 underline underline-offset-4'
									: 'text-black',
							]"
						>
							Home
						</span>
					</RouterLink>

					<RouterLink to="/contact" v-slot="{ isActive }">
						<span
							:class="[
								'hover:text-red-700 hover:-translate-y-0.5 transition-all duration-200 font-semibold cursor-pointer',
								isActive
									? 'text-red-700 underline underline-offset-4'
									: 'text-black',
							]"
						>
							Contact
						</span>
					</RouterLink>
				</nav>
			</div>
		</div>
	</header>
</template>

<script setup>

defineOptions({
	name: 'AppNavbar',
});

</script>
