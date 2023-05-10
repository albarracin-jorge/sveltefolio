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
	<header>Esto es un header</header>
	<slot />
</div>

<style>
	.scrollbar {
		height: 100vh;
		width: 100%;
		overflow: auto;
	}
</style>
