<script context="module">
	import { browser, dev } from '$app/env';

	// we don't need any JS on this page, though we'll load
	// it in dev so that we get hot module replacement...
	export const hydrate = dev;

	// ...but if the client-side router is already loaded
	// (i.e. we came here from elsewhere in the app), use it
	export const router = browser;

	// since there's no dynamic data here, we can prerender
	// it so that it gets served as a static asset in prod
	export const prerender = true;
</script>

<svelte:head>
	<title>About</title>
</svelte:head>

<div class="content">
	<h1>Sobre</h1>

	<p>
		Nós desenvolvemos o seu projeto utilizando as mais novas e eficientes tecnologias como SPA, Inteligência Artificial, PWA, e muitas outas, venha conhecer! Se você é desenvolvedor, pode fazer parte da nossa rede.
	</p>

	<!-- TODO lose the @next! -->
	<pre>COMEÇE AGORA SUA REVOLUÇÃO TECNOLOGICA</pre>

	
</div>

<style>
	.content {
		width: 100%;
		max-width: var(--column-width);
		margin: var(--column-margin-top) auto 0 auto;
	}
</style>
