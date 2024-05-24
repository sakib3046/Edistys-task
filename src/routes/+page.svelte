<script lang="ts">
	import Cerousel from './components/cerousel.svelte';

	let carImages = [
		{ title: '1', src: '/src/assets/1.jpg' },
		{ title: '2', src: '/src/assets/2.jpg' },
		{ title: '3', src: '/src/assets/3.jpg' },
		{ title: '4', src: '/src/assets/4.jpg' }
	];
</script>

<div class="">
	<Cerousel CarouselImage={carImages} />
</div>
