<script>
// @ts-nocheck

    import GameCard from "$lib/components/GameCard.svelte";
    import { games } from "$lib/data/games";
import Icon from "@iconify/svelte";
</script>

<section class="flex flex-col items-stretch text-mauve-200 px-3 py-2 font-bold font-tecno">
    <p class="text-mist-200 text-2xl">SELECT YOUR SYSTEM</p>
    <p class="text-mist-400">
        Access guides of games and optimize your gaming experience.maximun
        performance
    </p>
    <p class="py-4">AYUDAS RAPIDAS</p>

    <div class="flex justify-between px-2">
        <a
            href="bios-setup"
            class="flex items-center gap-1 rounded-lg text-cyan-300  border-4 border-b-cyan-300 border-r-4 border-b-4 border-l-4 border-t-4 px-7 py-7 transition delay-150 duration-300 ease-in-out hover:-translate-y-1 hover:scale-110 shadow-2xl"
        >
            <Icon icon="heroicons-solid:chip" />
            <p class="items-center font-tecno">Bios setup</p>
        </a>

        <a
            href="controller-mapping"
            class="flex items-center gap-1 rounded-lg  border-4 text-cyan-300 border-b-cyan-300 border-r-4 border-b-4 border-l-4 border-t-4 px-7 py-7 transition delay-150 duration-300 ease-in-out hover:-translate-y-1 hover:scale-110"
        >
            <Icon icon="teenyicons:nes-outline" />
            <p class="">controller mapping</p>
        </a>

        <a
            href="optimization-guide"
            class="flex items-center gap-1 rounded-lg  border-4 text-cyan-300 border-b-cyan-300 border-r-4 border-b-4 border-l-4 border-t-4 px-7 py-7 transition delay-150 duration-300 ease-in-out hover:-translate-y-1 hover:scale-110"
        >
            <Icon icon="eos-icons:compass" />
            <p class=" ">optimization guide</p>
        </a>
    </div>

    <section class="flex flex-col justify-betweens text-mist-950 font-bold">
        <div>
            <p class=" flex-3 text-mist-200">Featured games</p>
        </div>

        <div
            class="flex text-center justify-between px-1 py-30 relative pt-3 pb-3">
            
            
            <div class=" relative px-5 pt-5 pb-10 flex-1">
                <p class="text-lime-500">forza horizon</p>
                <img
                    src="/forza.jpg"
                    class="absolute top-0 left-0 z-10 h-full w-full object-cover"
                    alt=""
                />
            </div>

            <div class=" relative px-5 pt-60 pb-4 flex-1">
                <p class="text-cyan-200">Resident Evil:Requiem</p>
                <img
                    src="/resident.jpg"
                    class="absolute top-0 left-0 center-10 -z-10 h-full w-full object-cover"
                    alt=""
                />
            </div>

            <div class=" relative px-5 pt-60 pb-4 flex-1">
                <p class="text-red-700">Mario Kart</p>
                <img
                    src="/mario.jpg"
                    class="absolute top-0 left-0 right-0 -z-10 h-full w-full object-cover"
                    alt=""
                />
            </div>
        </div>
    </section>

    <div class="pt-10">
        <p>staff picks</p>
    </div>

    <section class="flex justify-between items-center px-50 py-2 gap-13">
        <div
            class="pt-5 gap-1.5 rounded-xl bg-mauve-900 border-4 text-cyan-300 border-b-cyan-300 border-r-4 border-b-4 border-l-4 border-t-4 px-5 py-5"
        >
            <p class="text-cyan-300">shadow of the colossus</p>
            <p class=" text-xs text-balance">
                La historia sigue a Wander, un joven que viaja hacia una
                desolada región conocida como la Tierra Prohibida. los 16
                colosos de piedra que habitan esas tierras.
            </p>
            <button class="">READ GUIDE</button>
        </div>

        <div
            class="rounded-xl bg-mauve-900 border-4 text-cyan-300 border-b-cyan-300 border-r-4 border-b-4 border-l-4 border-t-4 px-5 py-5"
        >
            <p class="text-cyan-300">No Man's Sky</p>
            <p class="text-xs text-balance">
                No Man's Sky es un juego de ciencia ficción sobre exploración y
                supervivencia en un universo infinito generado de forma
                procedimental.
            </p>
            <button>READ GUIDE</button>
        </div>

        <div
            class="rounded-xl bg-mauve-900 border-4 text-cyan-300 border-b-cyan-300 border-r-4 border-b-4 border-l-4 border-t-4 px-5 py-5"
        >
            <p class="text-cyan-300">Big Walk</p>
            <p class="text-xs text-balance">
                Pasa el rato con tus amigos y perdeos en un mundo enorme. Una
                caminata cooperativa en línea de los creadores de Untitled Goose
                Game.
            </p>
            <button>READ GUIDE</button>
        </div>
    </section>

    <p class="py-5">GLOBAL GAMING NEWS</p>

    <section class=" flex-col columns-2 py-2">
        <div>
            <p class="text-cyan-300">Xbox</p>
            <p>
                Xbox confirmó que publicará PHYSINT, el juego de acción y
                espionaje creado por Hideo Kojima.
            </p>
        </div>

        <div>
            <p class="text-cyan-300">Playstation</p>
            <p>
                PlayStation Plus Extra y Premium confirman los juegos de
                septiembre, con Ninja Gaiden
            </p>
        </div>

        <div>
            <p class="text-cyan-300">nintendo</p>
            <p>
                Remake de Zelda: Ocarina of Time: Llegará a Nintendo Switch 2 el
                5 de noviembre
            </p>
        </div>

        <div>
            <p class="text-cyan-300">PC</p>
            <p>
                Tarjetas gráficas: Las GPUs de Nvidia y AMD mantienen una
                tendencia de aumento en costos por el encarecimiento de la
                memoria GDDR6 y GDDR7
            </p>
        </div>
    </section>

    <section class="grid grid-cols-3">

        {#each games as Game}
            <GameCard  slug={Game.slug} description={Game.description} img={Game.img} title={Game.title} helps={Game.helps} guides={Game.guides} hours={Game.hours}/>
        {/each}
    
    </section>
</section>
