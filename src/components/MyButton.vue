<script>
export default {
  props: {
    text: Number,
    myButtonAction: Function
  },
}

</script>

<template>
  <button @mouseover="myButtonAction">{{  text }}</button>
</template>

<style scoped>
  * {
    font-size: 40px;
  }
</style>
