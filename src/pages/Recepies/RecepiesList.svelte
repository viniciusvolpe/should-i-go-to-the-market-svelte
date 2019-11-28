<script>
  export let recepies = [];
</script>

<style>
  /* your styles go here */
</style>

<table>
  <thead>
    <tr>
      <th>Name</th>
      <th>Time</th>
      <th>Items</th>
      <th>Method</th>
    </tr>
  </thead>

  <tbody>
    {#each recepies as recipe}
      <tr>
        <td>{recipe.name}</td>
        <td>{recipe.time}</td>
        <td>{recipe.items}</td>
        <td>{recipe.method}</td>
      </tr>
    {/each}
  </tbody>
</table>