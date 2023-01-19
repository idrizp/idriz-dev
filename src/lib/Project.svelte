<script lang="ts">
  export let title: string;
  export let technologies: string[];
</script>

<li>
  <details open>
    <summary class="font-bold text-xl">{title}</summary>
    <div class="pl-3">
      <slot />
      <p>Technologies used:</p>
      <ol class="list-disc list-inside pl-5">
        {#each technologies as technology}
          <li>{technology}</li>
        {/each}
      </ol>
    </div>
  </details>
</li>
