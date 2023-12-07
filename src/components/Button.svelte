<script>
  let text = 'click me'
  function handleClick() {
    text = 'clicked'
  }
</script>

<button on:click={handleClick}>
  {text}
 </button>