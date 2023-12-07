<script>
  export let name = '太郎';
</script>

{#if name === '太郎'}
  <p>太郎さん、こんにちは！</p>
{:else if name === '花子'}
  <p>花子さん、こんにちは！</p>
{:else}
  <p>{name}さん、こんにちは！</p>
{/if}