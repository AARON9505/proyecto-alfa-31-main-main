<script>
// @ts-nocheck

    import { games } from '$lib/data/games'
    const { params } = $props()

    const mygames = games.find(
        (games) => games.slug == params.slug
    )


</script>

{#if games}

<h1 class="text-mist-200 text-2xl font-bold">{mygames.title}</h1>

<div class="text-mist-200 pb-30 pt-10 px-9">
     <img src={img} class="" alt="">
    <p>{mygames.description}</p>
    <p>{mygames.helps}</p>
    <p>{mygames.guides}</p>
    <p>{mygames.hours}</p>
</div>  
    
{/if}

