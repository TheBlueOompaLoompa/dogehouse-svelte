<script>
	import PaneLeft from '../components/left/PaneLeft.svelte';
	import SvHead from './head.svelte';

	export let segment;

	let people = [
		{
			name: 'Idiot',
			icon: "logo-192.png",
			online: true,
		}
	];

</script>

<style>
	main {
		display: grid;
		grid-template-columns: 235px 640px 325px;
		column-gap: 60px;

		position: relative;

		scrollbar-width: thin;
		
	}
</style>

<svelte:head>
	<SvHead page={segment}></SvHead>
</svelte:head>

<main>
	<PaneLeft people={people}></PaneLeft>
</main>