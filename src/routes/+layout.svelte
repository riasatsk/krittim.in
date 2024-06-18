<script>
	import '../app.css';
	import { onMount } from 'svelte';

	onMount(() => {
		document.documentElement.setAttribute('data-theme', 'light');
	});
</script>

<slot />
