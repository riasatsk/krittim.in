<script>
	import '../app.css';
	import { onMount } from 'svelte';

	onMount(() => {
		const theme = localStorage.getItem('theme') || 'cupcake';
		document.documentElement.setAttribute('data-theme', theme);
	});
</script>

<slot />
