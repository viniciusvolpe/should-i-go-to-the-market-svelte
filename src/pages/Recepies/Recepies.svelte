<script>
  import Flex from "../../components/Flex/Flex.svelte"
  import RecepiesList from "./RecepiesList.svelte";
  let recepies = [];
</script>
<style>
  h3 {
    text-align: center;
  }
  span {
    margin-top: 30px;
    width: 100%;
  }
</style>
<Flex alignItemsCenter directionColumn>
  <h3>Recepies</h3>
  <span>
    <RecepiesList recepies={recepies} />
  </span>
</Flex>