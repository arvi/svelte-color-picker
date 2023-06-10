<script lang="ts">
  import ColorRGBToHex from './ColorRGBToHex.svelte';

  export let redValue: number;
  export let greenValue: number;
  export let blueValue: number;
</script>
<div class="row">
  <div id="color-preview" class="column" style="background-color: rgb({redValue}, {greenValue}, {blueValue});">&nbsp;</div>
</div>
<div class="row">
  <div class="column"><h3><span>rgb({redValue}, {greenValue}, {blueValue})</span> | <ColorRGBToHex {redValue} {greenValue} {blueValue} /></h3></div>
</div>


<style>
  #color-preview {
    border: 3px dashed #eee;
    min-height: 200px;
    min-width: 300px;
    margin: 10px;
  }
  h3 {
    text-align: center;
  }
</style>
