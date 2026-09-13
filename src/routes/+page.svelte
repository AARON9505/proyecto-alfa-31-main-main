<script>
    import  Icon  from  '@iconify/svelte' ;
</script>

<section class="flex flex-col items-stretch text-cyan-400 px-3 py-2 font-bold">
    <p class="text-mist-200">SELECT YOUR SYSTEM</p>
    <p class="text-mist-400">Access guides of games and optimize your gaming experience.maximun performance</p>
    <p class="py-4">AYUDAS RAPIDAS</p>

    <div class="flex justify-between bg-mauve-950">
        
        <a href="bios-setup" class="flex items-center gap-1.5">
            <Icon icon="heroicons-solid:chip" />
            <p class="text-mist-200">Bios setup</p>
        </a>

        <a href="controller-mapping" class="flex items-center gap-1.5">
           <Icon icon="teenyicons:nes-outline" />
            <p class="text-mist-200">controller mapping</p>
        </a>

        <a href="optimization-guide" class="flex items-center gap-1.5"> 
       <Icon icon="eos-icons:compass" />
        <p class="text-mist-200">optimization guide</p>
        </a>
    </div>

    
    <section class="flex flex-col justify-betweens text-mauve-200 font-bold">

        <div>
        <p class=" flex-3 text-mist-200 20">Featured games</p>

        <div class="flex text-center justify-between px-1 py-40 relative pt-40 pb-10">
        <p>Forza Horizon</p>
        <img src="/forza.jpg" class="absolute top-0 left-0 -z-10 w-small h-full object-cover " alt="">
         
       <div class="pt-6">
        <p>Resident Evil:Requiem</p>
         <img src="/resident.jpg" class="absolute top-0 center-10 -z-10 w-small h-full object-cover"  alt="">
        </div>

        <div>
            <p>Mario Kart</p>
            <img src="/mario.jpg" class="absolute top-0 right-0 -z-10 w-small h-full object-cover " alt="">
        </div>

         

    </section>



 
</section>