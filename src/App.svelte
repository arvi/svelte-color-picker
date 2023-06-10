<script lang="ts">
  import ColorPicker from './lib/ColorPicker.svelte'
  import ColorPreview from './lib/ColorPreview.svelte'

  let redValue = 126;
  let greenValue = 65;
  let blueValue = 0;
</script>

<div class="row">
  <div class="column">
    <h1>Color Picker</h1>
    <ColorPicker color="red" bind:colorValue="{redValue}" />
    <ColorPicker color="green" bind:colorValue="{greenValue}" />
    <ColorPicker color="blue" bind:colorValue="{blueValue}" />
  </div>
</div>
<ColorPreview {redValue} {greenValue} {blueValue}/>
<style>
  h1 {
    margin-top: 25px;
  }
</style>
