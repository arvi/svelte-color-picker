<script lang="ts">
    export let color: 'red' | 'green' | 'blue';
    export let colorValue: number;
</script>
<label for="{color}">{color} ({colorValue})</label>
<input type="range" class="color-slider" name="{color}" bind:value="{colorValue}" min="0" max="255">



<style>
    label::first-letter {
        text-transform:capitalize;
    }
    .color-slider {
        width: 100% !important;
        margin: 5px 0 20px 0;
    }
</style>
