<script>
    export let text;
    export let color = "white";
    export let isDir = false;
</script>

<style>
    @import './consoleLine.css';
</style>

<span class="consoleLine {isDir ? 'isDir' : ''}"  id = {color}>{text}</span>