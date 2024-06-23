<script>
	import emblaCarouselSvelte from 'embla-carousel-svelte';
	import Autoplay from 'embla-carousel-autoplay';
	export let CarouselImage;
	let options = { loop: true };
	let plugins = [Autoplay()];
</script>

<div
	class="embla mx-6 rounded-xl relative shadow-lg"
	use:emblaCarouselSvelte={{ options, plugins }}
>
	<div class="embla__container">
		<div class="embla__slide"><img src={CarouselImage[0].src} alt="" /></div>
		<div class="embla__slide"><img src={CarouselImage[1].src} alt="" /></div>
		<div class="embla__slide"><img src={CarouselImage[2].src} alt="" /></div>
		<div class="embla__slide"><img src={CarouselImage[3].src} alt="" /></div>
	</div>
</div>

<style>
	.embla {
		overflow: hidden;
	}
	.embla__container {
		display: flex;
	}
	.embla__slide {
		flex: 0 0 100%;
		min-width: 0;
		@apply w-full h-96;
	}
</style>
