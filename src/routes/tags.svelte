<script>
    import { onMount } from "svelte";
    import TagsData from "./tags_data.svelte";
    var scroll_container;
    let animationInterval;
    var width = 0;
    onMount(() => {
        const tags = new TagsData({target:scroll_container});
        new TagsData({target:scroll_container});
        width = tags.width;
        scroll_container.scrollLeft = scroll_container.scrollWidth;
        moveLeft();
    });

    function moveLeft() {
        
        clearInterval(animationInterval);
        animationInterval = setInterval(frame, 60); // 60 frames per second
    }

    function frame() {
        if (scroll_container.scrollLeft === 0) {
            scroll_container.scrollLeft =  width+80;
        } else {
            scroll_container.scrollLeft -= 1;
        }
    }
</script>

<div
    bind:this={scroll_container}
    class="flex flex-row gap-20 w-full overflow-hidden"
>
 
</div>
