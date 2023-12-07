<script>
  import Greeting  from "../components/Greeting.svelte";
  import Button from "../components/Button.svelte";
  import Count from "../components/Count.svelte";
  import List from "../components/List.svelte";
  let name = "太郎"
</script>

<h1>Hello, {name}</h1>
<input bind:value={name} />
<Greeting name={name} />
<div class="row">
  <Button />
  <Count />
</div>
<List />

<style>
  .row {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: flex-start;
    gap: 5px;
  }
</style>