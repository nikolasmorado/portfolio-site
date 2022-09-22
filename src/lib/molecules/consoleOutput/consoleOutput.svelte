<script>
    import ConsoleCursor from "../../atoms/consoleCursor/consoleCursor.svelte";
    import ConsoleLine from "../../atoms/consoleLine/consoleLine.svelte";
</script>

<style>
    @import 'consoleOutput.css';
</style>

<ConsoleLine text = {"~/info/contact-information"} color = {"blue"} isDir = {true}/>
<div>
    <ConsoleLine text = {"> "} color={"white"} />
    <ConsoleLine text = {"cat info.txt"} color = {"green"} />
</div>
<div class = "cmd-res">
    <ConsoleLine text = {"phone: +1 2899435305"} color = {"white"} />
    <br />
    <ConsoleLine text = {"email: nikolasmorado@gmail.com"} color = {"white"} />
    <br />
    <ConsoleLine text = {"github: /nikolasmorado"} color = {"white"} />
</div>
<div class = "new-cmd">
    <ConsoleLine text = {"~/info/contact-information"} color = {"blue"} isDir = {true}/>
    <br />
    <div class = "entry-line">
        <ConsoleLine text = {"> "} color = {"white"}/>
        <ConsoleCursor />
    </div>
</div>