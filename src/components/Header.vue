<template>
  <header>
    <h1>{{ title }}</h1>
    <Button text="Add Event" color="green" />
    <Button text="Update Event" color="blue" />
    <Button text="Delete Event" color="red" />
  </header>
</template>

<script>
import Button from "./Button";

export default {
  name: "Header",
  props: {
    title: String,
  },
  component: {
    Button,
  },
};
</script>

<style scoped>
header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin-bottom: 20px;
}
</style>
