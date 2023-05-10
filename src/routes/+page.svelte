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
			name: 'Calculator App',
			url: '/calculator'
		},
		{
			name: 'Tic Tac Toe App',
			url: '/tictactoe'
		}
	];
</script>

<h1>Welcome to Sveltefolio</h1>
<p>
	In this place i will rest some applications making whit Svelte & SvelteKit
	feauters. My goal is show humble but funny stuffs we can make whit this
	beautyfull framework
</p>
{#each LINK_APPS as link}
	<HomeCard data={link} />
{/each}
<!-- Todo: crear 4 mini apps -->
