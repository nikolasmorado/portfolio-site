<script>
    import NavLink from "../../atoms/navLink/navLink.svelte";

    export let focused = 1;
    export let sections = [];
</script>

<style>
    @import "navbar.css";
</style>

<!-- <NavLink text = "/~" isFocused = {true} />
<NavLink text = "/contact"/>
<NavLink text = "/experience"/>
<NavLink text = "/education"/> -->

{#each sections as sec, i}
    {#if i == focused}
        <NavLink text = {sec} isFocused = {true} />
    {:else}
        <NavLink text = {sec} />
    {/if}
{/each}