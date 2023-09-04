<script>
    import { onMount } from "svelte";
    import { tweened } from "svelte/motion";
    import { get_current_component } from "svelte/internal";
    var direction_move = tweened(200);
    var direcrion = "right";
    var bottom = tweened(200); 
    const me = get_current_component();
    var emojis = ["/emoji/dollar.png","/emoji/party_face.png","/emoji/cake.png"];
    var randomIndex = Math.floor(Math.random() * emojis.length); 
    onMount(()=>{
        direcrion = Math.random() < 0.5 ? "right" : "left";
        bottom = Math.random() < 0.5 ? tweened(100) : tweened(500);
        bottom.set($bottom+100,{duration:200});
        bottom.set($bottom,{delay:200,duration:300});
        direction_move.set(-750,{duration:1000}); 
        bottom.set(-500,{delay:500,duration:1000}).then(()=>{
            me.$destroy();
        });
    })
</script>

<img src={emojis[randomIndex]} class="absolute w-40 z-10" style="{direcrion}: {$direction_move}px; bottom: {$bottom}px;" />