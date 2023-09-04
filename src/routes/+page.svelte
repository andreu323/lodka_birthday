<script>
 
    import CoolText from "$lib/cool_text.svelte";
    import LodkaAvatar from "./lodka_avatar.svelte";
    import {scroll_top} from "$lib/app.js"
    import Tags from "./tags.svelte";
</script>
 
    <div
        class="border-b-2 py-40 border-white h-[1200px] w-full overflow-hidden relative flex justify-center"
    >
        <div
            class="absolute w-full h-full flex justify-center items-center rotate-12"
        >
            <svg
                xmlns="http://www.w3.org/2000/svg"
                id="b"
                viewBox="0 0 779.57 779.57"
                ><defs
                    ><style>
                        .d {
                            fill: none;
                            stroke: #fff;
                            stroke-miterlimit: 10;
                            stroke-width: 3px;
                        }
                    </style></defs
                ><g id="c"
                    ><polygon
                        class="d"
                        points="763.02 235.18 591.78 389.78 763.02 544.38 532.61 532.61 544.38 763.02 389.78 591.78 235.18 763.02 246.95 532.61 16.54 544.38 187.79 389.78 16.54 235.18 246.95 246.95 235.18 16.54 389.78 187.79 544.38 16.54 532.61 246.95 763.02 235.18"
                    /></g
                ></svg
            >
        </div>
        <div class="w-full h-full relative">
            <div
                class="absolute w-full h-full flex flex-row items-center justify-center"
                style="top: {$scroll_top - 400 >= 0 ? 0 : $scroll_top - 400}px;"
            >
                <img
                    draggable="false"
                    src="/cat_e.jpg"
                    class="h-full scale-75 aspect-square object-cover"
                />
                <LodkaAvatar />
                <img
                    draggable="false"
                    src="/cat_funny.jpg"
                    class="h-full scale-75 aspect-square object-cover"
                />
            </div>
        </div>
        <div
            class="absolute w-full h-full z-10 top-0 pointer-events-none"
            style="background-image:linear-gradient(180deg, rgba(0,0,0,1) 0%, rgba(0,0,0,1) 10%, rgba(255,255,255,0) 100%)"
        />
    
    </div>
    <div
        class="border-b-2 py-14 border-white flex flex-row items-center gap-16 relative pointer-events-none select-none w-full"
    >
        <img
            src="/blue.png"
            class="absolute w-full h-full object-cover object-center"
        />
        <CoolText text={"kto takoi lodka???"} color={"black"} />
        <div
            class="absolute w-full h-full opacity-20 pointer-events-none"
            style="background-image: url(/noice.png);"
        />
    </div>

    <div
        class="border-b-2 border-white bg-black flex flex-col gap-2 overflow-hidden"
    >
      
        <div class="p-10">
            <p
                class="w-full text-gray-500"
                style="font-family: ClashDisplay-SemiBold; font-size: 98px; "
            >
                lodka eto ne mark zuckerberg.
            </p>
            <div
                class="flex flex-row justify-center items-center w-full border-2 border-white h-[500px] overflow-hidden relative"
            >
                <div class=" grow h-full relative">
                    <img
                        src="./b53d30e509b44bfc5f7bf3d3a03cc000fcd50623.jpeg"
                        class=" absolute w-full h-full"
                    />
                </div>
                <div class=" grow h-full relative">
                    <img
                        src="./lodka_avatar.png"
                        class="  absolute w-full h-full"
                    />
                </div>
                
            </div>
        </div>
        <div>
            <img class="h-screen" src="https://assets.entrepreneur.com/content/3x2/2000/20150316195218-facebook-mark-zuckerberg-ceo.jpeg?format=pjeg&auto=webp&crop=4:3" />
        </div>
        <p
            class="w-full"
            style="font-family: ClashDisplay-SemiBold; font-size: 98px; "
        >
            lodka ne pridumal google.com
        </p>
        <div class="  w-full h-screen p-36  flex flex-row justify-center items-center  gap-20">
            <img class="w-[500px] " src="https://www.peoples.ru/undertake/founder/mark_zuckerberg/PPNECXz5oSM9j.jpeg" />
            <p  style="font-family: ClashDisplay-SemiBold; font-size: 98px; ">
                <span class="text-gray-500" style=" font-family: ClashDisplay-SemiBold;">"net ya ne riba" </span>- lodka
            </p>
        </div>
        <Tags/>
    </div>
    <div
        class="border-b-2 py-14 border-white flex flex-row items-center gap-16 relative pointer-events-none select-none w-full"
    >
        <img
            src="/pink.png"
            class="absolute w-full h-full object-cover object-center"
        />
        <CoolText text={"kakoui sledushii **season** fortnite?"} color={"black"} />
        <div
            class="absolute w-full h-full opacity-20 pointer-events-none"
            style="background-image: url(/noice.png);"
        />
    </div>
    <p  style="font-family: ClashDisplay-SemiBold; font-size: 48px; ">
        a ya ne yebu.
    </p>
