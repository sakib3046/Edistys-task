<script lang="ts">
	type Imagetype = {
		title: string;
		src: string;
	};
	export let images: Imagetype[];
	console.log(images);
</script>

<div class="p-6 rounded-lg">
	<ui
		style="list-style-type: none"
		class="flex overflow-x-auto gap-16 snap-x snap-mandatory before:shrink-0 before:w-[10wv] after:w-[10wv]"
	>
		{#each images as { title, src }}
			<li class="shrink-0 snap-center">
				<img class="w-[1200px] rounded-xl" {src} alt={title} />
			</li>
		{/each}
	</ui>
</div>
