<template>
  <svgicon
    :name="glass"
    class="w-12 h-12 mr-2 stroke-current text-grey-dark"
  ></svgicon>
</template>

<script>
export default {
  props: {
    glass: String,
  },
  mounted() {
    import(
      /* webpackChunkName: "svgicon-glass" */ `@/components/icons/${this.glass}`
    )
  },
}
</script>

<style>
.svg-icon [pid='0'] {
  fill: none;
  stroke-width: 3;
  stroke-linecap: round;
  stroke-linejoin: round;
  stroke-miterlimit: 10;
}
.svg-icon [pid='1'] {
  fill: none;
  stroke-width: 2;
  stroke-linecap: round;
  stroke-linejoin: round;
  stroke-miterlimit: 10;
}
</style>
