<script lang="ts">
  export let redValue: number;
  export let greenValue: number;
  export let blueValue: number;

  $: hexColor = rgbToHex(redValue, greenValue, blueValue);
  
  
  function rgbToHex(r: number, g: number, b: number): string {
    const toHex = (value: number): string => {
        const hex = value.toString(16);
        return hex.length === 1 ? `0${hex}` : hex;
    };

    const hexR = toHex(r);
    const hexG = toHex(g);
    const hexB = toHex(b);

    return `#${hexR}${hexG}${hexB}`;
    }
</script>

<span>HEX: {hexColor}</span>