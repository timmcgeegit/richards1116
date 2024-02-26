<script>
    // State to manage theme
    let isDark = false;
  
    // Function to toggle theme mode
    function toggleTheme() {
      isDark = !isDark;
      document.documentElement.classList.toggle('dark', isDark);
    }
  </script>
  
  <header class="bg-gray-200 dark:bg-gray-800 text-gray-800 dark:text-gray-200 p-4">
    <div class="container mx-auto flex justify-between items-center">
      <h1 class="text-xl font-bold">My Svelte Site</h1>
      <nav>
        <ul class="flex space-x-4">
          <li><a href="/" class="hover:underline">Home</a></li>
          <li><a href="/about" class="hover:underline">About</a></li>
          <li><a href="/contact" class="hover:underline">Contact</a></li>
        </ul>
      </nav>
      <button class="bg-gray-300 dark:bg-gray-700 p-2 rounded" on:click={toggleTheme}>
        {#if isDark}🌞{#else}🌜{/if}
      </button>
    </div>
  </header>