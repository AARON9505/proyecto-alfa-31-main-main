<script>
    const { title, img, description, helps, guides, hours, id, slug} = $props()
</script>

<a href={"/games/" + slug}>
    <div class="p-10 text-center gap-2 pt-4 text-mist-200">
    <img src={img} alt="">
    <p>{title}</p>
    <p>{description}</p>
    <p>{helps}</p>
    <p>{guides}</p>
    <p>{hours}</p>
    </div>

</a>