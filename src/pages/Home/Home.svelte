<script>
  import Flex from "../../components/Flex/Flex.svelte"
  let isFull = true
</script>
<style>
  div {
    margin-top: 20px;
  }
  h3 {
    text-align: center
  }
</style>
<div>
  <Flex alignItemsCenter directionColumn class="container">
    {#if isFull}
      <img src="images/full.png" alt="full of ingredients"/>
      <h3>Greate, you have all you need. Let's cook</h3>
    {/if}
  </Flex>
</div>