<script>
	import Header from './components/Header.svelte';
	import CardList from './components/CardList.svelte';

	let items = [
		{
			id: 1,
			screenname: "b1eedingr0mance",
			currently: "Euphoria",
			action: "watching",
			platform: "HBO"
		},
		{
			id: 2,
			screenname: "kheyralikesemo",
			currently: "Lazy Eye",
			action: "listening to",
			platform: "Spotify"
		},
	]
</script>

<Header />
<main>
	<CardList {items} />
</main>