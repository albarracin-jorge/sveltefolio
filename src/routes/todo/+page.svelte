<script>
	import Input from '../../components/todo/Input.svelte';
</script>

<main>
	<h1>Aca ira el todo</h1>
	<Input />
</main>

<style>
	@import '/static/app.css';
	main {
		margin: 0;
		width: 100%;
		height: calc(100svh - 84px);
		background-color: var(--bg-color);
	}
	h1 {
		margin: 0;
		color: var(--font-color);
	}
</style>
