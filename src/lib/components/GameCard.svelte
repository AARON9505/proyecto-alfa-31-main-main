<script>
    const { title, img, description, helps, guides, hours} = $props()
</script>

<div class="p-10">
    <img src={img} alt="">

    <p>{title}</p>
    <p>{description}</p>
    <p>{helps}</p>
    <p>{guides}</p>
    <p>{hours}</p>


</div>