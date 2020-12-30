<script>
	import Binder from './binder/binder.js';
</script>

<main class="zine">
	{#each Binder as EveryPage, i}
	<EveryPage page={i+1} />
	{/each}
</main>

<style lang="scss" global>
	@import 'bulma/bulma';
	

	main {
		background-color: lightgrey;
	}
</style>
