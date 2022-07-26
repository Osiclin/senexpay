<template>
  <button class="button" :style="{ background: bgcolor, color: color, borderRadius: radius }">
    <slot/>
  </button>
</template>

<script>
export default {
    name: "NuxtButton",
    props: ['bgcolor', 'color', 'radius']
}
</script>

<style scoped>
.button{
    border: 0;
    font-size: 1.5rem;
    margin-right: .5rem;
    padding: .8rem 2rem;
    display: flex;
    align-items: center;
    cursor: pointer;
}
</style>