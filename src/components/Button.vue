<template>
  <button :style="{ background: color }" class="btn outline">
    {{ text }}
  </button>
</template>

<script>
export default {
  name: 'Button',
  props: {
    text: String,
    color: String
  }
}
</script>

<style scoped>
.btn {
  border: 2px solid black;
  color: black;
  cursor: pointer;
  border-radius: 50%;
}
.outline {
  border-color: #4caf50;
  color: green;
}
</style>
