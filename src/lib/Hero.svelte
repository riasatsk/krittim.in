<script>

	import { goto } from "$app/navigation";

</script>
<section class="bg-gray-100 h-screen flex items-center justify-center text-gray-900">
	<div class="text-center max-w-xl mx-auto px-4 sm:px-6 md:px-8">
		<h1 class="text-3xl sm:text-4xl md:text-5xl font-bold mb-4 leading-tight">
			Transform Your School Management Digitally
		</h1>
		<p class="text-lg sm:text-xl md:text-2xl mb-8 leading-relaxed">
			Efficiently manage students, exams, fees, and more with our comprehensive system.
		</p>
		<button on:click={()=>goto("/start")}
			class="bg-blue-500 hover:bg-blue-600 text-white font-semibold py-2 sm:py-3 px-4 sm:px-6 rounded-full shadow-lg transition duration-300"
			>Get Started</button
		>
	</div>
</section>
