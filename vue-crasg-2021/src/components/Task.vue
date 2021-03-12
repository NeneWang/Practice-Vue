<template>
    <div class="task">
        <h3>{{task.text}}</h3>
    </div>
</template>


<script>
import Task from './Task'
export default {
    name: "Task",
    props: {
        task: Object,
    },
}
</script>