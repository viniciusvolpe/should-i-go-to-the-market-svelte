<script>
  export let justifyContentCenter;
  export let directionColumn;
  export let alignItemsCenter;
</script>
<style>
  .container {
    display: flex;
  }
  .justifyContentCenter{
    justify-content: center
  }
  .directionColumn{
    flex-direction: column
  }
  .alignItemsCenter {
    align-items: center
  }
</style>
<div class="container" class:justifyContentCenter class:directionColumn class:alignItemsCenter>
  <slot></slot>
</div>

