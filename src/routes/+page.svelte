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
<iframe
	width="560"
	height="315"
	src="https://www.youtube.com/embed/2jKCUWL8F8Q?si=jn6lzVwe0x6IZi3u"
	title="YouTube video player"
	frameborder="0"
	allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
	referrerpolicy="strict-origin-when-cross-origin"
	allowfullscreen
></iframe>
<Features />
<Screenshot />
<Trial />

<Footer />

<svelte:head>
	<title>Krittim Home Page</title>
</svelte:head>
