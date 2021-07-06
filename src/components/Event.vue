<template>
    <div class="event">
    <h3>{{event.text}}</h3>
    <p>{{event.day}}</p>
    <p>{{event.location}}</p>
    </div>
</template>

<script>
export default {
    name: 'Event',
    props: {
        task: Object
    }
}
</script>


<style>
.event {
    background: #f4f4f4;
    margin: 5px;
    padding: 10px 20px;
    cursor: pointer;
}

.event.reminder {
    border-left: 5px solid black;
}

.event h3 {
    display: flex;
    align-items: center;
    justify-content: space-between;
}
</style>