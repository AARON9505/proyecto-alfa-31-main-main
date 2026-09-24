<script>
    // @ts-ignore
    import Icon from "@iconify/svelte";
</script>

<section class="flex justify-end items-center py-10 text-mauve-200">
    <div
        class="flex-1 relative pt-110 pb-50 border-4 border-text-cyan-400text rounded-3xl overflow-hidden"
    >
        <p class="font-bold text-3xl">HALO:COMBAT ENVOLVED</p>
        <img
            src="/halo.jpg"
            class="absolute top-0 left-0 -z-10 w-full h-full object-cover"
            alt=""
        />
    </div>

    <div class=" bg-mauve-950 text-lime-500 px-10">
        <Icon icon="fluent-mdl2:xbox-controller" width={32} />
        <p class="font-bold text-3xl">Multiplayer Servers</p>
        <p>classic matchmaking</p>

        <Icon icon="fluent-mdl2:file-system" width={32} />
        <p class="font-bold text-3xl">Dashboard Rev</p>
        <p>boot directly</p>

        <Icon icon="arcticons:patrika-news" width={32} />
        <p class="font-bold text-3xl">Xbox-News & Releases</p>
        <p>hideo kojima deal with xbox</p>
    </div>
</section>

<section class="grid grid-flow-col grid-rows-3 px-20 pb-70">
        <div class="flex-1 flex flex-col text-lime-500 px-3 rounded-full border-b-lime-400 row-span-3">
            <p class="font-bold text-4xl pb-2">COMPLETION GUIDE</p>
            <p class="text-3xl underline underline-offside pb-2">
                Chapter List
            </p>
            <p>Chapter 1: The arrival</p>
            <Icon icon="akar-icons:play" />
            <p>Chapter 2: into the void</p>
            <Icon icon="streamline:padlock-square-1-remix" />
            <p>Chapter 3: The core</p>
            <Icon icon="streamline:padlock-square-1-remix" />
            <p>Chapter 4: Final descent</p>
            <Icon icon="streamline:padlock-square-1-remix" />
        </div>

        <div
            class="flex flex-col px-30 w-280 col-span-2 justify-start text-lime-500 row-span-2"
        >
            <p class="font-bold text-2xl">main object</p>
            
            <div class="flex items-center gap-1">
                <input type="checkbox" name="" id="" />
                <p class="flex flex-col">Infiltrate the control room</p>
            </div>

            <div class="flex items-center gap-1">
                <input type="checkbox" name="" id="" />
                <p>Retrieve the encrypted data core</p>
            </div>
            
            <div class="flex items-center gap-1">
                <input type="checkbox" name="" id="" />
                <p>Evacuate before the countdown ends</p>
            </div>
        </div>

        <div class=" flex flex-col text-lime-500 gap-1 px-30">
            <p>SECRET COLLECTIBLES</p>
            
        </div>
        
        <div class="flex items-center">        
        
            <div class="">
                <Icon icon="boxicons:cube-alt" width={32} />
                <p>01/03</p>
                
            </div>
            
            <div>
                    <Icon icon="game-icons:medal-skull" width={32} />
                    <p>00/01</p>
    
                </div>
    
                <div>
                    <Icon icon="boxicons:coins" width={32} />
                    <p>00/05</p>
    
                </div>

        </div>
        

    
</section>
