<script>
  export let text;
  export let onClick;
</script>

<button on:click={onClick} class="btn btn-primary">
  {text}
</button>