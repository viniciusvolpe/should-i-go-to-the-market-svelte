<script>
  let missingItems = [
    {name: "Potato", recipe: "mashed potatoes", quantity: 5}
  ]
</script>

<table>
  <thead>
    <tr>
      <th>Name</th>
      <th>Recipe</th>
      <th>Quantity</th>
    </tr>
  </thead>

  <tbody>
    {#each missingItems as item}
      <tr>
        <td>{item.name}</td>
        <td>{item.recipe}</td>
        <td>{item.quantity}</td>
      </tr>
    {/each}
  </tbody>
</table>
