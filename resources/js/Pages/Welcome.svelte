<script>
  import Layout from "./Layout.svelte";
  import Button from "../Components/Button.svelte";
  import DocsCard from "../Components/DocsCard.svelte";

  export let counter;

  function increment() {
    counter ++;
  }
</script>

<Layout>
  <section class="flex justify-center items-center flex-col min-h-screen">
    <h1 class="text-3xl uppercase font-bold mb-2">Welcome to <span class="bg-gradient-to-r from-purple-700 to-orange-500 bg-clip-text text-transparent">Laravelte</span></h1>
    <p class="mb-5">Hello World!</p>
    <p class="mb-5">This is a simple <span class="text-purple-400">Laravel</span> project already configured with <span class="text-orange-400">Svelte</span> (InertiaJS) and <span class="text-cyan-400">DaisyUI</span> (tailwindcss).</p>
    <Button text="Counter is {counter}" onClick={increment}/>
    <div class="grid grid-cols-12 gap-4 mt-10">
      <div class="col-span-6">
        <DocsCard title="Laravel Docs" text="If you are new to Laravel ou need some memory refresh, here are the docs" href="https://laravel.com/docs"/>
      </div>
      <div class="col-span-6">
        <DocsCard title="DaisyUI Docs" text="Here are the DaisyUI documentation so you can start creating your UIs" href="https://daisyui.com/docs/use/"/>
      </div>
    </div>
  </section>
</Layout>