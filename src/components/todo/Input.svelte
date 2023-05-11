<script lang="ts">
	let text: string;

	$: text;

	$: console.log(text);
</script>

<section>
	<input type="text" placeholder="what task do you have?" bind:value={text} />
</section>
