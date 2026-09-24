<script>
    const { title, img, description, helps, guides, hours, slug } = $props();
</script>

<a href={"/games-xbox/" + slug}>
    <div class="p-10 pt-4 text-center gap-2 text-mist-200">
        <img src={img} alt={title} />
        <p>{title}</p>
        <p>{description}</p>
        <p>{helps}</p>
        <p>{guides}</p>
        <p>{hours}</p>
    </div>
</a>
