<template>
  <div>
<!--    <input type="text" :value="keywordValue" @input="$emit('input', $event.target.value)">-->
    <input type="text" :value="value" @input="$emit('input', $event.target.value)">

    <button>search</button>
  </div>
</template>

<script>
export default {
  /* props: {
    keywordValue: {
      type: String,
      default: () => '',
    },
  }, */
  props: {
    value: {
      type: String,
      default: () => '',
    },
  },
}
</script>

<style scoped>

</style>
