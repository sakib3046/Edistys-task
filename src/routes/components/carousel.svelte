<script lang="ts">
	type Imagetype = {
		title: string;
		src: string;
	};
	export let images: Imagetype[];
	console.log(images);
</script>

<div class="relative rounded-lg">
	<ui
		style="list-style-type: none"
		class="flex overflow-x-auto gap-6 snap-x snap-mandatory before:shrink-0 before:w-[10wv] after:w-[10wv]"
	>
		{#each images as { title, src }}
			<li class="shrink-0 snap-center">
				<div class="bg-gradient-to-t from-200 to-50% absolute z-20 left-0 w-full h-full"></div>
				<div
					class="w-[1200px] h-[350px] bg-no-repeat bg-cover bg-center"
					style="background-image: url({src})"
				></div>
			</li>
		{/each}
	</ui>
</div>
