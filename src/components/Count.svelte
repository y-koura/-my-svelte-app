<script>
  import { count } from "../lib/store";
  import Double from "./Double.svelte";
  function increment() {
    $count +=1;
  }
</script>

<div class="count">
  <p>Count UP!</p>
  <button on:click={increment}>
    {$count}
  </button>
</div>
<Double />

<style>
  .count {
    display: flex;
    flex-direction: row;
    justify-content: center;
    align-items: center;
    gap: 5px;
  }
</style>