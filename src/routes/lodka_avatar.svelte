
<script>
    import EmojiFall from "./emoji_fall.svelte";

    function add_emoji(){
        new EmojiFall({target:emojis_container})
    }
    var emojis_container;  
</script>

<div class="h-full aspect-square relative">
    <div bind:this={emojis_container}>
 
    </div> 
    <button 
        on:click={add_emoji}
        class="w-full h-full relative z-10  object-cover bg-cover  active:scale-75 transition-transform"
        style="background-image: url(/lodka_avatar.png); "
    /> 
</div>