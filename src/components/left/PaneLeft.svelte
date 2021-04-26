<script>
	import People from './People.svelte';

	export let people;
</script>

<pane class="bold text-primary-100">
	<a href="dashboard" style="margin-bottom: 60px;"><img src="dash.svg" alt="Dashboard"></a>
	<h4>People</h4>
	<People people={people}></People>
</pane>

<style>
	pane {
		display: flex;
		flex-direction: column;

		top: 0;
		position: sticky;
		padding-top: 30px;
	}
</style>