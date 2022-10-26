<script>
  import Connect from "../dialogs/connect.svelte";

  let open = false;
</script>

<nav
  class="flex space-x-4 h-[75px] bg-secondary text-secondary-content flex items-center"
>
  <a class="btn btn-ghost" href="/">Home</a>
  <a class="btn btn-ghost" href="/about">About</a>
</nav>
<main>
  <section class="hero min-h-screen bg-base-100">
    <div class="hero-content flex-col">
      <h1 class="text-8xl font-bold">⚡️HypAR⚡️</h1>
      <p>The Ultimate Permaweb Stack!</p>
      <button class="btn" on:click={() => (open = true)}>Open Modal</button>
    </div>
  </section>
</main>
<Connect bind:open />
