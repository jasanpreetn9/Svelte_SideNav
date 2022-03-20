<script>
	import globals from '../global.css';
	import Sidebar from '../components/Nav.svelte';
	let sidebar_show = false;
</script>

<scelte:head>
	<title>Anime</title>
</scelte:head>
<button on:click={() => (sidebar_show = !sidebar_show)}>&#9776</button>


<Sidebar bind:show={sidebar_show} />
<slot />

<style>
	button {
		left: 6;
		top: 15px;
		border: none;
		color: white;
		background-color: transparent;
		font-size: 40px;
		cursor: pointer;
	}
</style>
