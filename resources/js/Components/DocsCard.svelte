<script>
  export let title;
  export let text;
  export let href;
</script>

<div class="card bg-base-100 min-h-full">
  <div class="card-body">
    <h2 class="card-title">{title}</h2>
    <p>{text}</p>
    <div class="card-actions justify-end">
      <a class="btn btn-primary" href={href}>Go to Docs</a>
    </div>
  </div>
</div>