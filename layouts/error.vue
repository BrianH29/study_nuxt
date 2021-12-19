<template>
  <div>
    <h1 v-if="error.statusCode === 404">PAGE NOT FOUND {{ error.statusCode }}</h1>
    <h1 v-else>An Occured</h1>

    <NuxtLink to="/">Home Page</NuxtLink>
  </div>
</template>

<script>
export default {
  props: {
    error: {
      type: Object,
      default: () => {},
    },
  },
}
</script>

<style scoped>

</style>
