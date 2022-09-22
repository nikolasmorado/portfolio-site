<script>
    export let text;
    export let isFocused = false;
    let cClass;

    if(isFocused) cClass = "navLinkFocused"
    else cClass = "navLink"

</script>

<style>
    @import "navLink.css";
</style>

<span class = {cClass}>
    {text}
</span>