<script>
  export default {
    data() {
      return {
        text: '',
        words: []
      }
    },
    methods: {
      cut: function () {
        this.words = this.text.split(' ')
      }
    }
  }
</script>

<template>
  <textarea v-model="text"></textarea>
  <button @click="cut">Разрезать</button>
  <ul>
    <li v-for="word in words">{{ word }}</li>
  </ul>
</template>

<style scoped>

</style>