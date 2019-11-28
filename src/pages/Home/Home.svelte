<script>
  import Flex from "../../components/Flex/Flex.svelte"
  import MissingItems from "../../components/MissingItems/MissingItems.svelte"
  let isFull = true
</script>
<style>
  div {
    margin-top: 20px;
  }
  h3 {
    text-align: center
  }
  span {
    margin-top: 30px;
    width: 100%;
  }
</style>
<div>
  <Flex alignItemsCenter directionColumn>
    {#if isFull}
      <img src="images/full.png" alt="full of ingredients"/>
      <h3>Greate, you have all you need. Let's cook</h3>
    {:else}
      <h3>You should go to de market</h3>
      <span>
        <MissingItems class="missing"/>
      </span>
    {/if}
  </Flex>
</div>