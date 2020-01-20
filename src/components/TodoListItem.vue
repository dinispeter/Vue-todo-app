<template>
  <li>
    {{ todo.text }}
    <button class="remove-button"
    @click="$emit('remove', todo.id)">
      X
    </button>
  </li>
</template>

<script>
export default {
  props: {
    todo: {
      type: Object,
      required: true
    }
  }
}
</script>

<style scoped>
  .remove-button {
    color: white;
    width: 25px;
    height: 25px;
    background-color: red
  }
</style>
