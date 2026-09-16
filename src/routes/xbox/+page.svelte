<script>
    // @ts-ignore
    import  Icon  from  '@iconify/svelte';
</script>

<section class="flex justify-end items-center gap-2 py-50 text-mauve-200">
    <div class="flex-1  relative pt-110 pb-50  px-47 border-4 border-text-cyan-400text rounded-3xl overflow-hidden">
      
        <p class="font-bold text-3xl">HALO:COMBAT ENVOLVED</p>
       <img src="/halo.jpg" class="absolute top-0 left-0 -z-10 w-full h-full object-cover" alt="">
    </div>

    <div class=" bg-mauve-950 text-cyan-400 px-4">
        
        <Icon icon="fluent-mdl2:xbox-controller" width={32}/>
        <p class="font-bold text-xl">Multiplayer Servers</p>
        <p>classic-matchmaking</p>
        
        <Icon icon="fluent-mdl2:file-system" width={32}/>
        <p class="font-bold text-2xl">Dashboard Rev</p>
        <p>boot-directly</p>

            <Icon icon="arcticons:patrika-news" width={32}/>
         <p class="font-bold text-2xl">Xbox-News & Releases</p>
         <p> hideo kojima deal with xbox</p>
        
    </div>
</section>