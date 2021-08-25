<template>
  <h1>Class Card</h1>
</template>

<script>
import axios from 'axios'
import { onMounted } from 'vue'

export default {
  setup () {
    // Mounted
    onMounted(() => {
      axios
        .get('http://localhost:8000/classes/')
        .then(res => console.log('this is the response ', res))
    })
  },

}
</script>

<style>
</style>
