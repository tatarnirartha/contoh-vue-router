<template>
  <div style="margin: 5rem" class="text-center">
    <router-link to="/about">Router Link</router-link>
    <br>
    <button @click="pushClick">Push</button>
    <br>
    <button @click="replaceClick">Replace</button>
    <br>
    <button @click="goClick">Go</button>
  </div>
</template>

<script>
export default {
  methods: {
    pushClick(){
      this.$router.push({name: "home"})
    },
    replaceClick(){
      this.$router.replace({name: "home"})
    },
    goClick(){
      this.$router.go(-1)
    }
  }
}
</script>