<script>
  import tasks from "./plan.json";
</script>

<section>
  <h2>Разработка в процессе...</h2>
  <h3>План:</h3>
  <ul>
    {#each tasks as { done, icon, text } (text)}
      <li><span class="icon" class:done>{icon}</span> {text}</li>
    {/each}
  </ul>
</section>

<style>
  section {
    max-width: 600px;
    text-align: left;
    margin: 3em auto;
  }
  li .icon {
    filter: grayscale(100%);
    opacity: 0.2;
    margin-right: 0.3em;
    width: 1.3em;
    display: inline-block;
  }
  li .icon.done {
    opacity: 1;
    filter: none;
  }
  li:hover .icon {
    filter: none;
    opacity: 0.4;
  }
</style>
