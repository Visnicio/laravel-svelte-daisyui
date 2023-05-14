<script>
  import "../../css/app.css"
  import { inertia } from '@inertiajs/svelte'
</script>

<header class="navbar bg-base-100">
  <div class="py-3 container mx-auto flex justify-between items-center">
    <div use:inertia href="/" class="font-bold text-2xl bg-gradient-to-r from-purple-700 to-orange-500 bg-clip-text text-transparent">Laravelte</div>
    <div>
      <a href="https://github.com/Visnicio/laravel-svelte-tailwind" class="mr-2">Github</a>
    </div>
  </div>
</header>
<main class="bg-neutral">
  <slot />
</main>