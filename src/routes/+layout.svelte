<script>
	import '../app.css';
	import Footer from './components/footer.svelte';
	import Navbar from './components/navbar.svelte';
</script>

<Navbar />
<slot />
<footer class="">
	<Footer />
</footer>
