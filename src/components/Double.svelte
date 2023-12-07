<script>
  import { count } from "../lib/store";
  $: double = $count * 2;
</script>

<p>Double: {double}</p>