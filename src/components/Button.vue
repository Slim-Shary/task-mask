<template>
  <button @click="onClick()" :style="{ background: color }" class="btn outline">
    {{ text }}
  </button>
</template>

<script>
export default {
  name: 'Button',
  props: {
    text: String,
    color: String
  },
  methods: {
    onClick() {
      console.log('pushed button')
    }
  }
}
</script>

<style scoped>
.btn {
  border: 2px solid black;
  color: black;
  cursor: pointer;
}
.outline {
  border-color: #4caf50;
  color: green;
}
</style>
