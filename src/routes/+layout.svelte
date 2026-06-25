<script lang="ts">
	import favicon from '$lib/assets/favicon.svg'; // remember to replace this

	let { children } = $props();
</script>

<svelte:head>
	<link rel="icon" href={favicon} />
	<link rel="stylesheet" href="src/app.css"/>
	<title>[Font name]</title>
</svelte:head>

{@render children()}
