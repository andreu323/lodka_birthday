<script>
    import { onMount } from "svelte";
    export var text = "";
    export var color ="white";
    var height = 0;
 
    setInterval(() => {
        if(object)height = object.getBoundingClientRect().height;
    }, 200);
    var object;
</script>

<div style="height: {height}px;" class="flex items-center max-w-full ">
    <p 
        class="w-full"
        style="scale: 1 0.5; font-family: ClashDisplay-SemiBold; font-size: 328px; color: {color};"
        bind:this={object}
    >
        {text}        
    </p>
    
</div>
