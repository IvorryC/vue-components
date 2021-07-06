<template>
  <div v-for="event in events" :key="event.id">
    <Event :event="event" />
  </div>
</template>

<script>
import Event from "./Event.vue";

export default {
  name: "Events",
  props: {
    events: Array,
  },
  component: {
    Event,
  },
};
</script>