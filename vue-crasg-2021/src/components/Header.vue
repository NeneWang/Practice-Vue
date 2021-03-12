<template>
  <header>
    <h1>{{title}}</h1>
    <Button />
  </header>
</template>

<script>
import Button from './Button'

export default {
  name: "Header",
  props: {
      title: {
          type: String,
          default: "Hello World"
      },
  },
  components: Button,
};
</script>

<style scoped>
Header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin-bottom: 20px;
}
</style>
