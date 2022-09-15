<script>
    export let text;
    export let isFocused = false;
</script>

<style>
    @import "navLink.css";
</style>

{#if isFocused}
    <div class = "navLinkFocused">
        <span>
            {text}
        </span>
    </div>
{:else}
    <div class = "navLink">
        <span>
            {text}
        </span>
    </div>
{/if}