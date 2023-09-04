<script>
    import "../app.css";
    import CoolText from "$lib/cool_text.svelte";
    import { onMount } from "svelte";
    import {scroll_top} from "$lib/app.js"
 
    onMount(async () => {
        page.addEventListener("scroll", (event) => {
            $scroll_top = page.scrollTop;
        });
    });
    var page;
</script>

<svelte:head>
    <title>Лодка.com</title>
    <meta property="theme-color" content="#ff005c">
    <meta name="description" content="открытка от Andreu333XD для лодочника" />
    <meta property="og:image" content="/lodka_avatar.png" />
</svelte:head>

<div
    bind:this={page}
    class="w-full h-screen bg-black overflow-y-auto overflow-x-hidden"
>
    <div
        class="border-b-2 border-white flex justify-center items-center gap-16"
    >
        <CoolText text={"lodka"} />
        <CoolText text={"lodka"} />
        <CoolText text={"lodka"} />
    </div>
    <slot />
    <div class="border-t-2 border-white h-screen flex flex-row justify-center items-center gap-6">
        <img src="https://media.discordapp.net/attachments/807809192537882647/1079901194954219670/IMG_6446.gif"/>
        <p 
            style="font-family: ClashDisplay-SemiBold; font-size: 28px; ">
            Ot Andreu333XD dla Igor(lodka, lodo4nik,lybertsy)
            <br/> happy birth!!
        </p>
    </div>
</div>  