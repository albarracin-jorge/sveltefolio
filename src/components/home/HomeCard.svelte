<script lang="ts">
	type Link = {
		name: string;
		url: string;
	};
	export let data: Link;
</script>

<div>
	<a href={data.url}>{data.name}</a>
</div>
