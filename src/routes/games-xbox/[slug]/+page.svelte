<script>
    // @ts-nocheck
    import { games } from "$lib/data/games-xbox";

    const { params } = $props();
    const game = games.find((item) => item.slug === params.slug);
</script>

{#if game}
    <section class="px-3 text-lime-500">
        <h1 class="text-4xl font-bold">{game.title}</h1>

        <img class="max-w-3xl" src={game.img} alt={game.title} />
        <p>{game.description}</p>
        <p>{game.helps}</p>
        <p>{game.guides}</p>
        <p>{game.hours}</p>
    </section>
{:else}
    <section class="p-10 text-mist-200">
        <h1 class="text-4xl font-bold">Juego no encontrado</h1>
    </section>
{/if}
