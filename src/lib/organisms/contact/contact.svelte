<script>
    import ConsoleLine from "../../atoms/consoleLine/consoleLine.svelte";
</script>

<style>
    @import './contact.css';
</style>

<div class = "terminal">
    <ConsoleLine text = {"~/info/contact-information"} color = {"blue"} isDir = {true}/>
    <div>
        <ConsoleLine text = {"> "} color={"white"} /> <ConsoleLine text = {"cat info.txt"} color = {"green"} />
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
        <ConsoleLine text = {"> "} color = {"white"}/>
    </div>
</div>