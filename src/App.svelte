<script lang="ts">
    import Task from "./lib/Task.svelte";
    let tasks = [];

    function newTask() {
        tasks.push("dude")
    }
</script>

<button onclick={newTask}>New Task</button>
<input id="newtask">