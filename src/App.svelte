<script>
  import PlanPlaceholder from "./Components/PlanPlaceholder/PlanPlaceholder.svelte";
  import Sign from "./Components/Sign.svelte";
</script>

<main>
  <h1>text-quest</h1>
  <PlanPlaceholder />
</main>
<Sign />

<style>
  main {
    padding: 1em;
    margin: 0 auto;
  }

  h1 {
    text-align: center;
    color: #ff3e00;
    font-size: 4em;
    font-weight: 100;
    margin: 0.7em 0;
  }
</style>
