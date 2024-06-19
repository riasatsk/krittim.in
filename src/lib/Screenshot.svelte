<script>
  // Array of screenshot details
  const screenshots = [
    { title: 'Home Page', src: '/home.png' },
    { title: 'Student Page', src: '/student.png' },
    { title: 'Exam Page', src: '/exam.png' },
    { title: 'Fees Page', src: '/fees.png' }
  ];
</script>

<section class="bg-gray-50 py-20">
  <div class="max-w-6xl mx-auto px-4 sm:px-6 lg:px-8">
    <h2 class="text-3xl font-bold text-center mb-12">Explore Our Features</h2>
    <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 gap-8">
      {#each screenshots as { title, src }}
        <div class="bg-white rounded-lg shadow-lg overflow-hidden">
          <img class="w-full h-48 object-cover" {src} alt={title} />
          <div class="p-4">
            <h3 class="text-xl font-semibold">{title}</h3>
          </div>
        </div>
      {/each}
    </div>
    <div class="text-center mt-12">
      <a href="screenshots" class="bg-blue-500 hover:bg-blue-600 text-white font-semibold py-2 px-6 rounded-full shadow-lg transition duration-300">
        More Screenshots
      </a>
    </div>
  </div>
</section>
