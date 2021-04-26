<script>
	export let icon;
	export let name;
</script>

<div id="usrcontainer">
	<prow class="font-bold">
		<div style="height: 45px; display: inline-block;"><img src={icon} alt={`User ${name}`}></div><h5 class="text-primary-100">{name}</h5>
	</prow>
</div>
<style>
	#usrcontainer {
		padding: 15px 0 15px 0;
	}
	prow {
		display: flex;
		align-items: center;
		flex-direction: row;
	}
	img {
		border-radius: 100%;
		height: 40px;
		margin-right: 15px;
	}
</style>