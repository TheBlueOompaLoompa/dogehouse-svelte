<script>
	import Person from "./Person.svelte";

	export let people;
</script>

<h6 class="font-bold text-sm mt-3 text-primary-300 extendo-mode">ONLINE</h6>
{#each people as person}
{#if person['online']}
	<Person icon={person['icon']} name={person['name']}></Person>
{/if}
{/each}

<h6 class="font-bold text-sm mt-3 text-primary-300 extendo-mode">OFFLINE</h6>
{#each people as person}
{#if person['offline']}
	<Person class="mt-3" icon={person['icon']} name={person['name']}></Person>
{/if}
{/each}

<style>
	.extendo-mode {
		margin-bottom: 15px;
	}
</style>