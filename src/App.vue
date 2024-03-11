<script>
  import User from './components/User.vue'
  import Employee from "@/components/Employee.vue";

  export default {
    data() {
      return {

      }
    },
    methods: {
      func(arg1, arg2) {
        console.log(arg1, arg2)
      },
    },
    components: {
      User,
      Employee
    }
  }
</script>

<template>
  <User @show="func"/>
</template>

<style scoped>

</style>