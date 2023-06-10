<script lang="ts">
  export let redValue: number;
  export let greenValue: number;
  export let blueValue: number;
</script>
<div class="row">
  <div id="color-preview" class="column" style="background-color: rgb({redValue}, {greenValue}, {blueValue});">&nbsp;</div>
</div>
<div class="row">
  <div class="column"><h3>rgb({redValue}, {greenValue}, {blueValue})</h3></div>
</div>
<style>
  #color-preview {
    min-height: 200px;
    min-width: 300px;
    margin: 10px;
  }
  h3 {
    text-align: center;
  }
</style>