<script>
  let gridObjects = [1, 2, 3, 4];
</script>

<div class="container">
  {#each gridObjects as gridObject}
    <div class="card">
      {gridObject}
    </div>
  {/each}
</div>

<style>
  .container {
    background-color: rgba(35, 114, 241, 0.4);
    display: grid;
    grid-template-columns: repeat(3, 33% [card]);
  }
  .card {
    border-style: dashed;
    border-width: 3px;
    border-color: red;
  }
</style>
