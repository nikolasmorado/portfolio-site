<script>
    import NavLink from "../../atoms/navLink/navLink.svelte";
    import {onMount} from 'svelte'

    export let focused = 0;
    export let sections = [];

    let y, yMax = 0;

    onMount(() => {
        setTimeout(() => {yMax = document.documentElement.scrollHeight - document.documentElement.clientHeight}, 0)
    })

    const findFocus = (val, max) => {
        console.log({val, max})
        let tper = val / max;
        if
            (tper >= 0 && tper <= 0.15)  return 0
        else if
            (tper > 0.15 && tper <= 0.5) return 1
        else if
            (tper > 0.5 && tper <= 0.75) return 2
        else if
            (tper > 0.75 && tper <= 1)   return 3
    }

    $ : focused = findFocus(y, yMax)
</script>

<style>
    @import "navbar.css";
</style>

<svelte:window bind:scrollY={y}/>

{#each sections as sec, i}
    {#if i == focused}
        <NavLink text = {sec} isFocused = {true} />
    {:else}
        <NavLink text = {sec} />
    {/if}
{/each}