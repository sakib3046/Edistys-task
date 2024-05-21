<script land="ts">
	let navOptions = [
		{ name: 'home', link: '/' },
		{ name: 'Services', link: '/services' }
	];
</script>

<div class="w-full px-6">
	<div
		class="z-50 top-0 left-0 my-4 flex flex-row justify-between w-full bg-gradient-to-r from-400 via-200 to-600 px-6 py-3 shadow-xl shadow-950/10 rounded-lg"
	>
		<a href="/" class=" flex flex-col leading-3 hover:scale-110 duration-200">
			<span class="font-bold">Edistys</span>
			<span class="">Intern</span>
		</a>
		<div class="space-x-4 flex flex-row text-50 font-bold text-xl">
			{#each navOptions as option}
				<a
					class="hover:text-white hover:-translate-y-0.5 hover:scale-110 duration-200"
					href={option.link}>{option.name}</a
				>
			{/each}
		</div>
	</div>
</div>
