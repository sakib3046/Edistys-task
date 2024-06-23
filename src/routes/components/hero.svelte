<script>
	import Card from './card.svelte';

	let cardData = [
		{
			title: 'Test Card',
			src: '/src/assets/cardicons/1.png',
			shortDes: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit.'
		},
		{
			title: 'Test Card',
			src: '/src/assets/cardicons/2.png',
			shortDes: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit.'
		},
		{
			title: 'Test Card',
			src: '/src/assets/cardicons/3.png',
			shortDes: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit.'
		},
		{
			title: 'Test Card',
			src: '/src/assets/cardicons/4.png',
			shortDes: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit.'
		},
		{
			title: 'Test Card',
			src: '/src/assets/cardicons/5.png',
			shortDes: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit.'
		},
		{
			title: 'Test Card',
			src: '/src/assets/cardicons/6.png',
			shortDes: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit.'
		}
	];
</script>

<div class="bg-200 p-6 m-6 flex flex-col justify-center rounded-lg shadow-lg relative">
	<h1 class="m-auto text-3xl">
		This is a example project <span class="font-bold text-400"> prove my self</span>
	</h1>
	<div class="mt-10 bg-50 rounded-lg p-4 m-2 w-full flex flex-col justify-center">
		<div class="flex flex-row justify-stretch">
			<div class="bg-500 rounded-sm w-2 h-10 justify-self-end"></div>
			<h1 class="mx-4 text-4xl font-extrabold justify-self-start">About Me</h1>
		</div>

		<div class=" my-4 bg-950/50 w-full h-1"></div>
		<p class="px-2">
			Lorem ipsum dolor sit amet, consectetur adipiscing elit. Aliquam vestibulum maximus nulla,
			eget scelerisque dui auctor ut. Nam ultricies elit tristique gravida mollis. Donec ac iaculis
			neque. Sed rhoncus, tellus vitae rutrum iaculis, quam odio porttitor nunc, aliquet dictum arcu
			risus dignissim sem. Nullam sit amet sapien nec urna luctus mattis ac quis lacus. Integer sed
			risus a nisl dignissim efficitur. Vestibulum id pretium nisl, a cursus urna. Aliquam ut neque
			ipsum. Morbi quis facilisis ex. Maecenas nunc lorem, tempus eget magna quis, fringilla posuere
			ligula. Integer sit amet ultrices nisi, nec mollis purus. Fusce pulvinar dui sagittis neque
			aliquam maximus. Vestibulum molestie, tellus sed pharetra cursus, leo mi volutpat nisl, in
			volutpat nulla tellus eget velit. Donec aliquam lacus justo, id porta nibh hendrerit id. Nulla
			placerat maximus ligula, quis consectetur mauris dignissim sit amet. Etiam diam elit,
			vestibulum vel eleifend a, gravida quis ipsum. Vestibulum sed erat pellentesque nunc auctor
			accumsan. Ut augue libero, tristique et lectus lacinia, mollis malesuada turpis.
		</p>
	</div>
</div>
<div class="flex flex-row">
	{#each cardData as data}
		<Card cardData={data} />
	{/each}
</div>
