<script lang="ts">
	import './layout.css';
	import favicon from '$lib/assets/favicon.svg';
    import Icon from '@iconify/svelte';

	let { children } = $props();
</script>

<svelte:head><link rel="icon" href={favicon} /></svelte:head>



<nav class="flex justify-between bg-mauve-950  text-mist-200 items-center px-3 py-2 font-bold font-tecno">
	<p class="flex text-xl">PROYECT-ARC</p>

	<div class="bg-mauve-950 text-mist-200 rounded px-3.5 py-2.5 gap-6">
		<a href="/">Inicio</a>
		<a href="/xbox">xbox</a>
		<a href="/playstation">playstation</a>
		<a href="/nintendo">nintendo</a>
		<a href="/pc">pc</a>
		
	</div>

		<a class="bg-mauve-950 text-mist-200  flex items-center rounded px-3.5 py-2.5" href="/login">
		<Icon icon="ant-design:user-add-outlined widht:{50}" />
		<p>login</p>
	</a>

	<a class="bg-mauve-950  text-mist-200  rounded px-3.5 py-2.5" href="/search">
		<span></span>
		<p>search </p>
	</a>

</nav>

{@render children()}

<footer class="flex justify-center gap-5 bg-mauve-950 text-mist-200">
	<p>PROYECT-ARC</p>

	<div class="flex gap-5">
		<!-- svelte-ignore a11y_consider_explicit_label -->
		<a href="/creator">creator</a>
		<p>privacy</p>
		<p>hardware</p>
		<p>community</p>
	</div>
</footer>
