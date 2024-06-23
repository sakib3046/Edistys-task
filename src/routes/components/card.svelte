<script>
	export let cardData;
</script>

<div
	class=" overflow-scroll no-scrollbar bg-400/25 backdrop-blur-lg shadow-xl w-[240px] h-[300px] rounded-lg p-6 m-6"
	style="-ms-overflow-style: none;  scrollbar-width: none;"
>
	<img src={cardData.src} class="h-[25vh] m-auto" alt="" />
	<a href="" class="font-bold">{cardData.title}</a>
	<p>{cardData.shortDes}</p>
</div>
