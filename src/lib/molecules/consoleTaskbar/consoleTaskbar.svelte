<script>
    import ConsoleDot from "../../atoms/consoleDot/consoleDot.svelte";
</script>

<style>
    @import './consoleTaskbar.css';
</style>

<div id = "console-taskbar">
    <div class="dot-wrapper">
        <ConsoleDot color = "red" />
        <ConsoleDot color = "yellow" />
        <ConsoleDot color = "green" />
    </div>
</div>