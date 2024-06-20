<script>
	import Hero from '$lib/Hero.svelte';
	import Features from '$lib/Features.svelte';
	import Screenshot from '$lib/Screenshot.svelte';
	import Trial from '$lib/Trial.svelte';
	import Footer from '$lib/Footer.svelte';
</script>

<div class="navbar bg-base-100">
	<div class="navbar-start">
		<a class="btn btn-ghost text-xl" href="/">Krittim</a>
	</div>
	<div class="navbar-end">
		<a class="btn btn-success" href="/download">Download</a>
	</div>
</div>

<Hero />

<Features />
<Screenshot />
<Trial />

<Footer />


<svelte:head>
	<title>Krittim Home Page</title>
</svelte:head>
