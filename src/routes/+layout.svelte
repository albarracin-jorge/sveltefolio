<script lang="ts">
	import { onMount } from 'svelte';
	import Scrollbar from 'smooth-scrollbar';

	onMount(() => {
		const scroller = document.querySelector('.scrollbar') as HTMLElement;
		Scrollbar.init(scroller, {
			damping: 0.05
		});
	});
</script>

<div class="scrollbar">
	<header><a href="/"><h1>SVELTEFOLIO</h1></a></header>
	<slot />
</div>

<style>
	@import '/static/app.css';
	.scrollbar {
		height: 100vh;
		width: 100%;
		overflow: auto;
	}
	header {
		background-color: var(--terciary-color);
		height: 84px;
		/* padding: 1rem; */
		text-align: center;
	}
	h1 {
		margin: 0;
	}
	a {
		text-decoration: none;
		color: var(--font-color);
	}
</style>
