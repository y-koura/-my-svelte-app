<script>
  import Greeting from "./Greeting.svelte";
  let users = [
    { id: 1, name: '太郎', age: 20 },
    { id: 2, name: '花子', age: 18 },
    { id: 3, name: '次郎', age: 25 },
  ];
</script>

<ul>
  {#each users as user, i}
  <li><Greeting name={user.name} />年齢{user.age}</li>
  {/each}
</ul>