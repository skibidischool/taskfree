<script lang="ts">
    let { name } = $props();
    let checked: boolean = $state(false);

    function completeTask() {
        checked = !checked;
    }
</script>

<p>
    {name}
    <button onclick={completeTask}>
        {#if checked}
            Done
        {:else}
            Not Done
        {/if}
    </button>
</p>