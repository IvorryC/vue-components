<template>
  <div class="container">
  <Header title="Events" />
  <Event :events="event" />
  </div>
</template>

<script>
import Header from './components/Header.vue' 
import Events from './components/Events.vue'

export default {
  name: 'App',
  component: {
    Header,
    Events,
  },
  data() {
    return {
      events: []
    }
  },
  created() {
    this.Events = [
      {
        id: 1,
        text: 'Modest Mouse',
        day: 'March 1st at 2:00pm',
        location: 'Red Rocks',
        reminder: true,
      },
      {
        id: 2,
        text: 'Built to Spill',
        day: 'March 3rd at 3:00pm',
        location: 'The Ogden',
        reminder: true,
      },
      {
        id: 3,
        text: 'Faith No More',
        day: 'March 1st at 12:00pm',
        location: 'St Louis',
        reminder: false,
      },
    ]
  }

}
</script>

<style>

* {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}

body {
  font-family: "Helvetica", sans-serif;
}

.container {
  max-width: 500px;
  margin: 30px auto;
  overflow: auto;
  min-height: 300px;
  border: 1px solid steelblue;
  padding: 30 px;
  border-radius: 5px;
}

.btn {
  display: inline-block;
  background: #000;
  border: none;
  color: #fff;
  padding: 10px 20px;
  margin: 5px;
  border-radius: 5px;
  cursor: pointer;
  text-decoration: none;
  font-size: 15px;
  font-family: inherit;
}

.btn:focus {
  outline: none;
}

.btn:active {
  transform: scale(0.98);
}

.btn-block {
  display: block;
  width: 100%;
}

</style>