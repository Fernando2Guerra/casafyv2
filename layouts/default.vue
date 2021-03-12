<template>
    <nuxt />
</template>


<script>

  export default {
    components: {
    },
    head(){
      return {
        title: "Casafy - Sua próxima experiência para encontrar as melhores casas e apartamentos para você morar"
      }
    },
    mounted(){
      this.$nextTick(() => {
        this.$nuxt.$loading.start()
        setTimeout(() => this.$nuxt.$loading.finish(), 500)
      })
    }
  }
</script>

<style>
</style>
