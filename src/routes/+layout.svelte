<script>
  import { browser } from "$app/environment";
  import "../app.css";
  let dark = true;
  $: browser ? updateDarkMode() : {};

  function updateDarkMode() {
    const html = document.querySelector("html");
    console.log("hi");
    if (html) {
      html.classList.toggle("dark", dark);
    }
  }
  function toggleDarkMode() {
    dark = !dark;
    updateDarkMode();
  }
</script>

<button
  class="absolute bg-black text-white dark:bg-white dark:text-black px-5 text-2xl rounded-full p-2 m-5 right-0"
  class:dark
  on:click={toggleDarkMode}
>
  {#if !dark}
    ☽
  {:else}
    ☼
  {/if}
</button>
<slot />
