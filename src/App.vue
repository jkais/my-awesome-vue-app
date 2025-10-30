<script>
import MyButton from './components/MyButton.vue';
export default {
  components:{ MyButton },
  data() {
    return {
      counter: 0,
    }
  },
  methods: {
    increase() { this.counter++ },
    decrease() { this.counter-- },
    reset() { this.counter = 0 },
  }
}

</script>

<template>
  <div>
    {{ counter }}
  </div>
  <MyButton text="-" :my-button-action="decrease"/>
  <MyButton :text="2 * 5" :my-button-action="reset"/>
  <MyButton text="+" @click="increase"/>
</template>

<style scoped>
  * {
    color: red;
  }
</style>
