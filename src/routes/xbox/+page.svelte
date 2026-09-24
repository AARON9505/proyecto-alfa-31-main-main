<script>
    // @ts-ignore
    import Icon from "@iconify/svelte";
    import GameCard from "./GameCard.svelte";
    import { games } from "$lib/data/games-xbox";
</script>

<section class="flex justify-end items-center pb-5 text-mauve-200 px-10 pt-3 ">
    <div
        class="flex-1 relative px-10 pt-110 pb-50 border-4 border-lime-500 text-lime-500 rounded-3xl overflow-hidden"
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

<section class="grid grid-flow-col grid-rows-3 px-10 pb-15 gap-5">
    <div
        class="flex-1 flex flex-col text-lime-500 px-3 rounded-lg border-b-lime-400 row-span-3 border-4 border-lime-500 py-3 pr-20"
    >
        <p class="font-bold text-4xl pb-2">COMPLETION GUIDE</p>
        <p class="text-3xl underline underline-offside pb-2">Chapter List</p>
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
        class="flex justify-between items-center px-20 w-360 col-span-2 text-lime-500 row-span-2 rounded-lg border-b-lime-400 border-4 border-lime-500 py-3 gap-5"
    >
        <p class="font-bold text-4xl">main object</p>

        <div class="flex items-center gap-1 text-2xl">
            <input type="checkbox" name="" id="" />
            <p class="flex flex-col">Infiltrate the control room</p>
        </div>

        <div class="flex items-center gap-1 text-2xl">
            <input type="checkbox" name="" id="" />
            <p>Retrieve the encrypted data core</p>
        </div>

        <div class="flex items-center gap-1 text-2xl">
            <input type="checkbox" name="" id="" />
            <p>Evacuate before the countdown ends</p>
        </div>
    </div>

    <div
        class=" flex justify-center items-center text-lime-500 gap-3 px-6 py-5 grid-cols-2 pt-5 rounded-lg border-b-lime-400 border-4 border-lime-500"
    >
        <p class="">SECRET COLLECTIBLES</p>

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

    <div
        class="grid-cols-3 flex flex-col text-lime-500 rounded-lg border-4 border-lime-500 py-3 px-3"
    >
        <p>BOSS STRATEGIES</p>

        <p>
            Use the plasma rifle to deplete shields before switching to the
            kinetic launcher for maximum damage. Stay mobile to avoid the
            ground-pound shockwave.
        </p>
    </div>
</section>

<p class="font-bold text-3xl text-lime-500 px-10">LIBRALY DIRECTORY</p>

<section class="grid grid-cols-3 gap-5 pb-2">
    {#each games as game}
        <GameCard
            slug={game.slug}
            description={game.description}
            img={game.img}
            title={game.title}
            helps={game.helps}
            guides={game.guides}
            hours={game.hours}
        />
    {/each}
</section>
