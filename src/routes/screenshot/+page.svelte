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
				<img
					src={screenshot}
					alt="Screenshot"
					class="w-full h-auto"
					on:click={() => {
						const modal = document.getElementById('modal');
						modal.show();
					}}
				/>
			</div>
		{/each}
	</div>
</div>

<!-- You can open the modal using ID.showModal() method -->

<dialog id="modal" class="modal">
	<div class="modal-box w-11/12 max-w-5xl">
		<div class="carousel w-full">
			{#each screenshots as screenshot, i}
				<div id="slide{i}" class="carousel-item relative w-full">
					<img src={screenshot} alt="screenshot" class="w-full" />
					<div
						class="absolute flex justify-between transform -translate-y-1/2 left-5 right-5 top-1/2"
					>
						<a href="#slide{i}" class="btn btn-circle">❮</a>
						<a href="#slide{i + 1}" class="btn btn-circle">❯</a>
					</div>
				</div>
			{/each}
		</div>
		<div class="modal-action">
			<form method="dialog">
				<!-- if there is a button, it will close the modal -->
				<button class="btn">Close</button>
			</form>
		</div>
	</div>
</dialog>

<style>
	/* Optional: You can add custom styling here */
</style>
