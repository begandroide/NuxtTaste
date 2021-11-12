
<template>
  <div class="relative flex items-center justify-center bg-gray-100 pt-4">
    <h2 class="text-2xl leading-7 font-semibold">{{counter}}</h2>
    <button
      class="absolute top-0 right-0 m-4 text-gray-500 hover:text-gray-700 focus:outline-none focus:text-gray-700"
      @click="plusOne"
    ></button>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'
export default Vue.extend({
  data() {
    return {
      counter: 0
    }
  },
  methods: {
    plusOne() {
      this.counter++
    }
  }
})
</script>
