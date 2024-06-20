<!-- ScreenshotPage.svelte -->

<script>
	// Define an array of screenshot image URLs
	const screenshots = [
		'/home.png',
		'/class.png',
		'/student.png',
		'/add-student.png',
		'/fees.png',
		'/add-fees.png',
		'/exam.png',
		'/marksheet.png',
		'/marksheet-example.png',
		'/fees-example.png',
		'/school.png',
		'/update.png',
		'/theme.png',
		'/edit-mark.png',
		'/list.png'

		// Add more screenshot images as needed
	];
</script>

<div class="navbar bg-base-100">
	<div class="flex-1">
		<a class="btn btn-ghost text-xl" href="/">Krittim</a>
	</div>
	<div class="flex-none">
		<button class="btn btn-square btn-ghost">
			<svg
				xmlns="http://www.w3.org/2000/svg"
				fill="none"
				viewBox="0 0 24 24"
				class="inline-block w-5 h-5 stroke-current"
				><path
					stroke-linecap="round"
					stroke-linejoin="round"
					stroke-width="2"
					d="M5 12h.01M12 12h.01M19 12h.01M6 12a1 1 0 11-2 0 1 1 0 012 0zm7 0a1 1 0 11-2 0 1 1 0 012 0zm7 0a1 1 0 11-2 0 1 1 0 012 0z"
				></path></svg
			>
		</button>
	</div>
</div>
<div class="container mx-auto py-8">
	<div class="font-bold text-2xl m-5">More Screenshots</div>
	<div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 gap-8 m-5">
		{#each screenshots as screenshot}
			<div class="overflow-hidden bg-white rounded-lg shadow-md">
				<img src={screenshot} alt="Screenshot" class="w-full h-auto" />
			</div>
		{/each}
	</div>
</div>
