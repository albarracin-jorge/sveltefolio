<script lang="ts">
	import HomeCard from '../components/home/HomeCard.svelte';
	const LINK_APPS = [
		{
			name: 'Todo App',
			url: '/todo'
		},
		{
			name: 'Blog App',
			url: '/blog'
		},
		{
			name: 'Book List',
			url: '/booklist'
		}
	];
</script>

<main>
	<p>
		In this place i will rest some applications making whit Svelte & SvelteKit
		feauters. My goal is show humble but funny stuffs we can make whit this
		beautyfull framework
	</p>
	{#each LINK_APPS as link}
		<HomeCard data={link} />
	{/each}
	<!-- Todo: crear 4 mini apps -->
</main>

<style>
	@import '/static/app.css';
	main {
		padding: 24px;
		background-color: var(--bg-color);
		height: calc(100vh - 84px);
	}
	p {
		margin: 0;
		color: var(--font-color);
	}
</style>
