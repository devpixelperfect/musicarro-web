<script>
	import Header from '$lib/components/Header.svelte';
	import Footer from '$lib/components/Footer.svelte';
	import '$lib/css/main.css';
</script>

<div class="app">
	<Header />

	<main>
		<slot />
	</main>

	<Footer>
	</Footer>
</div>

<style>

</style>
